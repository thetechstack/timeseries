# 时间序列分解概述

我们通常会把时间序列分解成三个成分: 季节项$S_t$（ seasonal component）、趋势-周期项$T_t$（ trend-cycle component）和残差项
$R_t$ （ remainder component）。

!!! 注意
    这里的趋势-周期项中周期是指Cyclic而不是Periodic，参阅[周期性 - 基本概念](/timeseries/concepts/pattern/#_4)
    
有两种分解模型, 一种是加法模型:

$$y_{t} = S_{t} + T_{t} + R_t$$

另一种是乘法模型：

$$y_{t} = S_{t} \times T_{t} \times R_t$$

如果季节性波动的幅度或者趋势周期项的波动不随时间序列水平（level）的变化而变化，那么加法模型是最为合适的。当季节项或趋势周期项的变化与时间序列的水平成比例时，则乘法模型更为合适。在经济时间序列中，乘法模型较为常用。


## 参考链接

- [时间序列成分 - 预测： 方法与实践](https://otexts.com/fppcn/components.html){target=_blank}