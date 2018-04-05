[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

``` python
import scipy.stats

mu = 178
sigma = 7.7
dist = scipy.stats.norm(loc=mu, scale=sigma)
type(dist)

dist.mean(), dist.std()

dist.cdf(mu-sigma)

# How many people are between 5'10" and 6'1"?
h_510 = dist.cdf(177.8)
h_601 = dist.cdf(185.42)
answer = (h_601 - h_510)*100
print((h_601-h_510)*100)


print("Percent of men who qualify for BMG is %f " % answer)
```
