[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

### Excercise 5.1
In the BRFSS (see Section 5.4), the distribution of heights is roughly normal with parameters μ = 178 cm and σ = 7.7 cm for men, and μ = 163 cm and σ = 7.3 cm for women.
In order to join Blue Man Group, you have to be male between 5’10” and 6’1” (see http://bluemancasting.com). What percentage of the U.S. male population is in this range? Hint: use scipy.stats.norm.cdf.


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
