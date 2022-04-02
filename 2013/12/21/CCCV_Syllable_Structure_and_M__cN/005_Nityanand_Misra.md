+++
title = "005 Nityanand Misra"

+++
[[Nityanand Misra	2013-12-22, 14:53:01 [Source](https://groups.google.com/g/bvparishat/c/cNoHQNYriks)]]



  
  
On Sunday, December 22, 2013 12:17:27 AM UTC+8, Mārcis Gasūns wrote:

> 
> >   
>   
> On Saturday, 21 December 2013 16:19:57 UTC+4, Nityanand Misra wrote: >
> > 
> > > > 
> > > > 
> > > > 
> > > > > 
> > > > > > 
> > > > > > Is the "five-sample Chi-square test" code available for download, > > > Nityanand, the prop.test() one? <http://ideone.com/XKVHTM> seems > > > to be your testing of it lately. > > > > > > 
> > > > > > 
> > > > 
> > > >   
> > > > 
> > > > 
> > > > I have lost it. I had it on my old machine. I can write it again, it > > is simple. But why do you need it? You would not find it useful > > unless you want to statistically test for stability of proportion of > > a certain set of syllables across different periods.  
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > 
> > I would want to see the difference of output. >
> 
> > 
> > 
> > 

  
See attached - it is a plaint text file with R code. No copyright or copyleft, use as you like and you are not obliged to credit me.  
  
For theory on the test, you may refer the following references (from the help page [here](http://stat.ethz.ch/R-manual/R-patched/library/stats/html/prop.test.html))  
  

Wilson, E.B. (1927) Probable inference, the law of succession, and statistical inference. *J. Am. Stat. Assoc.*, **22**, 209–212.

Newcombe R.G. (1998) Two-Sided Confidence Intervals for the Single Proportion: Comparison of Seven Methods. *Statistics in Medicine* **17**, 857–872.

Newcombe R.G. (1998) Interval Estimation for the Difference Between Independent Proportions: Comparison of Eleven Methods. *Statistics in Medicine* **17**, 873–890.  



> 
> >   
> > 
> > Thanks, some great hints. What I wonder is >
> 
> > 
> > 
> > -   Number of open syllables?  
> > 
> > 
> > 

  
What do you mean by "open syllable"?  

> 
> > 
> > 
> > -   
> > 
> > 
> > sum( data\[grep( "^V$", data$Syllable2 ),\]$total ) >
> 
> > 
> > \[1\] 255956 >
> 
> > 
> >   
> > 
> > 
> > -   Number of closed syllables?  
> > 
> > 
> > 

What is meant by "closed syllable"?  


> 
> > 
> > 
> > -   
> > 
> > 
> > sum( data\[grep( "^C$", data$Syllable2 ),\]$total ) >
> 
> > 
> > \[1\] 0 >
> 
> > 
> > 
> > Why 0? >
> 
> > 
> > 
> > 
> > 

  
Single consonant is not a syllable in Samskrita, and not a syllable in Hellwig's data.  
  

  

