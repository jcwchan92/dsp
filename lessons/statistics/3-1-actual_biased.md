# [Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

```
pmf = thinkstats2.Pmf(resp.numkdhh,label='actual')
biased_pmf = BiasPmf(pmf, label='observed')

```

Create the pmf and biased pmf
```
thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased_pmf])
thinkplot.Config(xlabel='Num KD HH', ylabel='PMF')

print('Actual mean', pmf.Mean())
print('Observed mean', biased_pmf.Mean())
```

Outputs 
```
Actual mean 1.024205155043831
Observed mean 2.403679100664282
```



![Ex 3 chart](/lessons/statistics/Exercise3.png)
