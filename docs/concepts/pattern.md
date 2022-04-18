# 趋势性、季节性和周期性

我们通常使用例如“趋势”、“季节性”等词语描述时间序列。在深入研究时间序列模式时，应该更精确的定义这些词语。

## 趋势

当一个时间序列数据长期增长或者长期下降时，表示该序列有 **趋势（Trend）** 。下图存在一个明显的增长趋势。

<figure markdown>
  ![澳大利亚降糖药物的月销量](https://otexts.com/fppcn/fpp_files/figure-html/a10-1.png){ width="100%" }
  <figcaption>澳大利亚降糖药物的月销量</figcaption>
</figure>

## 季节性

当时间序列中的数据受到季节性因素（例如一年的时间或者一周的时间）的影响时，表示该序列具有 **季节性** （ **Seasonal** ，有时也称为 **Periodic** ） 。
季节性总是一个已知并且 **固定的频率** 。由于抗糖尿病药物的成本在年底时会有变化，导致上图抗糖尿药物的月销售额存在季节性。

## 周期性

当时间序列数据存在不固定频率的上升和下降时，表示该序列有 **周期性（Cyclic） ** 。这些波动经常由经济活动引起，并且与“商业周期”有关。周期波动通常至少持续两年。


## 参考链接

- [时间序列模式 - 预测： 方法与实践](https://otexts.com/fppcn/tspatterns.html){target=_blank}
- [Cyclic and seasonal time series - ob J Hyndman](https://robjhyndman.com/hyndsight/cyclicts/){target=_blank}