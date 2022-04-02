+++
title = "006 Nityanand Misra"

+++
[[Nityanand Misra	2016-01-29, 08:58:07 [Source](https://groups.google.com/g/bvparishat/c/HPdtmEvjJ0c)]]



  
  
On Wednesday, 27 January 2016 14:41:00 UTC+5:30, nagarajpaturi wrote:

> 
> > 
> > The researchers in this article used four language families as one of > the category of variables. Mr Suresh Kolichala who is on this list, is > adding one more language category 'nishaada'. We may expect 'more > robust' genome analysis in future when such new categories are added. >
> 
> > 
> > 
> > 
> > 
> > The present study does not seem to have taken into > accountthesocially institutionalized matrilinealinter-caste 'gene > mixing'(?) (as in Kerala and the north-east ). 
> > 
> > 
> > 
> > 

  

I am still reading the paper and trying to completely understand the methods used for the analysis. I am comfortable with Principal Component Analysis and have worked in R. I may write to the authors to see if it is possible for them to share the R code and raw data used for the analysis (not sure how big the raw dataset is though). I do not claim to completely understand the ADMIXTURE algorithm (the paper describing it is [here](http://genome.cshlp.org/content/early/2009/07/31/gr.094052.109.full.pdf)), however I can confidently assert from my reading of the paper and results so far that language family is ***not*** used as a variable or a category of variable in the ADMIXTURE analysis. Language family isonlyshown as a part of summary statistics of the populations surveyed in Exhibit 1. Therefore, adding a new category of language will not have any impact on the ADMIXTURE study. Furthermore, it is to be noted that even the population labels are not used as a variable in their modeling. The authors emphasize multiple times in the paper (under [here](http://www.pnas.org/content/early/2016/01/20/1513197113.full.pdf)) as well as in the supplement (under [here](http://www.pnas.org/content/suppl/2016/01/20/1513197113.DCSupplemental/pnas.1513197113.sapp.pdf)) that:

  

*“Population labels were added only after each individual’s ancestry had been estimated; they were used to order the samples in plotting.”*

  

Therefore, a criticism based on argument of questionable labels is also unfounded as the labels are not used as a factor in the model.

  

We need a full and correct understanding of the method used by the authors before critiquing it. At least the approach of the authors is transparent and well-documented.





