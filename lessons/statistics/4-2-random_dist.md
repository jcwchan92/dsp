# [Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)
```
thinkplot.PrePlot(2)

random_array = np.random.random(1000)
random_pmf = thinkstats2.Pmf(random_array, label='random')

thinkplot.hist(random_pmf,width=.2)

```

![ex4pic1](/lessons/statistics/ex4pic1.png)

This shows a uniform distribution. 

```
cdf = thinkstats2.Cdf(random_array, label='random')

thinkplot.Cdf(cdf)


![ex4pic1](/lessons/statistics/ex4pic2.png)

