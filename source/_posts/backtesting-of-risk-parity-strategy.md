title: Backtesting of Risk Parity Strategy
date: 2013-06-05 10:04:27
author: Weilin Lin
categories:
- 大类资产配置研究
---

一、目的：对风险平摊（Risk Parity）策略进行历史回测

二、背景：risk parity是目前非常热门的资产配置方法，但是对此不同的公司有不同的理解和做法。其中最为出名的是当前世界上最大的对冲基金Bridgewater提出的风险平摊概念。Bridgewater公司将其运用于其旗舰基金之一Beta1和Beta2（组合经理皆为公司创始人Ray Dalio先生），取得非常的成功。Risk parity具体的投资操作过程非常量化和复杂，但是思想却十分直观：构建一个在任何宏观经济环境下都能够获取稳定回报（当然是正回报）的投资组合。

三、回测模型要求：

1.  分析不同经济环境对于不同资产类别回报率的影响。由于不同的资产类别在不同经济环境中会有不同的表现，因此构建投资组合首先要对各资产类别在不同环境中的表现作分析。由于市场预期对资产类别的价格产生重要的影响，因此模型采用惊喜冲击指数作为宏观经济变量。即：任何一种资产类别的回报可以分解为：

    $$ R = a+\beta\_{1} \* factor\_{1}+\beta\_{2} \* factor\_{2}+e$$

    $R$为回报率，$a$为截距即premium，$factor\_{1}$为经济增长意外指数，$factor\_{2}$为通货膨胀意外指数，$\beta\_{1}$和$\beta\_{2}$分别为对两个因素的$\beta$，即敏感度。

2.  资产类别

    先用美国数据作为回测，因此采用美国股票（SPX500）、美国国债（US Treasury index）、美国公司债（US Corporate）、通胀联接债券（Inflation linked）作为资产类别，采用UBS US Growth surprise index 和UBS US Inflation Surprise index作为因子。

3.  beta的稳定性

    根据历史数据计算beta，测试beta的稳定情况。

4.  确定组合构建规则构建组合。

5.  回测组合的回报，计算组合的风险收益指标。