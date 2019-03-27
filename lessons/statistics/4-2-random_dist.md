[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>> It is a normal distribution.

```
random_num=numpy.random.random(1000)
cdf = thinkstats2.Cdf(random_num, label='random')
thinkplot.Cdf(cdf)
thinkplot.Config(xlabel='number', ylabel='CDF')
pmf = thinkstats2.Pmf(random_num, label='random')
thinkplot.Pmf(pmf, linewidth=0.1)
thinkplot.Config(xlabel='number', ylabel='PMF')
```
