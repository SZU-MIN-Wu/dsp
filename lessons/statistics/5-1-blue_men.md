[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> 34.3%

```
import scipy.stats
mu = 178
sigma = 7.7
dist = scipy.stats.norm(loc=mu, scale=sigma)
def to_cm(ft,inches):
    return ft*30.48+inches*2.54
dist.cdf(to_cm(6,1))-dist.cdf(to_cm(5,10))
```
