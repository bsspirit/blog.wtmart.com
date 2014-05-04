title: 逆回购与远期收益率分解
date: 2013-11-01 12:04:49
author: Weilin Lin
categories:
- 债券货币市场
---

这里要解决的问题是放逆回购的最优问题，在平时放回购的时候，遇到的一个最常见的问题就是，我到底是放1天，2天，4天，还是7天？ 很显然要做出正确的决定必须要求我们能够对未来利率走向做出准确的判断，用比较专业的术语来讲的话，就叫&quot;远期利率&quot;（forward rate）。举个很简单的一个例子，比如现在交易终端各个期限的回购报价如下：

|回购代码| 资金借出日期| 资金可用日期| 实时报价|
| --------   | -----  | ----  |  ------ |
|204001.SH| 20131101| 20131104| 1.648%|
|131809.SZ| 20131101| 20131105| 2.000%|
|131801.SZ| 20131101| 20131115| 3.838%|
|204014.SH| 20131101| 20131129| 4.070%|

那么在这样的一个报价情况下，我们应该放哪个回购比较划算？ 如上所示，这个问题涉及到我们对未来利率走势的判断，但是因为这几个回购利率之间不是相互独立的（很显然期限比较长的回购利率隐含了较短的回购利率），我们这里要做的就是对这几个回购进行分解，得到彼此之间相互独立的远期利率。

基于我们开发的金融工具箱，我们可以实时地对这个报价进行分解，相关的程序如下（注意：这里的程序已经能在所有的环境里面运行，不仅仅是基于server3）

```{r}
## This is the script to run the repo application
## load packages.
library(quantmod);
library(RMySQL);
library(TTR);
library(rredis);
library(PerformanceAnalytics);
library(datatools);
require(googleVis);
options(warn=-2);
sqlQuery <- dbGetQuery;
redisConnect(host = "xxx");

## 从APE上面读取实时的市场数据
mktDf <- redisMGet(c("bondFutureWind.time","bondFutureWind.jtid","bondFutureWind.rt_time","bondFutureWind.last","bondFutureWind.bid1","bondFutureWind.bsize1","bondFutureWind.ask1","bondFutureWind.asize1"));
mktDf <- as.data.frame(mktDf, stringsAsFactors = FALSE);
colnames(mktDf) <- c("time","jtid","TradeTime","LastPx","BidPx1","BidSize1","OfferPx1","OfferSize1");
jtids <- c("CN204001.SH","CN204002.SH","CN204003.SH","CN204004.SH","CN204007.SH","CN204014.SH","CN204028.SH","CN204091.SH","CN131810.SZ","CN131811.SZ","CN131800.SZ","CN131809.SZ","CN131801.SZ","CN131802.SZ","CN131803.SZ","CN131805.SZ");
names <- c("GC001","GC002","GC003","GC004","GC007","GC014","GC028","GC091","R-001","R-002","R-003","R-004","R-007","R-014","R-028","R-091");
days <- c(1,2,3,4,7,14,28,91,1,2,3,4,7,14,28,91);
data <- data.frame(jtid=jtids, name=names, day=days);
data <- merge(data, mktDf, by="jtid");

## 交易所回购日期的详细计算（资金场内可用）
date <- date.currentDate(); # 交易日，成交日, 清算日
if(!date.isBusDate(date)) date <- date.convert(date.toBusDate(date, shift=-1, region="CN"), format="YYYYMMDD");
settleDate <- date.toBusDate(date, region="CN", shift=1); # 资金到帐日
endDates <- date.convert(date) + data$day*60*60*24; # 到期日
endDates <- date.toBusDate(endDates, region="CN", shift=0);# 到期清算日
data$day.EX <- as.integer(difftime(endDates, date.convert(date), units="days"));
data$endDate.EX <- date.convert(endDates, format="YYYYMMDD");

## 银行间回购日期的详细计算（资金场内可取）
date <- date.currentDate(); # 交易日，成交日, 清算日
if(!date.isBusDate(date)) date <- date.convert(date.toBusDate(date, shift=-1, region="CN"), format="YYYYMMDD");
settleDate <- date.toBusDate(date, region="CN", shift=1); # 资金到账日
endDates <- date.convert(date) + data$day*60*60*24; # 到期日
endDates <- date.toBusDate(endDates, region="CN", shift=0);# 到期清算日
endDates <- date.toBusDate(endDates, region="CN", shift=1);# 资金到期日
data$day.IB <- as.integer(difftime(endDates,settleDate, units="days"));
data$endDate.IB <- date.convert(endDates, format="YYYYMMDD");
data$day <- as.integer(data$day);
data$LastPx.EX <- data$LastPx*data$day/data$day.EX;
data$LastPx.IB <- data$LastPx*data$day/data$day.IB;
data$coef.EX <- p(data$day,"/",data$day.EX);
data$coef.IB <- p(data$day,"/",data$day.IB);
data <- data[,c("jtid","name","TradeTime","day","day.EX","day.IB","endDate.EX","endDate.IB","LastPx","LastPx.EX","LastPx.IB","BidPx1","BidSize1","OfferPx1","OfferSize1","coef.EX","coef.IB")];
data <- data[order(data$jtid,data$day),];
rownames(data) <- NULL;

## 交易所逆回购分析
data <- data[,c(&quot;jtid&quot;,&quot;day.EX&quot;,&quot;LastPx.EX&quot;,&quot;endDate.EX&quot;)];
colnames(data) <- c("data","day","LastPx","endDate");
data <- data[order(data$day, data$LastPx, decreasing=TRUE),];
data <- data[!duplicated(data$day),];
data <- data[order(data$day),];

## 生成远期利率表
data$LastPx.C <- log(1+data$LastPx/100);
endDates <- data$endDate;
diffDates <- as.integer(difftime(date.convert(endDates), date.convert(date),units="days"));
endDates <- p(diffDates, " (", endDates, ")" );
df <- array(data = NA, dim = c(length(endDates), length(endDates)+1), dimnames = list(date1=endDates, date2=c(p(0, " (",date,")"),endDates)));
df[,1] <- data$LastPx/100;
diffDates_cp <- diffDates;
for(j in 2:(ncol(df)-1)){
# R1: df[j-1,j-1]
# T1:
# R2: df[j:nrow(df),j-1]
# T2:
R1 <- df[j-1,j-1];
R2 <- df[j:nrow(df),j-1];
T1 <- diffDates[j-1];
T2 <- diffDates[j:nrow(df)];
#df[j:nrow(df),j] <- (R2*T2-R1*T1)/(T2-T1);
r <- (1+R2*T2/365)/(1+R1*T1/365)-1;
df[j:nrow(df),j] <- r*365/(T2-T1);
## adjuste diffDates to origin.
diffDates <- diffDates_cp-diffDates_cp[j-1];
}

### 得到逆回购的分解表
df
```

![repo](/uploads/2013/11/repo.png)


	 

	 

	 