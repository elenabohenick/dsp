[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

``` python
from __future__ import print_function, division

%matplotlib inline

import numpy as np

import nsfg
import thinkstats2
import thinkplot

rand_nums = np.random.random(size = 1000)

pmf = thinkstats2.Pmf(rand_nums)
thinkplot.Hist(pmf, linewidth=0.1)
thinkplot.Config(xlabel = 'Random Variate', ylabel = 'PMF')

cdf = thinkstats2.Cdf(rand_nums)
thinkplot.Cdf(cdf)
thinkplot.Config(xlabel = 'Random Variate', ylabel = 'CDF')
```
