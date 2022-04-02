+++
title = "004 Mārcis Gasūns"

+++
[[Mārcis Gasūns	2013-12-21, 21:47:27 [Source](https://groups.google.com/g/bvparishat/c/cNoHQNYriks)]]



  
  
On Saturday, 21 December 2013 16:19:57 UTC+4, Nityanand Misra wrote:

> 
> > 
> > 
> > 
> > > 
> > > > 
> > > > Is the "five-sample Chi-square test" code available for download, > > Nityanand, the prop.test() one? <http://ideone.com/XKVHTM> seems to > > be your testing of it lately. > > > > 
> > > > 
> > 
> >   
> > 
> > 
> > I have lost it. I had it on my old machine. I can write it again, it > is simple. But why do you need it? You would not find it useful unless > you want to statistically test for stability of proportion of a > certain set of syllables across different periods.  
> > 
> > 
> > 
> > 
> > 

I would want to see the difference of output.



> 
> > 
> > 
> > 
> > 
> >   
> Do you have a background in math or statistics? If you do not, I will > add some comments and references also.  
> > 
> > 
> > 
> > 
> > 

I have next to none. So commenting would help a lot, thanks.



> 
> > 
> > 
> > 
> > 
> > 
> > 
> > 
> > 
> > > 
> > > > 
> > > > And I found "I would start with a prose work like Daśakumāracaritam > > rather than a poetic work. The reason is that the constraints of > > prosody may bias the frequency of long and short syllables and in > > some cases also the consonants. For example if you choose a work > > like Meghadūta or Bhṛṅgadūta which is entirely composed in the > > Mandākrāntā, you would get 10 long syllables for every 7 short > > syllables which may be undesirable." at > > <https://groups.google.com/forum/#!msg/samskrita/4oGLpUXyjxI/_xHkmfCfhn4J> > > > > 
> > > > 
> > > > So data for prose and metrical texts separately would maybe change > > the picture even more, who knows. > > > > 
> > > > 
> > > >   
> > > > 
> > > > 
> > 
> >   
> > 
> > 
> > Yes, because data for metrical texts would give you "conditional > probabilities", conditional upon the text fitting the metre. Data for > prose would not have this condition, so one may think of the results > as "unconditional probabilities"  
> > 
> > 
> > 
> > 
> > 

Yes, I agree. But never seen data comparison on such a huge scale.



> 
> > 
> > > 
> > > >   
> > > > 
> > > > Thanks for the code, I made a video how I got different results > > running the same code <http://youtu.be/1IVc7y7ICtc>: > > > > 
> > > > 
> > > > -   \[1\] 337122  
> > -   \[1\] 7566142  
> > -   \[1\] 0.04455666  
> > > > 
> > > > 
> > > > 
> > > > 
> > 
> > I don't know how you got that. I use the raw R GUI, not R Studio. >
> 
> > 
> > 

R GUI is too old-school to me. Studio should not differ in anything, I guess, it just has an UI.



> 
> > 
> > 
> > I saw the video, was interesting to see how you "figure things out" in > something that is totally new, the language here. That I must say is a > talent not many people have.  
> > 
> > 
> > 

Oh, it's bad. My PHP skill are weak, but R - oh, I would never thought I'll get that deep in this swamp.



> 
> > 
> > > 
> > > > 
> > > > sum( data\[grep( "**\[C\]{3}**", data$Syllable2 ),\]$total ) works > > for **CCCV** or VCCC as well? Right, works for both, should not. > > There must be a limitation set. I would want to keep CCCV and VCCC > > seperately and not mix them only because they have CCC (=\[C\]{3}) > > in common. "# Count of triple conjuncts" is not identical to CCCV in > > my case (it remains too vague). > > > > 
> > > > 
> > 
> >   
> > 
> > 
> > There is no case of VCCC in Oliver's data. >
> 
> > 
> > 

Right. In my data as well. No case of CVCC as well.



> 
> > 
> > 
> > Remember he has "single-voweled" syllables. >
> 
> > 
> > 

Yes, but there is only one kind of Indian syllables. There can be no two ways.



> 
> > 
> > 
> > I think you are thinking about Yamuna Kachru's book which firstly > talks about Hindi (which has Schwa syncope) and not Sanskrit and > patterns of words and not single-vowelled syllables (एकाच्).  
> > 
> > 
> > 

No, I did not mean it. Just for reference that there is a work about Hindi, so it could have something in common.



Thanks, some great hints. What I wonder is

-   Number of open syllables?  

sum( data\[grep( "^V$", data$Syllable2 ),\]$total )

\[1\] 255956

  

-   Number of closed syllables?  

sum( data\[grep( "^C$", data$Syllable2 ),\]$total )

\[1\] 0

Why 0?



Right, just a few I've found out with my eye

Markup issues

-   \[la

-   \<p11>pra

-   ''jJa

  

Encoding issues

-   j¤e

-   j¤i

-   S›A

-   ¤jA

-   j¤aH

-   S›hi

-   rS›yA

-   j¤air

-   ›a

-   ›ha

-   жga

  

Bad input

-   9zlSma

-   2ka

-   3va

-   4zo

-   \_\_a

-   \*i

-   \*va

-   \*ya

-   \*nA

-   \*vi

-   \*ni

-   \*cA

-   \*ra

-   \*ka

-   d{}vR

-   \~ci



> 
> > 
> > > 
> > > > 
> > > > "# There are some rows with bad syllable data (\< 0.02%) - retain > > only rows with clean data" - does the 0.02% cuts of the single > > instance only or double ones as well? Have you looked at it? Because > > as you must have noticed it's nasty indeed: > > > > 
> > > > 
> > > >   
> > > > 
> > > > 
> > 
> > 

> 
> > 
> > 
> >   
> > 
> > 
> > No it only throws out characters outside the Harvard-Kyoto > transliteration alphabet.  
> > 
> > 
> > 
> > 
> > 
> > 

> 
> > 
> > 
> > 

Understood.



> 
> > 
> > 
> > 
> > 
> > > 
> > > > 
> > > > As per Elizarenkova a Sanskrit syllable can consist only out of 4 > > elements, CCCVCC at once is impossible. > > > > 
> > > > 
> > 
> >   
> > 
> > 
> > Yes, no occurrence of CCCVCC.  
>   
> > sum( data\[grep( "CCCVCC", data$Syllable2 ),\]$total >
> \[1\] 0 >
>   
> > 
> > 
> > 
> > 
> > > 
> > > > 
> > > > So CCCVCCC > > at<http://books.google.ru/books?id=jQw6AAAAQBAJ&pg=PA33&lpg=PA33&dq=CCCVCC+sanskrit&source=bl&ots=W7KamcV-Ij&sig=AHbIJQ5MeEdUXSQ1-2LM2jx_tq8&hl=en&sa=X&ei=loy0Ur6AG8PDyQPBtIGwAQ&redir_esc=y#v=onepage&q=CCCVCC%20sanskrit&f=false>in > > the Sanskrit samples should be treated as wrong. Wrong? > > > > 
> > > > 
> > > >   
> > > > 
> > > > 
> > 
> >   
> > 
> > 
> > As I said earlier, firstly the page in the book is about Hindi > pronunciation. Hindi has Schwa syncope, Samskrita does not. The words > स्पृष्ट is pronounced CCVCCV in Samskrita, but CCCVCC in Hindi.  
> > 
> > 
> > 

Ah, you one can never trust Hindi :)



> 
> > 
> > 
> > Secondly this page talks about words and not single-syllabled vowels, > which is Oliver's dataset.  
> > 
> > 
> >   
> > 
> > 
> > 

So yes. Oliver has syllables. I have words. There is a gap. No bridge yet. Oliver has corpora. I have 21 dictionary and a huge word list behind me. It was a surprise for me to found out that there are people interested in such topics on this forum. A pleasant surprise and I hope I can find the questions to my answers in the future as well,

  

M.G.

