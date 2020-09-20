[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)
pmf = thinkstats2.Pmf(resp.numkdhh, label='numkdhh')

thinkplot.Pmf(pmf)
thinkplot.Config(xlabel='Number of children', ylabel='PMF')

biased_distribution = BiasPmf(pmf, label='biased distribution')

thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased_distribution])
thinkplot.Config(xlabel='Number of children', ylabel='PMF')

pmf.Mean()

biased_distribution.Mean()
