# [Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

```min_height_cm = (5*(12)*(2.54))+(10*2.54)
max_height_cm  = (6*(12)*(2.54))+(1*2.54)

z_min = (min_height_cm-mu)/(dist.std())
z_max = (max_height_cm-mu)/(dist.std())
```
```
print(dist.cdf(mu+(z_min*sigma)))
print(dist.cdf(mu+(z_max*sigma)))
print(dist.cdf(mu+(z_max*sigma))-dist.cdf(mu+(z_min*sigma)))
```
Returns:
Percent lower than 5 10: 0.48963902786483265
Percent lower than 6 : 1.8323858654963063
Difference: 0.3427468376314737
