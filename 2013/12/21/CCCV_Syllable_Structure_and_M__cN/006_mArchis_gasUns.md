+++
title = "006 Mārcis Gasūns"

+++
[[Mārcis Gasūns	2013-12-22, 23:43:24 [Source](https://groups.google.com/g/bvparishat/c/cNoHQNYriks)]]



  
  
On Sunday, 22 December 2013 13:23:01 UTC+4, Nityanand Misra wrote:

> 
> > > 
> > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > I have lost it. I had it on my old machine. I can write it again, > > > it is simple. But why do you need it? You would not find it useful > > > unless you want to statistically test for stability of proportion > > > of a certain set of syllables across different periods.  
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > 
> > > > I would want to see the difference of output. > > > > 
> > > > 
> > > > 
> > > > 
> > 
> >   
> See attached - it is a plaint text file with R code. No copyright or > copyleft, use as you like and you are not obliged to credit me.  
> > 
> > 

Thanks, but the links and articles do not help. Please explain in plain English<https://docs.google.com/document/d/1nDDLsylG6hp6v9Q-gSnQsiJz9sjg0wJbO8_amqAZQZ0/edit#>

  

All periods Early & Epic Epic & Classical Classical & Medieval Medieval & Late

Gutturals 0.000000e+00 3.607401e-43 0.000000e+00
0.000000e+00 1.267108e-01

Palatals 1.175834e-246 8.720096e-51 1.598550e-161
9.514065e-01 2.303646e-02

Retroflexes 0.000000e+00 3.181280e-01 6.859133e-92
1.400428e-127 3.685050e-02

Dentals 3.114376e-48 1.022459e-08 6.671614e-07
2.707000e-14 3.677069e-34

Labials 0.000000e+00 2.611753e-01 4.399987e-35
1.750870e-106 6.592439e-01  



1)0.000000e means that there is no change? +00 stands for no change? + can be only 00?

2) 1.175834e and 9.514065e - 1 is the minimum, 10 - maximum?

3) -01 small change? -92 mid change?-161 big change?

4) e is for what?

5) how to build a plot with this data? Can we have something more aesthetic than just <http://upload.wikimedia.org/wikipedia/commons/thumb/f/f6/Plots_from_lm_example.svg/540px-Plots_from_lm_example.svg.png>? Does<http://latticeextra.r-forge.r-project.org/#marginal.plot&theme=default>contains the kind of plot we could use to represent this kind of data?

  

> 
> > 
> >   
> For theory on the test, you may refer the following references (from > the help page > [here](http://stat.ethz.ch/R-manual/R-patched/library/stats/html/prop.test.html))  
>   
> > Wilson, E.B. (1927) Probable inference, the law of succession, and > statistical inference. *J. Am. Stat. Assoc.*, **22**, 209–212. >
> Newcombe R.G. (1998) Two-Sided Confidence Intervals for the Single > Proportion: Comparison of Seven Methods. *Statistics in Medicine* > **17**, 857–872. >
> Newcombe R.G. (1998) Interval Estimation for the Difference Between > Independent Proportions: Comparison of Eleven Methods. *Statistics in > Medicine* **17**, 873–890.  
> > 
> > 

It's FAR too specific :)

A video series like<http://www.youtube.com/watch?v=o0Y478jOjGk>is what can help.

Not those smart articles even a mathematician would read with toothache, really.



> 
> > 
> > What do you mean by "open syllable"?  
> > 
> > 

The same as everybody else,<http://www.allaboutlearningpress.com/how-to-teach-closed-and-open-syllables>

Open Syllables

  

In an open syllable, nothing comes after the vowel. Look at the word he. We say that the vowel is open. There is nothing closing it in.

  

For other examples, look at the first syllables in these words:

  

ba by

e ven

pa per

a ble

  

Do you notice that in each of the open syllables, the vowel is long (says its name)?

> 
> > 
> > What is meant by "closed syllable"?  
> 
> > 
> > 

Closed Syllables

  

In a closed syllable, the vowel is followed by a consonant. Explain to your students that the vowel is “closed in” by the consonant. Take a look at these words:

  

cap

sit

men

  

Do you notice that in each of the closed syllables, the vowel is short?



> 
> > 
> > Single consonant is not a syllable in Samskrita, and not a syllable in > Hellwig's data.  
> > 
> > 

I know. Still every syllable is open or closed. So I need to know what is the end of each syllable. Is it V or C? Whatever is before it. Even if nothing. Very interesting topic, too bad that R is not as easy as perl or php, it takes time to understand even the basic issues. Can it extract samples as well, or only count?

  

M.G.

