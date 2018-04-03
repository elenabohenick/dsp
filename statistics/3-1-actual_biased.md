[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

``` python

from __future__ import print_function, division

%matplotlib inline

import numpy as np

import nsfg
import first
import thinkstats2
import thinkplot

resp = nsfg.ReadFemResp()

pmf = thinkstats2.Pmf(resp.numkdhh, label = 'numkdhh')
thinkplot.Hist(pmf)
thinkplot.Config(xlabel = 'num of children', ylabel = 'PMF')

biased = BiasPmf(pmf, label = 'biased')

pmf = thinkstats2.Pmf(resp.numkdhh, label = 'numkdhh')

biased = BiasPmf(pmf, label = 'biased')

thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased])
thinkplot.Config(xlabel = 'number of children', ylabel = 'PMF')

print(pmf.Mean(), biased.Mean())
