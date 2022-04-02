+++
title = "007 Nityanand Misra"

+++
[[Nityanand Misra	2013-12-23, 05:05:56 [Source](https://groups.google.com/g/bvparishat/c/cNoHQNYriks)]]



  

You ask a lot of questions :)  
  
Answers inline.  

  

On Mon, Dec 23, 2013 at 2:13 AM, Mārcis Gasūns \<[gas...@gmail.com]()\> wrote:  

> 
> > 
> > Thanks, but the links and articles do not help. Please explain in > plain > English<https://docs.google.com/document/d/1nDDLsylG6hp6v9Q-gSnQsiJz9sjg0wJbO8_amqAZQZ0/edit#>
> > 
> > 
> >   
> > 
> > 
> > All periods Early & Epic Epic & Classical Classical & Medieval > Medieval & Late >
> Gutturals 0.000000e+00 3.607401e-43 0.000000e+00 > 0.000000e+00 1.267108e-01 >
> Palatals 1.175834e-246 8.720096e-51 1.598550e-161 > 9.514065e-01 2.303646e-02 >
> Retroflexes 0.000000e+00 3.181280e-01 6.859133e-92 > 1.400428e-127 3.685050e-02 >
> Dentals 3.114376e-48 1.022459e-08 6.671614e-07 > 2.707000e-14 3.677069e-34 >
> Labials 0.000000e+00 2.611753e-01 4.399987e-35 > 1.750870e-106 6.592439e-01  
> > 
> > 

  

The above table as output by R uses [scientific notation](http://en.wikipedia.org/wiki/Scientific_notation). So a number like 4.399987e-35 means 4.399987 x 10 raised to -35. Or 4.399987 divided by 1 followed by 35 zeros.  



> 
> > 
> > 
> > 
> > 
> > 1)0.000000e means that there is no change? +00 stands for no > change? + can be only 00? >
> 
> > 

  

These are p-values for the Chi-square test. The smaller the p-value, the more is the evidence against our assumption (Null Hypothesis: No Change). The assumption for the test is no change (null hypothesis assumption is like the assumption in law - innocent until proven guilty). Usually whenever the p-value is smaller than a threshold like 0.05 (5% significance) or 0.01 (1% significance), we reject the null hypothesis (assumption). For a large sample set, one can use even a smaller threshold like 0.001 (0.1% significance).  
  

Under the link below, you can see between which periods we do not have enough evidence for change (numbers in red, all greater than 0.001) -  
<https://groups.google.com/forum/#!msg/samskrita/4oGLpUXyjxI/MV4z0uIoTQcJ>  
  
So 0e+00 means the p-value is infinitesimally small, which means there is enough evidence against the assumption of no change. Which means the conclusion is the ratio has changed.  
  

That's the best I can explain in plan English, to learn more, one needs to understand [Statistical Hypothesis Testing](http://en.wikipedia.org/wiki/Statistical_hypothesis_testing).  



> 
> > 
> > 2) 1.175834e and 9.514065e - 1 is the minimum, 10 - maximum? >
> 
> > 
> > 3) -01 small change? -92 mid change?-161 big change? >
> 
> > 
> > 4) e is for what? >
> 
> > 

  

\(2\) to (3): No, this is scientific notation. (4) E stands for "x 10 raised to".  



> 
> > 
> > 5) how to build a plot with this data? Can we have something more > aesthetic than just > <http://upload.wikimedia.org/wikipedia/commons/thumb/f/f6/Plots_from_lm_example.svg/540px-Plots_from_lm_example.svg.png>? > Does<http://latticeextra.r-forge.r-project.org/#marginal.plot&theme=default>contains > the kind of plot we could use to represent this kind of data? >
> 
> > 
> > 
> >   
> > 
> > 
> > 

  

One can use a heatmap. See [here](http://www.r-bloggers.com/using-heatmaps-to-uncover-the-individual-level-structure-of-brand-perceptions/). Further discussion, I am afraid, is beyond the scope of a mailgroup discussion.  



> 
> > 
> > It's FAR too specific :)
> > 
> > 
> > A video series like<http://www.youtube.com/watch?v=o0Y478jOjGk>is > what can help.
> > 
> > 
> > Not those smart articles even a mathematician would read with > toothache, really. >
> 
> > 
> > 
> > 
> > 
> > 
> > 

  

I currently do not have time or motivation for making YouTube videos. Will do when I have the leisure.  



> 
> > 

> 
> > 
> > > 
> > > > 
> > > > What do you mean by "open syllable"?  
> > > > 
> > > > 
> > 
> > 
> > The same as everybody > else,<http://www.allaboutlearningpress.com/how-to-teach-closed-and-open-syllables>
> > 
> > 

> 
> > 
> > 
> > Open Syllables >
> 
> > 
> >   
> > 
> > 
> > In an open syllable, nothing comes after the vowel. Look at the word > he. We say that the vowel is open. There is nothing closing it in. >
> 
> > 
> >   
> > 
> >   
> > 
> > 

> 
> > 
> > 
> > Do you notice that in each of the open syllables, the vowel is long > (says its name)? >
> 
> > 
> > 

> 
> > 
> > > 
> > > > 
> > > > What is meant by "closed syllable"?  
> > 
> > > > 
> > > > 
> > 
> > 
> > 
> > Closed Syllables >
> 
> > 
> >   
> > 
> > 
> > In a closed syllable, the vowel is followed by a consonant. Explain to > your students that the vowel is “closed in” by the consonant. Take a > look at these words: >
> 
> > 
> >   
> > 
> > 
> > 
> > 
> > 

> 
> > 

  

Ah I see. Then you may want to use the below. I get 5.4% closed syllables, 84.8% open syllables, 6.1% syllables with Anusvaara and 3.6% syllables with Visarga.  
  

# Closed syllables - end in a consonant

sum( data\[grep( "C$", data$Syllable2 ),\]$total )

\[1\] 406054

# Pure open syllables - end in a vowel

sum( data\[grep( "V$", data$Syllable2 ),\]$total )

\[1\] 6404405

# Semi-open syllables - end in a vowel + Anusvaara

sum( data\[grep( "VM$", data$Syllable2 ),\]$total )

\[1\] 461717

# Semi-open syllables - end in a vowel + Visarga

sum( data\[grep( "VH$", data$Syllable2 ),\]$total )

\[1\] 277554

# Do they add up?

406054 + 6404405 + 461717 + 277554

\[1\] 7549730

sum( data$total )

\[1\] 7566142

# Not quite! That's because there are some bad values still there

# Let's find them out

unique( data$Syllable2 )

\[1\] "V" "CV" "CVH" "CCV" "CVC" "CVM" "CCVC"
"CCVH" **NA** "CCVM" "CCCV" "CCCCV" "CCCVH" "CCCVC"
"CCCVM" "CCCCVC" "VM" "VC"

\[19\] "VH" "CCCCVM" "CVV" "CCCCVH" "MCV" "CCCCCV" "MCVH"
"MCVC" "HCV" "CCMCV" "CCHVH" "CMV" "CCVV" "CCHV" "MCVM"
"CMCV" "VV" "HCVH"

# Ah, see the "NA" there - some missing values

# Let's see the rows with these missing values

data\[[is.na](http://is.na)(data$Syllable2),\]

 Syllable early epic classical medieval late total Syllable2

74 \<NA> 661 6231 4873 2866 1781 16412 \<NA>

# Hmm, is that 16412 the missing number from the total?

# Let's check

406054 + 6404405 + 461717 + 277554 + 16412

\[1\] 7566142

sum( data$total )

\[1\] 7566142

# Yes, perfect match, so let's throw the row out

data \<- data\[![is.na](http://is.na)( data$Syllable2 ),\]

sum( data$total )

\[1\] 7549730

# This is same as before

# Now do the percentages

# Percentage of closed syllables - end in a consonant

sum( data\[grep( "C$", data$Syllable2 ),\]$total ) / 7549730

\[1\] 0.05378391

# Percentage of pure open syllables - end in a vowel

sum( data\[grep( "V$", data$Syllable2 ),\]$total ) / 7549730

\[1\] 0.8482959

# Percentage of semi-open syllables - end in a vowel + Anusvaara

sum( data\[grep( "VM$", data$Syllable2 ),\]$total ) / 7549730

\[1\] 0.06115676

# Percentage of semi-open syllables - end in a vowel + Visarga

sum( data\[grep( "VH$", data$Syllable2 ),\]$total ) / 7549730

\[1\] 0.03676343



  
  
  



  

