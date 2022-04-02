+++
title = "008 Mārcis Gasūns"

+++
[[Mārcis Gasūns	2013-12-24, 23:32:33 [Source](https://groups.google.com/g/bvparishat/c/cNoHQNYriks)]]



Namaste,

  
  
On Monday, 23 December 2013 03:35:56 UTC+4, Nityanand Misra wrote:

> 
> > 
> > You ask a lot of questions :)  
> > 
> > 

Oh no, only the bare minimum. The topic is such that has never been actually explored before Oliver. Not in such detail. What I miss in his data is the metadata if the syllable comes from word beginning or end. That would make even more calculations possible. I'll make such data open for my data at<https://github.com/gasyoun/nagari>as soon as I manage to split Sanskrit syllables correctly.



> 
> > 
> > Answers inline.  
> > 
> > 

Thanks.



> 
> > 
> > 
> > 
> >   
> > 
> > On Mon, Dec 23, 2013 at 2:13 AM, Mārcis Gasūns \<gas...@gmail.com\> > wrote:  
> > > 
> > > > 
> > > > Thanks, but the links and articles do not help. Please explain in > > plain > > English<https://docs.google.com/document/d/1nDDLsylG6hp6v9Q-gSnQsiJz9sjg0wJbO8_amqAZQZ0/edit#>
> > > > 
> > > > 
> > > >   
> > > > 
> > > > 
> > > > All periods Early & Epic Epic & Classical Classical & Medieval > > Medieval & Late > > > > Gutturals 0.000000e+00 3.607401e-43 0.000000e+00 > > 0.000000e+00 1.267108e-01 > > > > Palatals 1.175834e-246 8.720096e-51 1.598550e-161 > > 9.514065e-01 2.303646e-02 > > > > Retroflexes 0.000000e+00 3.181280e-01 6.859133e-92 > > 1.400428e-127 3.685050e-02 > > > > Dentals 3.114376e-48 1.022459e-08 6.671614e-07 > > 2.707000e-14 3.677069e-34 > > > > Labials 0.000000e+00 2.611753e-01 4.399987e-35 > > 1.750870e-106 6.592439e-01  
> > > > 
> > > > 
> > 
> >   
> > 
> > 
> > The above table as output by R uses [scientific > notation](http://en.wikipedia.org/wiki/Scientific_notation). So a > number like 4.399987e-35 means 4.399987 x 10 raised to -35. Or > 4.399987 divided by 1 followed by 35 zeros.  
> > 
> > 
> > 
> > 

Ah, oh, ok. Is there a way to make it easier to read? I mean how do I actually make the plot, what is the R code to make plots out of it?



> 
> > 
> > 
> > 
> > 
> > 
> > 
> > 
> > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 1)0.000000e means that there is no change? +00 stands for no > > change? + can be only 00? > > > > 
> > > > 
> > 
> >   
> > 
> > 
> > These are p-values for the Chi-square test. The smaller the p-value, > the more is the evidence against our assumption (Null Hypothesis: No > Change). The assumption for the test is no change (null hypothesis > assumption is like the assumption in law - innocent until proven > guilty). >
> 
> > 
> > 
> > 

null hypothesis assumption - ok, this I've understood. But can we change the starting point? Can we take the maximum value as 100% and everything else less, compared to it?  



> 
> > 
> > 
> > 
> > Usually whenever the p-value is smaller than a threshold like 0.05 (5% > significance) or 0.01 (1% significance), we reject the null hypothesis > (assumption). For a large sample set, one can use even a smaller > threshold like 0.001 (0.1% significance).  
> > 
> > 
> > 
> > 

In our case which cells are smaller as the large sample set treshold? Our's is large, is it not?



> 
> > 
> > 
> > 
> > Under the link below, you can see between which periods we do not have > enough evidence for change (numbers in red, all greater than 0.001) > -  
> <https://groups.google.com/forum/#!msg/samskrita/4oGLpUXyjxI/MV4z0uIoTQcJ>  
>   
> So 0e+00 means the p-value is infinitesimally small, which means there > is enough evidence against the assumption of no change. Which means > the conclusion is the ratio has changed.  
> > 
> > 
> > 
> > 

So no change, no interest for us, right?



> 
> > 
> > 
> > 
> > That's the best I can explain in plan English, to learn more, one > needs to understand [Statistical Hypothesis > Testing](http://en.wikipedia.org/wiki/Statistical_hypothesis_testing).  
> > 
> > 
> > 
> > 

Oh, it's getting bad, but anyway it's much clearer now, thanks you so much.



> 
> > 
> > 
> > 
> > 
> > 
> > 
> > 
> > > 
> > > > 
> > > > 2) 1.175834e and 9.514065e - 1 is the minimum, 10 - maximum? > > > > 
> > > > 
> > > > 3) -01 small change? -92 mid change?-161 big change? > > > > 
> > > > 
> > > > 4) e is for what? > > > > 
> > > > 
> > 
> >   
> > 
> > 
> > \(2\) to (3): No, this is scientific notation. (4) E stands for "x 10 > raised to".  
> > 
> > 
> > 
> > 
> > > 
> > > > 
> > > > 5) how to build a plot with this data? Can we have something more > > aesthetic than just > > <http://upload.wikimedia.org/wikipedia/commons/thumb/f/f6/Plots_from_lm_example.svg/540px-Plots_from_lm_example.svg.png>? > > Does<http://latticeextra.r-forge.r-project.org/#marginal.plot&theme=default>contains > > the kind of plot we could use to represent this kind of data? > > > > 
> > > > 
> > > > 
> > > >   
> > > > 
> > > > 
> > > > 
> > 
> >   
> > 
> > 
> > One can use a heatmap. See > [here](http://www.r-bloggers.com/using-heatmaps-to-uncover-the-individual-level-structure-of-brand-perceptions/). > Further discussion, I am afraid, is beyond the scope of a mailgroup > discussion.  
> > 
> > 
> > 
> > 

Sure, can you please copy the code here? Or we can move to<https://groups.google.com/forum/#!forum/sanskrit-programmers> ? Never seen you there actually.



> 
> > 
> > 
> > I currently do not have time or motivation for making YouTube videos. > Will do when I have the leisure.  
> > 
> > 
> > 

Thanks indeed.



> 
> > 
> > 
> > Ah I see. Then you may want to use the below. I get 5.4% closed > syllables, 84.8% open syllables, 6.1% syllables with Anusvaara and > 3.6% syllables with Visarga.  
> > 
> > 
> > 

Yes, perfect. Only issue 3.6 should be 3.7, otherwise the total sum of all numbers is not 100.



Thanks for the code. Why is not possible to get numbers and % with same single line of code? Strange :)

  

M.G.

