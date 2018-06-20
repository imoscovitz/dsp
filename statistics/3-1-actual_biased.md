[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

```
resp = nsfg.ReadFemResp()
numkdhh = thinkstats2.Pmf(resp.numkdhh, 'actual')
biased_numkdhh = BiasPmf(numkdhh, 'biased')

thinkplot.PrePlot(2)
thinkplot.Pmfs([numkdhh, biased_numkdhh])
thinkplot.Config(xlabel='NumChildren', ylabel='PMF')

print('Actual mean', numkdhh.Mean())
print('Biased mean', biased_numkdhh.Mean())
```

![actual_biased](https://github.com/imoscovitz/dsp/blob/master/statistics/actualbiased.png) 

Actual mean: 1.024    
Biased mean: 2.403
