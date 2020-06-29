# [Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

```
def cohen_d(col_one,col_two):
    mean_diff= np.mean(col_one)-np.mean(col_two)
    var_one = np.var(col_one)
    var_two = np.var(col_two)
    n1=len(col_one)
    n2=len(col_two)
    pooled_dev = np.sqrt(((var_one*n1)+(var_two*n2))/(len(col_one)+len(col_two)))
    print(mean_diff/pooled_dev)
    
    
cohen_d(firsts.totalwgt_lb,others.totalwgt_lb)```
