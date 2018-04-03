[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

```python
from math import sqrt

firsts.totalwgt_lb.mean(), others.totalwgt_lb.mean()

diff = firsts.totalwgt_lb.mean() - others.totalwgt_lb.mean()
firsts_var = firsts.totalwgt_lb.var()
others_var = others.totalwgt_lb.var()
n1, n2 = len(firsts.totalwgt_lb), len(others.totalwgt_lb)
pooled_var = (n1 * firsts_var + n2 * others_var) / (n1 + n2)
Cohen_d = diff / math.sqrt(pooled_var)

print(Cohen_d) 
```

Interpretaion:
Cohen’s d showed that the difference between the first babies mean weight and non-first babies mean weight in stands deviation for the two groups is equal to -0.089 STDs. This indicates that there is a very small difference in weights and that the first babies are lighter. 

Similarly, the difference in pregnancy length also had a very small Cohen’s d of 0.029 STDs. 


