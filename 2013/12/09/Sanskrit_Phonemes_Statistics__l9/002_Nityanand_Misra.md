+++
title = "002 Nityanand Misra"

+++
[[Nityanand Misra	2013-12-13, 13:26:06 [Source](https://groups.google.com/g/bvparishat/c/l9p-KuSMLCo)]]



  
  
On Tuesday, December 10, 2013 1:04:37 AM UTC+8, Nanasaheb wrote:

> Dec 9, 2013 >
> Respected Scholars Namaskar ! >
> I like the way Russian scholarMG doing his research in > various aspects of Sanskrit. If we look into the dictionary of > V.S.Apte, we find no of words involving Moordhanya VarNas (Phonemes) > are small in number. The same is true for the second dental phoneme > (th). I would like to know is there any research within India or > outside about frequency of occurrences of certain phonemes in a given > Sanskrit book on either philosophy or religion or science. This has in > my opinion bearing on semantics of Sanskrit words. Let us not forget > that VarNavaada versus Sphotavaada occupies important place in > Sanskrit linguistic philosophy. Thanks. N.R.Joshi >
>   

If you don’t mind looking at a large corpus encompassing many works (instead of being limited to a specific book), all the data needed for what you are looking for is here -

  

<http://kjc-fs-cluster.kjc.uni-heidelberg.de/dcs/data/syllables/syllables.htm>

  

Dr. Oliver Hellwig of the Digital Corpus of Sanskrit fame has the data-set with frequency counts of all ekāc (single-voweled sounds) in the corpus, with a categorical variable for the time of the work. The data is directly readable in R (my favourite tool for statistical analyses).

  

Here is an approximate estimate of probability of different types ofSparśaconsonants (fricatives) across different times (more precise numbers can be computed, see the R code below which I used for this). Note that the R code on Dr. Hellwig's site does not work - there are a couple of bugs.



 group early epic classical medieval late

1 Gutturals 0.07562657 0.08421253 0.09937352 0.11411426 0.11342108

2 Palatals 0.05272054 0.06074915 0.05501486 0.05503126 0.05577363

3 Retroflexes 0.03191418 0.03231378 0.03561312 0.04080364 0.04139547

4 Dentals 0.32049402 0.31450654 0.31658844 0.32061069 0.31251504

5 Labials 0.19226118 0.19126421 0.18689746 0.17728158 0.17704032



So Nanasaheb Ji is right (we knew it already, did we not), the Retroflexes (Mūrdhanya fricative consonants) are only present in 3-4% of the ekāc sounds in Sanskrit, but so are the Palatals (Tālavya fricative consonants), being present in only 5-6% of the ekāc sounds in Sanskrit.

  

Dr. Hellwig's page also has charts showing some significant t-stats for a non-zero slope when fitting a linear regression increase in frequency of gutturals, retroflexes and labials. This elementary analysis shows that over time the usage of gutturals and retroflexes increased while that of labials decreased. However, as Dr. Hellwig rightly mentions on his page, linear regression is not the right method to test this - the reasons being the time being a categorical variable (and not discrete values corresponding to a continuous scale), and the lack of robustness of linear regression estimates on a sample size as small as four (degree of freedom being only two).



The right tool to use with Dr. Hellwig's data would be Chi-Square test to compare proportions in several groups. This is done by the R function prop.test(). With this test, I found the following in January 2012 -



*“The evidence against the null hypothesis of constant probability across different time periods for the five categories of ekācs is statistically significant for all five groups. The observed evidence is most extreme for Gutturals, Retroflexes and Labials. It is interesting to see that from Medieval to Later period, only Dentals have shown a significant change in their probability ofoccurrencewith p-value of the Chi-Square test being less than 0.1% (a justifiable critical value given the large sample sizes), while from Epic to Classic, evidence shows that probabilities for all five groups have changed. It is also interesting to observe that the probability of Retroflexes occurring in anekācdid not change significantly between Early (Vedic/Upanishadic) and Epic periods, but it did in the post-Epic periods.”*



\> matpvals

 All periods Ea & Ep Ep & Cl Cl & Me
Me & La

Gutturals 0.000000e+00 3.607401e-43 0.000000e+00 0.000000e+00 1.267108e-01

Palatals 1.175834e-246 8.720096e-51 1.598550e-161 9.514065e-01 2.303646e-02

Retroflexes 0.000000e+00 3.181280e-01 6.859133e-92 1.400428e-127 3.685050e-02

Dentals 3.114376e-48 1.022459e-08 6.671614e-07 2.707000e-14 3.677069e-34

Labials 0.000000e+00 2.611753e-01 4.399987e-35 1.750870e-106 6.592439e-01



What Dr. Hellwig's data is missing is the joint probability of two ekācs occuring one after the other - which can give us further insights to the kind of questions Nanasaheb Ji has raised.

  

One day I plan to write a paper on this. But I do not know which journal I can send it to. Maybe we need a conference series on "Sanskrit Statistical Linguistics". Any takers?



# R code for the probability table above

data \<- read.delim( '<http://kjc-fs-cluster.kjc.uni-heidelberg.de/dcs/data/syllables/syllables.dat>', sep=";", header=TRUE, comment.char="#", stringsAsFactors=FALSE);

sums \<-

d \<- data\[order(data$Syllable),\];

sums \<- colSums( data\[,2:6\] );

groups \<- data.frame(rbind(

 c("Gutturals", "k\|g\|G"),

 c("Palatals", "c\|j\|J"),

 c("Retroflexes", "T\|D\|N"),

 c("Dentals", "t\|d\|n"),

 c("Labials", "p\|b\|m")

), stringsAsFactors=FALSE)



Y \<- data.frame();

for(i in 1:nrow(groups))

{

 g \<- grep(groups\[i,2\], data$Syllable, ignore.case=FALSE)

 sub \<- data\[g,\]

 sub.sums \<- colSums(sub\[,2:6\])

 Y \<- rbind( Y,

 cbind( data.frame( group=c( groups$X1\[i\] ) ), data.frame( t( sub.sums / sums ) ) )

 );

};

Y

  

  

