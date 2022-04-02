+++
title = "001 Nityanand Misra"

+++
[[Nityanand Misra	2013-12-21, 11:42:12 [Source](https://groups.google.com/g/bvparishat/c/cNoHQNYriks)]]



  
  
On Saturday, December 21, 2013 3:02:56 AM UTC+8, Mārcis Gasūns wrote:

> 
> > 
> > Namaste, >
> 
> > 
> >   
> > 
> > 
> > Is **CCCV** actually a rare syllable in Sanskrit? I do not think so. >
> 
> > 

  
No it is not rare. Of the 7.5 million syllables in Digital Corpus of Sanskrit (DCS), the pattern CCCV occurs in more than 115,000 syllables (around 1.5% of the total syllables).  
  
You can check this and all other combinations of your interest with the R code below.  
  
  

# Read file

data \<- read.delim( '<http://kjc-fs-cluster.kjc.uni-heidelberg.de/dcs/data/syllables/syllables.dat>', sep=";", header=TRUE, comment.char="#", stringsAsFactors=FALSE);

# Delete Avagrahas

data$Syllable \<- gsub( "'", "", data$Syllable );

# There are some rows with bad syllable data (\< 0.02%) - retain only rows with clean data

data \<- data\[ !grepl( '\[^athAHsnevidmyMkuroSpzUjIbgcNDlTRGJL\]', data$Syllable ),\];

# Map to consonants and vowels

data$Syllable2 \<- data$Syllable;

data$Syllable2 \<- gsub( "\[kgcjTDpbtd\]h", "C", data$Syllable2 );

data$Syllable2 \<- gsub( "\[kgcjTDpbBtdDGhJlmnNrsSvVyz\]", "C", data$Syllable2 );

data$Syllable2 \<- gsub( "\[aA\]\[iIuU\]", "V", data$Syllable2 );

data$Syllable2 \<- gsub( "\[aAiIuURLeo\]", "V", data$Syllable2 );

# Count of triple conjuncts

sum( data\[grep( "\[C\]{3}", data$Syllable2 ),\]$total )

\[1\] 116457

# Count of total syllables

sum( data$total )

\[1\] 7566142

# % of syllables with triple conjuncts

sum( data\[grep( "\[C\]{3}", data$Syllable2 ),\]$total ) / sum( data$total )

\[1\] 0.01539186

  

