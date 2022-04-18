# 预测的统计学观点

!!! 说明
    本文概括自[预测： 方法与实践](https://otexts.com/fppcn/perspective.html#){target=_blank}

我们试图预测的东西是未知的(或者我们不能预测它)，所以我们可以把它想象成一个 **随机变量** 。例如，下个月的总销售额可能会有一系列的可能值，直到月底我们把实际销售额加起来，我们才知道这个值会是多少。所以在我们知道下个月的销售情况之前，这是一个随机的变量。

我们进行预测的过程实际是寻找随机变量可能取值范围内的中间值。通常情况下，预测会伴随着一个 **预测区间** ，给出一个随机变量具有较高概率的范围值。例如，95%的预测区间包含一系列的值，这个预测区间包含实际未来值的概率为95%。

下面的图表显示了未来澳大利亚国际游客的80%和95%的预测区间。蓝线是可能的预测值的平均值，我们称之为“ **点预测** ”。

<figure markdown>
  ![澳大利亚的国际游客总数](https://otexts.com/fppcn/fpp_files/figure-html/austa2-1.png){ width="100%" }
  <figcaption>1980年到2015年澳大利亚的国际游客总数及对其未来10年的预测值和80%和90%预测区间。</figcaption>
</figure>

使用下标$t$作为时间, $y_t$表示在时间$t$的观察值。假设将观察到的所有信息表示为${\cal I}$，
目标是预测$y_t$。此时，$y_{t} | {\cal I}$表示“给定已知${\cal I}$情况下的随机变量$y_t$”，这个随机变量的取值的
概率测度称为$y_{t} |{\cal I}$的 "**概率分布** “，在预测种，我们称之为” **预测分布** “

每当我们谈到“预测”时，通常指的是预测分布的平均值，用$\hat{y}_t$来表示$y_t$的预测值。

明确指出我们在进行预测时使用的信息是很必要的。例如，我们使用$\hat{y}_{t|t-1}$表示表示在已知观测值
$(y_1,\dots,y_{t-1})$的情况下$y_t$的预测值。类似地，我们使用$\hat{y}_{T+h|T}$表示在已知观测值
$y_1,\dots,y_T$ 的情况下$y_{T+h}$的预测值（即考虑时间$T$之前所有观测值的$h$步预测）。