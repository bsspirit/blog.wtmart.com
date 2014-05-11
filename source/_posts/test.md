title: This is a test Rmd demo
date: 2014-05-11 10:04:18 
author: Weilin Lin
categories:
- 大类资产配置研究
- 高收益债
---
This is an R Markdown document. Markdown is a simple formatting syntax for authoring web pages (click the **MD** toolbar button for help on Markdown).

When you click the **Knit HTML** button a web page will be generated that includes both content as well as the output of any embedded R code chunks within the document. You can embed an R code chunk like this:




Plot and save it in the file path

```r
png = bloomberg.gg.daily("Yr10", 20080101)
image.tmp = "/home/amg/git/blog.wtmart.com/source/images/ggdaily.png"
ggsave(png, file = image.tmp, width = 8, height = 5)
```


**图 1：ggplot 画图测试** 
* ------------------------------------- *
![高收益债样本个数](/images/ggdaily.png)
* ------------------------------------- *
资料来源：Wind,COS Inv系统



```r
n <- 100
x <- rnorm(n)
y <- 2 * x + rnorm(n)
out <- lm(y ~ x)
library(xtable)
tab <- xtable(summary(out)$coef, digits = c(0, 2, 2, 1, 2))
print(tab, type = "html")
```

<!-- html table generated in R 3.0.1 by xtable 1.7-1 package -->
<!-- Sun May 11 10:04:20 2014 -->
<TABLE border=1>
<TR> <TH>  </TH> <TH> Estimate </TH> <TH> Std. Error </TH> <TH> t value </TH> <TH> Pr(&gt |t|) </TH>  </TR>
  <TR> <TD align="right"> (Intercept) </TD> <TD align="right"> 0.02 </TD> <TD align="right"> 0.11 </TD> <TD align="right"> 0.2 </TD> <TD align="right"> 0.87 </TD> </TR>
  <TR> <TD align="right"> x </TD> <TD align="right"> 2.10 </TD> <TD align="right"> 0.11 </TD> <TD align="right"> 19.2 </TD> <TD align="right"> 0.00 </TD> </TR>
   </TABLE>






