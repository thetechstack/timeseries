# 自相关

设$\{X_t\}$为一随机过程（姑且视其为随机变量的集合），t是时间上的一个点（对于离散型随机过程，它是整数；对于连续性随机过程，它是实数）。
假设改过程在时刻t的均值为$\mu_t$，方差为$\sigma_t^2$, 则$t_1$和$t_2$的自相关函数( auto-correlation function)定义为：

$$R_{XX}(t_1t_2) = E[X_{t_1}X_{t_2}]$$

!!! 注意
    我们这里只考虑实随机变量。对复随机变量上面的$X_{t_2}$要取共轭。

$t_1$和$t_2$的自协方差函数( auto-covariance function)定义为:

$$K_{XX}(t_1t_2) = E[(X_{t_1}-\mu_{t_1})(X_{t_2}-\mu_{t_2})] = E[X_{t_1}X_{t_2}] - \mu_{t_1}\mu_{t_2}$$


## 对于弱平稳随机过程

对于弱平稳随机过程，$X_t$的均值和方差与时间t无关，且自相关或自协方差函数仅与$t_2$和$t_1$的差（也称为lag，滞后）有关。因此我们可以将
自相关或自协方差表示为滞后$k=t2-t1$的函数。

自相关：

$$R_{XX}(k) = E[X_{t+k}X_t]$$

自协方差：

$$K_{XX}(k) = E[(X_{t+k}-\mu)(X_{t}-\mu)] = E[X_{t+k}X_{t}] - \mu\mu$$

## 标准化

随机过程的 **自相关系数** （auto-correlation coefficient） 定义为

$$\rho_{XX}(t_1t_2) = \frac{K_{XX}(t_1t_2)}{\sigma_{t_1}\sigma_{t_2}} = \frac{E[(X_{t_1}-\mu_{t_1})(X_{t_2}-\mu_{t_2})]}{\sigma_{t_1}\sigma_{t_2}}$$

对于弱平稳过程，有

$$\rho_{XX}(k) = \frac{K_{XX}(k)}{\sigma^2} = \frac{E[(X_{t+k}-\mu)(X_{t}-\mu)]}{\sigma^2}$$

## 计算

对于具体的时间序列$\{y_t, t=1,2,...,T\}$, 自相关系数按一下方式计算：

$$r_{k} = \frac{\sum\limits_{t=k+1}^T (y_{t}-\bar{y})(y_{t-k}-\bar{y})}
 {\sum\limits_{t=1}^T (y_{t}-\bar{y})^2}$$

## 参考链接

- [Autocorrelation - Wikipedia](https://en.wikipedia.org/wiki/Autocorrelation){target=_blank}
- [自相关 - 预测： 方法与实践](https://otexts.com/fppcn/autocorrelation.html){target=_blank}


