+++
title = "003 Nityanand Misra"

+++
[[Nityanand Misra	2013-12-21, 17:49:57 [Source](https://groups.google.com/g/bvparishat/c/cNoHQNYriks)]]



Namaste  

  
  

On Sat, Dec 21, 2013 at 5:49 PM, Mārcis Gasūns \<[gas...@gmail.com]()\> wrote:  

> 
> > 
> > Namaste, >
> 
> > 
> >   
> > 
> > 
> > Oliver's data amazing as usual. How did you find it? Seems like from > <https://groups.google.com/d/msg/samskrita/4oGLpUXyjxI/MV4z0uIoTQcJ> >
> 
> > 

  

Yes  



> 
> > 
> > Is the "five-sample Chi-square test" code available for download, > Nityanand, the prop.test() one? <http://ideone.com/XKVHTM> seems to be > your testing of it lately. >
> 
> > 

  

I have lost it. I had it on my old machine. I can write it again, it is simple. But why do you need it? You would not find it useful unless you want to statistically test for stability of proportion of a certain set of syllables across different periods.  
  
Do you have a background in math or statistics? If you do not, I will add some comments and references also.  



> 
> > 
> > And I found "I would start with a prose work like Daśakumāracaritam > rather than a poetic work. The reason is that the constraints of > prosody may bias the frequency of long and short syllables and in some > cases also the consonants. For example if you choose a work like > Meghadūta or Bhṛṅgadūta which is entirely composed in the Mandākrāntā, > you would get 10 long syllables for every 7 short syllables which may > be undesirable." at > <https://groups.google.com/forum/#!msg/samskrita/4oGLpUXyjxI/_xHkmfCfhn4J> >
> 
> > 
> > So data for prose and metrical texts separately would maybe change the > picture even more, who knows. >
> 
> > 
> >   
> > 
> > 

  

Yes, because data for metrical texts would give you "conditional probabilities", conditional upon the text fitting the metre. Data for prose would not have this condition, so one may think of the results as "unconditional probabilities"  



> 
> >   
> > 
> > Thanks for the code, I made a video how I got different results > running the same code <http://youtu.be/1IVc7y7ICtc>: >
> 
> > 
> > -   \[1\] 337122  
> -   \[1\] 7566142  
> -   \[1\] 0.04455666  
> > 
> > 
> > 
> > 

I don't know how you got that. I use the raw R GUI, not R Studio. I saw the video, was interesting to see how you "figure things out" in something that is totally new, the language here. That I must say is a talent not many people have.  



> 
> > 
> > After taking that video I learned to select the whole code and press > the "Run" button. Now I get exactly the same results. Documenting > links <http://samskrtam.ru/sanskrit-r-statistics/> here. >
> 
> > 
> >   
> > 
> > 
> > But the question is not yet answered. It's closer than ever. To > sayCCCV I have to compare it with the other possible combinations. >
> 
> > 
> > -   CCCV  
> -   VCCC  
> -   CVCC  
> -   CCVC  
> > 
> > 
> >   
> > 
> > 
> > sum( data\[grep( "**\[C\]{3}**", data$Syllable2 ),\]$total ) works for > **CCCV** or VCCC as well? Right, works for both, should not. There > must be a limitation set. I would want to keep CCCV and VCCC > seperately and not mix them only because they have CCC (=\[C\]{3}) in > common. "# Count of triple conjuncts" is not identical to CCCV in my > case (it remains too vague). >
> 
> > 

  

There is no case of VCCC in Oliver's data. Remember he has "single-voweled" syllables. I think you are thinking about Yamuna Kachru's book which firstly talks about Hindi (which has Schwa syncope) and not Sanskrit and patterns of words and not single-vowelled syllables (एकाच्).  
  

Try this out after you have run the previous code (input in black, output in red), M is Anusvaara and H is visarga.  
  

# Match exactly "CCCV"

sum( data\[grep( "^CCCV$", data$Syllable2 ),\]$total )

\[1\] 96375

# Match various supersets of "CCCV"

sum( data\[grep( "^CCCCV$", data$Syllable2 ),\]$total )

\[1\] 1021

sum( data\[grep( "^CCCVH$", data$Syllable2 ),\]$total )

\[1\] 2907

sum( data\[grep( "^CCCVC$", data$Syllable2 ),\]$total )

\[1\] 5018

sum( data\[grep( "^CCCVM$", data$Syllable2 ),\]$total )

\[1\] 10866

sum( data\[grep( "^CCCCVC$", data$Syllable2 ),\]$total )

\[1\] 74

sum( data\[grep( "^CCCCVM$", data$Syllable2 ),\]$total )

\[1\] 101

sum( data\[grep( "^CCCCVH$", data$Syllable2 ),\]$total )

\[1\] 24

sum( data\[grep( "^CCCCCV$", data$Syllable2 ),\]$total )

\[1\] 71

96375 + 1021 + 2907 + 5018 + 10866 + 74 + 101 + 24 + 71

\[1\] 116457

sum( data\[grep( "CCCV", data$Syllable2 ),\]$total )

\[1\] 116457

  



> 
> > 
> > Can we be sure Oliver did not mistakes in syllable splitting? I hope > he did not. It seems some of them hint to errors in the OCR of texts. > No? >
> 
> > 

  

Could be bad OCR. There were a lot of rows with "bad data" - rows with characters like â, ã, and æ, and also numbers! Overall there are 1.8% of the rows which I throw out, these rows correspond to less than 0.2% of total syllables. See below (again, code in black, output in red).  

  

# Read file

data \<- read.delim( '<http://kjc-fs-cluster.kjc.uni-heidelberg.de/dcs/data/syllables/syllables.dat>', sep=";", header=TRUE, comment.char="#", stringsAsFactors=FALSE);

sort( unique( unlist( strsplit( data$Syllable, NULL ) ) ) )

\[1\] "'" "-" " " "" "\*" "," "." "/" ";" "?" "\[" "\]" "\_" "{" "}" "\~" "¡" "›" "¤" "\<" ">" "»" "0" "1" "2" "²" "3" "4" "5" "6" "9" "a" "A" "â" "ã" "æ" "b" "c" "d" "D"

\[41\] "e" "g" "G" "h" "H" "i" "I" "í" "j" "J" "k" "l" "L" "m" "M" "n" "N" "o" "p" "r" "R" "s" "S" "t" "T" "u" "U" "v" "V" "y" "z" "Z"

nrow( data )

\[1\] 11670

sum( data$total )

\[1\] 7567475

# Delete Avagraha

data$Syllable \<- gsub( "'", "", data$Syllable );

# There are some rows with bad syllable data (\< 0.02%) - retain only rows with clean data

data \<- data\[ !grepl( '\[^athAHsnevidmyMkuroSpzUjIbgcNDlTRGJL\]', data$Syllable ),\];

sort( unique( unlist( strsplit( data$Syllable, NULL ) ) ) )

\[1\] "a" "A" "b" "c" "d" "D" "e" "g" "G" "h" "H" "i" "I" "j" "J" "k" "l" "L" "m" "M" "n" "N" "o" "p" "r" "R" "s" "S" "t" "T" "u" "U" "v" "y" "z"

nrow( data )

\[1\] 11451

sum( data$total )

\[1\] 7566142

1 - 11451 / 11670

\[1\] 0.01876607

1 - 7566142 / 7567475

\[1\] 0.0001761486

  
  

> 
> > 
> > Anyway I have no clue (I'm learning GREP for months now, but still bad > at it is as regular expressions do not come always easy for me) how to > code CVCC or CCVC. How to compare these 4 between each other. It is > also saidVCC is even rarer. So I have to compare with CVC & CCV. >
> 
> > 

  

You can try out using the code above. There are many people on this forum who can help you with GREP.  



> 
> > 
> > "# There are some rows with bad syllable data (\< 0.02%) - retain only > rows with clean data" - does the 0.02% cutts of the single instance > only or double ones as well? Have you looked at it? Because as you > must have noticed it's nasty indeed: >
> 
> > 
> >   
> > 
> > 

  

No it only throws out characters outside the Harvard-Kyoto transliteration alphabet.  



> 
> > Number of syllables with C >
> 
> > -   \[1\] 0.9638667  
> > 
> > 
> > 
> > 

  

Correct.  



> 
> > 
> > So the rest 0.04 are syllables with V. >
> 
> > 

  

Correct.  



> 
> > 
> > As per Elizarenkova a Sanskrit syllable can consist only out of 4 > elements, CCCVCC at once is impossible. >
> 
> > 

  

Yes, no occurrence of CCCVCC.  
  

sum( data\[grep( "CCCVCC", data$Syllable2 ),\]$total

\[1\] 0

  



> 
> > 
> > So CCCVCCC > at<http://books.google.ru/books?id=jQw6AAAAQBAJ&pg=PA33&lpg=PA33&dq=CCCVCC+sanskrit&source=bl&ots=W7KamcV-Ij&sig=AHbIJQ5MeEdUXSQ1-2LM2jx_tq8&hl=en&sa=X&ei=loy0Ur6AG8PDyQPBtIGwAQ&redir_esc=y#v=onepage&q=CCCVCC%20sanskrit&f=false>in > the Sanskrit samples should be treated as wrong. Wrong? >
> 
> > 
> >   
> > 
> > 

  

As I said earlier, firstly the page in the book is about Hindi pronunciation. Hindi has Schwa syncope, Samskrita does not. The words स्पृष्ट is pronounced CCVCCV in Samskrita, but CCCVCC in Hindi.  
  

Secondly this page talks about words and not single-syllabled vowels, which is Oliver's dataset.  



> 
> > 
> > 
> > 
> > Thanks, >
> 
> > 
> > Marcis >
> 
> > 
> > 
> >   
> > 
> > 
> > 

  


Thanks for the discussion.  

  

--  
Nityānanda Miśra  
Vice President, Equity Markets, Citigroup, Hong Kong SAR  
Member, Advisory Council, JRHU, Chitrakoot, Uttar Pradesh, India  
<http://nmisra.googlepages.com>  
  

