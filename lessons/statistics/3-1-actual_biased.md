[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>> Means={"actual":1.024, "biased":2.404}

 ```
resp = nsfg.ReadFemResp()
pmf = thinkstats2.Pmf(resp.numkdhh, label='actual')
thinkplot.Pmf(pmf)
thinkplot.Config(xlabel='number_of_kids', ylabel='PMF')
biased_pmf = BiasPmf(pmf, label='observed')
thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased_pmf])
thinkplot.Config(xlabel='number_of_kids', ylabel='PMF')
print(pmf.Mean(),biased_pmf.Mean())

```
