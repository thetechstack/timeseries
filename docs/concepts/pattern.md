# 趋势性、季节性和周期性

我们通常使用例如“趋势”、“季节性”等词语描述时间序列。在深入研究时间序列模式时，应该更精确的定义这些词语。

## 趋势

当一个时间序列数据长期增长或者长期下降时，表示该序列有 **趋势** （ **Trend** ） 。下图存在一个明显的增长趋势。

<figure markdown>
  ![澳大利亚降糖药物的月销量](https://otexts.com/fppcn/fpp_files/figure-html/a10-1.png){ width="100%" }
  <figcaption>澳大利亚降糖药物的月销量</figcaption>
</figure>

## 季节性

当时间序列中的数据受到季节性因素（例如一年的时间或者一周的时间）的影响时，表示该序列具有 **季节性** （ **Seasonal** ，有时也称为 **Periodic** ） 。
季节性总是一个已知并且 **固定的频率** 。由于抗糖尿病药物的成本在年底时会有变化，导致上图抗糖尿药物的月销售额存在季节性。

## 周期性

当时间序列数据存在不固定频率的上升和下降时，表示该序列有 **周期性**（ **Cyclic** ） 。这些波动经常由经济活动引起，并且与“商业周期”有关。周期波动通常至少持续两年。

许多初学者都不能很好的区分季节性和周期性，然而这两个概念是完全不同的。

- 当数据的波动是无规律时，表示序列存在周期性；
- 如果波动的频率不变并且与固定长度的时间段有关，表示序列存在季节性。一般而言，周期的长度较长，并且周期的波动幅度也更大。

许多时间序列同时包含趋势、季节性以及周期性。当我们选择预测方法时，首先应该分析时间序列数据所具备的特征，然后再选择合适的预测方法抓取特征。

!!! 注意
    不过，在中文语境下，这里说的周期性通常不是指Cyclic，而是Periodic，指季节性。

## 参考链接

- [时间序列模式 - 预测： 方法与实践](https://otexts.com/fppcn/tspatterns.html){target=_blank}
- [Cyclic and seasonal time series - ob J Hyndman](https://robjhyndman.com/hyndsight/cyclicts/){target=_blank}