[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

```
nums = np.random.random(1000)
pmf = thinkstats2.Pmf(nums, label='pmf')
cdf = thinkstats2.Cdf(nums, label='cdf')

thinkplot.Pmf(pmf, linewidth = 0.1)
thinkplot.Config(xlabel='Value', ylabel='PMF')

#thinkplot.Cdf(cdf, linewidth=1)
#thinkplot.Config(xlabel='Value', ylabel='CDF')
```

![Pmf](https://github.com/imoscovitz/dsp/blob/master/statistics/Pmf.png "Pmf") 
![Cdf](https://github.com/imoscovitz/dsp/blob/master/statistics/Cdf.png "Cdf")

Yup! Looks pretty random! The pmf looks like a random distribution, and the cdf looks linnear.
