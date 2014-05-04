title: 量化选股介绍和思考-追涨杀跌的简单例子
date: 2013-11-02 15:24:06
author: Weilin Lin
categories:
- 股票市场
---

之前实习做过一些关于量化选股的工作，从那时起我就对这种投资方法很感兴趣。但是这些年来可以看到国内做这方面的公募和对冲基金都不少，能把这种投资方法运用好的几乎没有。这也一直引起了我对于这套投资体系的思考，为何在国内市场运用这种较为科学的投资方法却没有取得较好的结果。对比一下国内传统的投资方法，基本上是采用研究员对每个行业进行覆盖，然后行业研究员通过跟上市公司的交流和研究在行业里面选出能击败整个行业平均水平的股票，从而创造超额收益(alpha)。 我个人认为量化选股的投资方法相对于传统的这种方法的话，主要有以下几点优势和略势：

*   传统研究方法对现金流的来源把握的更加精细，有可能找出&ldquo;牛股&rdquo;。而量化投资一般不会去判断个股的情况，而是批量的研究股票。所以传统的方法有可能通过一只股票实现非常好的收益，量化选股没法做到这一点。
*   传统的投资方法具有较强的经济直觉和背景，这样的话人能在这其中发挥主观能动性。而量化投资很多的时候更像是数据挖掘，做量化投资的人很多往往也是计算机或者统计出身，经济直觉较差，所以就造成量化投资缺少思想的尴尬情况。反观传统投资，可以说得很玄乎，就像巴菲特之类的，很多的时候甚至都能提升到哲学的层次，别人也很难模仿其投资的方式。而量化选股的思想往往较为简单，都是一些较为明显的统计规律或者是一些大家都知道的基本面指标，宽客的圈子里面大家的投资策略很容易相互模仿。
*   普通的行业研究员很难看多个行业（虽然这些行员大部分至少都是清北名校硕士毕业，但是每个个体的时间和能力的限制使得其很难覆盖多个行业）。那么就会带来的一个问题就是这些研究员不会对不同行业的股票进行比较，而量化投资却没有这个问题，可以把研究股票的范围很容易的推广到整个市场的股票。
*   传统的研究方法一般会倾向于把筹码赌在少数的几只股票上面，而且传统的投资方法基本上可以说是没有风险的意识，可能现在国内的行业研究员基本上都不知道股票的风险模型，不知道股票的风险可能有哪些来源。相比之下，量化选股的投资方式有非常精细的风险模型，甚至还有一套及其复杂的优化器能够对各种风险进行严密的控制。
*   传统的投资容易受人为情感的影响，除非是人格分裂，否则很难找到一个传统的基金经理又具有价值投资的理念，又能很好地投资于成长股。比如巴菲特，基本上就没碰过成长股，一辈子都是坚持其价值投资的投资哲学。但是相比之下，量化选股的投资方式能够很好地融合价值投资和成长股投资这两种风格（这些对应到数学上就是一个简单的加减乘除的问题），而且通过变换模型能够很容易地在价值和成长之间进行切换。传统的基金经理却很难做到这一点，这是因为人到了一定的年纪之后（特别是过去取得一些成功的人），思想会有一种惰性，不愿意去改变其认识世界的方法（这个现象应该存在于各个行业，我个人认为是人类的本性之一，只不过在自负傲慢的金融投资圈子这个体现得更为明显而已）。
*   还有很重要的一点，量化选股的成本要远远低于传统的投资方法。开一家对冲基金，如果是采用量化投资的方式，基本上只需要雇几个综合能力较好的phd就可以运营，等整个投资框架建立起来之后，甚至可以裁掉部分员工只留下维护人员即可。而传统的投资方法需要雇佣大量的研究员天天跟上市公司沟通，就算<span style="font-size: 13px;">整个投资框架建立起来也无法裁掉他们，而且现在即使是国内的股票研究员工资也是接近于华尔街，成本非常地高。</span>

	综合上面对比的几个优缺点，我个人认为量化选股这种投资方式为何没有在国内发展起来主要有以下几个原因：

*   会使用量化这个工具，又深入了解中国市场的人实在太少。
*   量化选股要交易的是一个群体性的规律，所以会买卖大量的股票，这样子就会造成相比于传统投资&rdquo;找牛股&ldquo;的方法波动新会小很多，所以通过量化投资的方式很难在短期内击败传统的投资方法。当然这个问题之所以得不到解决还是跟国内股票市场无法使用杠杆这个因素息息相关，这一点在很大程度上限制了量化选股在我国的发展。
*   对冲工具太过于单一，即使能放杠杆，也可能遭受黑天鹅的冲击。目前国内放空的工具少得可怜，基本上只有股指期货可以做空，而我们知道股指期货对应的是沪深300，你如果想对冲行业风险、市值风险等更细一些的风险的话，根本没有相应的工具。量化选股投资最大的优势就是研究某一稳定的统计规律，对于其它不熟悉的影响因素全部通过做空对冲掉风险，在这基础上通过放杆杆获得高收益。而如果国内做空工具不完善的话，即使有一天股票能做质押回购做杠杆了，由于承担了不必要的风险，黑天鹅事件很有可能一下子就把整个基金击倒。

	以上是个人观点，下面通过实际例子讲解一个简单的追涨杀跌策略的&rdquo;宽客&ldquo;视角。追涨杀跌估计是每个刚开始进入股市的人的最喜欢的投资方式了，对于宽客来说，首要任务就是对这种策略进行量化和回测检验，加以经济基本面的理解：

1.  **首先载入必须的R包**

```{r}
library(devtools)
install_github("COSinvestment","casunlight",subdir="quantutils",auth_user="***",password="***")
install_github("COSinvestment","casunlight",subdir="datatools",auth_user="***",password="***")
library(datatools);
utils.init();
```

2.  **将追涨杀跌的这种策略模型化，生成买卖的信号**
```{r}
pr.writeCSV <- function(startDate, endDate=startDate, region, outDir=NULL, verbose=TRUE)
{
  if (is.null(outDir))
    outDir <- p(DATA.DIR, "/", tolower(region),"/daily/signal/pr");
  if (!file.exists(outDir)) dir.create(outDir, recursive = TRUE, showWarnings=FALSE);
  lags       <- c(3, 5, 10, 20, 40, 50, 60, 80, 100, 120);
  lagVars    <- p("pr", as.character(lags), "d");  dataStartDate <- date.convert(date.toBusDate(date=startDate, region=region, shift = -max(lags+1), forward=FALSE), format="YYYYMMDD");
  dataEndDate   <- date.convert(date.toBusDate(date=endDate,   region=region, shift = -1,           forward=FALSE), format="YYYYMMDD");
  mktDf         <- mktData(dataStartDate, dataEndDate, vars="ret", region=region);
  mktDf         <- mktDf[!is.na(mktDf$jtid), ];
  retArr        <- df.dfToArray(mktDf, keyCols=c("jtid","date"),"ret")[,,];
  retArr[is.na(retArr)] <- 0.0;  prcMat <- t(apply(1+retArr, 1, cumprod));  dates  <- date.convert(date.range(startDate, endDate, region=region), format="YYYYMMDD");  jtids  <- dimnames(prcMat)[[1]];
  lst <- list();
  for (date in dates)
    {
      cat(date);
      df <- data.frame(jtid=jtids, date=rep(date, length(jtids)));
      dateL1 <- date.convert(date.toBusDate(date, shift=-1, region=region),format="YYYYMMDD");
      for (i in 1:length(lags))
        {
          lag          <- lags[i];
          lagVar       <- lagVars[i];
          dateLL       <- date.convert(date.toBusDate(date, shift=-lag, region=region),format="YYYYMMDD");
          ## only save those who was above ma line.
          tmpDates     <- date.convert(date.range(dateLL, dateL1, region=region), format="YYYYMMDD");
          ## Deternmin whether ablove MA20d.
          df[[lagVar]] <- ifelse(prcMat[df$jtid, dateL1]>rowMeans(prcMat[df$jtid, tmpDates,drop=FALSE]),prcMat[df$jtid, dateL1]/prcMat[df$jtid, dateLL]-1,-2);
          ## notice: NOT to use order command here, it will caused serious error !!
          #df[[lagVar]] <- prcMat[df$jtid, dateL1]/prcMat[df$jtid, dateLL]-1;        }      lst[[date]] <- df;
      cat("\b\b\b\b\b\b\b\b");
    }
  prDf <- df.rbindList(lst);  utils.writeCSV(prDf[, c("jtid", "date", lagVars)], outDir, filePrefix="pr",startDate=startDate, endDate=endDate,  region=region, verbose=verbose);
  invisible(prDf);
}

pr.writeCSV(20130901, 20131031, region="CN", outDir = "~/temp/pr");
```

**对该策略进行回测检验结果**
```{r}
### 回测

cfgLst.simple <- list(
                   region = "CN",
                startDate = 20130901,                                     ## the startDate to estimate beta
                  endDate = 20131031,                                     ## the end to estimate beta
           runFromScratch = TRUE,                                         ## True <-> run from scratch; FALSE <-> continue backtesting with existing portfolio
         tradingDatesFile = NULL,                                         ## if a file of trading dates is given, then will only trade at such given dates; Using file format of ~/data/cn/busDate/busDates.csv
            rebalanceRule = "simple",                                     ## rule used to construct the portfolio
                 portType = "L",                                          ## L <-> Long Onley; S <-> Short Only; LS <-> Long Short
                  portWgt = "eq",                                         ## weights used to construct the portfolio
         tradeInThreshold = 1,                                            ##  buy stock from where its alpha ranked top 1 of the stock.
        tradeOutThreshold = 100,                                          ##  sell stock if its alpha is NOT in the top 150 of stocks.
       investSizePerStock = 2e6,                                          ## each time buy investSizePerStock RMB for each selected stock
                 tradeLot = 100,                                          ## must trade the mulitples of tradeLot shares
 volumeParticipationLimit = 0.1,                                          ## trade limit. (0.01 means can't trade more than 1% of one day's total trading volume for a given stock a day)
                 alphaDir = "~/temp/pr",                   ## directory of the alpha data
          alphaFilePrefix = "pr",                                         ## directory of the alpha data
                 alphaVar = "pr20d",                                      ## alpha variable name
                  indexID = "CN000300",                                   ## indexID for the index used to compute beta
                 univType = "liquidityBased",                             ## universe type                        univRange = c(0,1),                                       ##
             saveHldFiles = TRUE,                                         ## TRUE <-> write out daily holding's files; FALSE <-> don't write out daily holding's files
               dataOutDir = "~/temp/CN/backtest/pr20d",                   ## data output dir
                  verbose = TRUE
)

cfgLst                   <- cfgLst.simple;
cfgLst                   <- backtest.loadData(startDate=NULL, endDate=NULL, cfgLst=cfgLst);
cfgLst                   <- backtest.loadAlpha(cfgLst=cfgLst);
cfgLst                   <- backtest.loadUniv(cfgLst=cfgLst);

## update data upto the endDate
cfgLst$cfgLst            <- backtest(cfgLst);
dataLst                  <- backtest.summary(cfgLst, pnlVar="betaAdjPnL",extraTC=0.002,plotToFile=TRUE);
```

3.  **回测结果展示**

![pr20d_backtest1](/uploads/2013/11/pr20d_backtest.gif)

![pr20d_backtest2](/uploads/2013/11/pr20d_backtest1.gif)

![pr20d_backtest3](/uploads/2013/11/pr20d_backtest2.gif)