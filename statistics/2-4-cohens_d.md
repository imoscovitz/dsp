[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

```
firsts['totalwgt_lb'].mean(), others['totalwgt_lb'].mean()
```
(7.201094430437772, 7.325855614973262)

First babies' mean weight is 7.20 lbs; others' is 7.32. 

FWIW, there are some likely record errors in the outliers. 
```
thinkstats2.Hist(live['totalwgt_lb']).Smallest(10)
```
[(0.125, 1),
 (0.3125, 1),
 (0.4375, 1),
 (0.5625, 1),
 (0.625, 2),
 (0.9375, 1),
 (1.0, 1),
 (1.0625, 3),
 (1.125, 2),
 (1.1875, 1)] 
 
Four of the values came in lower than the world record for the lowest birth weight for a living baby (0.57 lbs): http://www.guinnessworldrecords.com/world-records/lightest-birth 

```
CohenEffectSize(firsts['totalwgt_lb'], others['totalwgt_lb'])
```
-0.088672927072602006 
 
Cohen's d-score is -0.088. It's larger in magnitude than the d-score for pregnancy length, and it's negative instead of positive, though the effect still doesn't seem very large. So others' pregnancy lengths were ever-so-slightly longer than first-births, whereas first-births weighed slightly less than did others.


