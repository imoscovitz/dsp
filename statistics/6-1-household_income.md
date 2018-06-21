[Think Stats Chapter 6 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2007.html#toc60) (household income)

```
Median(sample), Mean(sample), Skewness(sample), PearsonMedianSkewness(sample)
```
(51226.45447894046, 74278.70753118733, 4.949920244429583, 0.7361258019141782)
```
cdf.Prob(74278)
```
0.660005879566872
```
log_sample2 = InterpolateSample(income_df, log_upper=7.0)
sample2 = np.power(10, log_sample2)
Skewness(sample2), PearsonMedianSkewness(sample2)
```
(11.603690267537793, 0.39156450927742087) 
Skewness more than doubled, and Pearson fell. It makes sense that skewness would rise, though it seems a little counterintuitive than Pearson would fall. Unsure whether or not I messed something up, or whether it might have something to do with raising the upper range but only having sample values up to the old upper.
