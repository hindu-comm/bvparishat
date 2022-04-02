+++
title = "009 Nityanand Misra"

+++
[[Nityanand Misra	2013-12-25, 14:10:38 [Source](https://groups.google.com/g/bvparishat/c/cNoHQNYriks)]]



  
  
On Wednesday, December 25, 2013 2:02:33 AM UTC+8, Mārcis Gasūns wrote:

> 
> > > 
> > > > 
> > > > 
> > > >   
> > > > 
> > > > The above table as output by R uses [scientific > > notation](http://en.wikipedia.org/wiki/Scientific_notation). So a > > number like 4.399987e-35 means 4.399987 x 10 raised to -35. Or > > 4.399987 divided by 1 followed by 35 zeros.  
> > > > 
> > > > 
> > > > 
> > > > 
> > 
> > Ah, oh, ok. Is there a way to make it easier to read? I mean how do I > actually make the plot, what is the R code to make plots out of it? >
> 
> > 
> > 
> > 
> > 

  
You can find most answers on Google.  
  
<http://stackoverflow.com/questions/5352099/how-to-disable-scientific-notation-in-r>  
<http://flowingdata.com/2010/01/21/how-to-make-a-heatmap-a-quick-and-easy-solution/>  


> 
> > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > >   
> > > > 
> > > > These are p-values for the Chi-square test. The smaller the p-value, > > the more is the evidence against our assumption (Null Hypothesis: No > > Change). The assumption for the test is no change (null hypothesis > > assumption is like the assumption in law - innocent until proven > > guilty). > > > > 
> > > > 
> > > > 
> > > > 
> > 
> > null hypothesis assumption - ok, this I've understood. But can we > change the starting point? Can we take the maximum value as 100% and > everything else less, compared to it?  
> > 
> > 
> > 
> > 
> > 

  
You can if you like, but I would not recommend. A scaled p-value is no good. A p-value is understood and used as is in Statistics.   
  

> 
> > > 
> > > > 
> > > > 
> > > > 
> > > > Usually whenever the p-value is smaller than a threshold like 0.05 > > (5% significance) or 0.01 (1% significance), we reject the null > > hypothesis (assumption). For a large sample set, one can use even a > > smaller threshold like 0.001 (0.1% significance).  
> > > > 
> > > > 
> > > > 
> > > > 
> > 
> > In our case which cells are smaller as the large sample set treshold? > Our's is large, is it not? >
> 
> > 
> > 
> > 

  
You can find out on your own. Try "nrow" function with "ddply" in R.  


> 
> > 
> > 
> > 
> > > 
> > > > 
> > > > 
> > > > 
> > > > Under the link below, you can see between which periods we do not > > have enough evidence for change (numbers in red, all greater than > > 0.001) -  
> > <https://groups.google.com/forum/#!msg/samskrita/4oGLpUXyjxI/MV4z0uIoTQcJ>  
> >   
> > So 0e+00 means the p-value is infinitesimally small, which means > > there is enough evidence against the assumption of no change. Which > > means the conclusion is the ratio has changed.  
> > > > 
> > > > 
> > > > 
> > > > 
> > 
> > So no change, no interest for us, right? >
> 
> > 
> > 
> > 

  
Weight of evidence (or p-value) against the null hypothesis aids in reaching a conclusion. Whether conclusion A is more interesting than conclusion B is a completely subjective matter.  


> 
> > > 
> > > > 
> > > > 
> > > >   
> > > > 
> > > >   
> > > > 
> > > > 
> > > > One can use a heatmap. See > > [here](http://www.r-bloggers.com/using-heatmaps-to-uncover-the-individual-level-structure-of-brand-perceptions/). > > Further discussion, I am afraid, is beyond the scope of a mailgroup > > discussion.  
> > > > 
> > > > 
> > > > 
> > > > 
> > 
> > Sure, can you please copy the code here? Or we can move > to<https://groups.google.com/forum/#!forum/sanskrit-programmers> ? > Never seen you there actually. >
> 
> > 
> > 
> > 

  
I currently do not have the time for this. Will come back after some weeks when I am freer.  


> 
> > 
> > > 
> > > > 
> > > > 
> > > > Ah I see. Then you may want to use the below. I get 5.4% closed > > syllables, 84.8% open syllables, 6.1% syllables with Anusvaara and > > 3.6% syllables with Visarga.  
> > > > 
> > > > 
> > > > 
> > 
> > Yes, perfect. Only issue 3.6 should be 3.7, otherwise the total sum of > all numbers is not 100.
> > 
> > 
> > 
> > 

  
Yes, I truncated rather than rounding. But you get the sense.  


> 
> >   
> > 
> > Thanks for the code. Why is not possible to get numbers and % with > same single line of code? Strange :) >
> 
> > 
> >   
> > 
> > 

  
Very much possible. R-tists can do anything in R! There are people who make high frequency electronic markets on stock exchanges running massive installations of R in parallel.  
  
I had shown them separately for better understanding. Try the "c" function (concatenate in R). Or "ddply" with "nrow" and then add another column which divides by sum.  


> 
> > 
> > 
> > 
> > M.G. >
> 
> > 

  


