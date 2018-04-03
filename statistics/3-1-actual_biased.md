[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

The code below computes biased distribution that we would get if we surveyed the childred and asked how many children uder 18 years old live in the household. Biased mean of the number of childer in the household will be higher than the actual mean.

The code also computes an actual distribution and its mean and puts them on one graph for comparison.


``` python

%matplotlib inline

import nsfg
import thinkstats2
import thinkplot

def BiasPmf(pmf, label):
    new_pmf = pmf.Copy(label=label)

    for x, p in pmf.Items():
        new_pmf.Mult(x, x)
        
    new_pmf.Normalize()
    return new_pmf

resp = nsfg.ReadFemResp()

pmf = thinkstats2.Pmf(resp.numkdhh, label = 'numkdhh')
biased = BiasPmf(pmf, label = 'biased')

thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased])
thinkplot.Config(xlabel = 'number of children', ylabel = 'PMF')

print(pmf.Mean(), biased.Mean())
```
