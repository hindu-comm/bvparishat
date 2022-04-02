+++
title = "002 Mārcis Gasūns"

+++
[[Mārcis Gasūns	2013-12-21, 15:19:14 [Source](https://groups.google.com/g/bvparishat/c/cNoHQNYriks)]]



Namaste,

  

Oliver's data amazing as usual. How did you find it? Seems like from <https://groups.google.com/d/msg/samskrita/4oGLpUXyjxI/MV4z0uIoTQcJ> Is the "five-sample Chi-square test" code available for download, Nityanand, the prop.test() one? <http://ideone.com/XKVHTM> seems to be your testing of it lately. And I found "I would start with a prose work like Daśakumāracaritam rather than a poetic work. The reason is that the constraints of prosody may bias the frequency of long and short syllables and in some cases also the consonants. For example if you choose a work like Meghadūta or Bhṛṅgadūta which is entirely composed in the Mandākrāntā, you would get 10 long syllables for every 7 short syllables which may be undesirable." at <https://groups.google.com/forum/#!msg/samskrita/4oGLpUXyjxI/_xHkmfCfhn4J>

So data for prose and metrical texts separately would maybe change the picture even more, who knows.

  

Sample extract from Oliver's file sorted by total:

Syllable early epic classical medieval late total

-   ta 3982 78961 45040 31293 18766 178042  
-   va 4983 76569 44747 30717 16986 174002  
-   sa 3893 75864 38874 25986 15449 160066  
-   ma 3412 70903 40963 23539 16112 154929  
-   ra 2534 54458 32641 28499 15644 133776  
-   na 3283 59642 34267 22763 13264 133219  
-   pa 4682 55596 33961 21098 12969 128306  
-   ya 4803 47977 30017 17312 10398 110507  
-   ca 2478 49648 27457 17279 11899 108761  
-   a 5174 57752 21378 13821 7089 105214  

  

Thanks for the code, I made a video how I got different results running the same code <http://youtu.be/1IVc7y7ICtc>:

-   \[1\] 337122  
-   \[1\] 7566142  
-   \[1\] 0.04455666  

After taking that video I learned to select the whole code and press the "Run" button. Now I get exactly the same results. Documenting links <http://samskrtam.ru/sanskrit-r-statistics/> here.

  

But the question is not yet answered. It's closer than ever. To sayCCCV I have to compare it with the other possible combinations.

-   CCCV  
-   VCCC  
-   CVCC  
-   CCVC  

  

sum( data\[grep( "**\[C\]{3}**", data$Syllable2 ),\]$total ) works for **CCCV** or VCCC as well? Right, works for both, should not. There must be a limitation set. I would want to keep CCCV and VCCC seperately and not mix them only because they have CCC (=\[C\]{3}) in common. "# Count of triple conjuncts" is not identical to CCCV in my case (it remains too vague). Can we be sure Oliver did not mistakes in syllable splitting? I hope he did not. It seems some of them hint to errors in the OCR of texts. No?

Anyway I have no clue (I'm learning GREP for months now, but still bad at it is as regular expressions do not come always easy for me) how to code CVCC or CCVC. How to compare these 4 between each other. It is also saidVCC is even rarer. So I have to compare with CVC & CCV.

"# There are some rows with bad syllable data (\< 0.02%) - retain only rows with clean data" - does the 0.02% cutts of the single instance only or double ones as well? Have you looked at it? Because as you must have noticed it's nasty indeed:

  

-   STvI 1 0 0 0 0 1  
-   tvyA 1 0 0 0 0 1  
-   Aj 1 0 0 0 0 1  
-   suk 1 0 0 0 0 1  
-   nuT 1 0 0 0 0 1  
-   sji 1 0 0 0 0 1  
-   lgha 1 0 0 0 0 1  
-   JoH 1 0 0 0 0 1  
-   Ac 1 0 0 0 0 1  
-   pzya 1 0 0 0 0 1  
-   aut 1 0 0 0 0 1  
-   thyR 1 0 0 0 0 1  
-   'suG 1 0 0 0 0 1  
-   Nit 1 0 0 0 0 1  
-   Nal 1 0 0 0 0 1  
-   jvat 1 0 0 0 0 1  
-   GkIM 0 1 0 0 0 1  
-   lpsya 0 1 0 0 0 1  
-   mvo 0 1 0 0 0 1  
-   'nnAd 1 0 0 0 0 1  
-   'dbhyo 1 0 0 0 0 1  
-   ti 0 2 0 0 0 2  
-   ma 0 0 1 0 0 1  

Number of syllables with C

-   \[1\] 0.9638667  

So the rest 0.04 are syllables with V.

As per Elizarenkova a Sanskrit syllable can consist only out of 4 elements, CCCVCC at once is impossible. So CCCVCCC at<http://books.google.ru/books?id=jQw6AAAAQBAJ&pg=PA33&lpg=PA33&dq=CCCVCC+sanskrit&source=bl&ots=W7KamcV-Ij&sig=AHbIJQ5MeEdUXSQ1-2LM2jx_tq8&hl=en&sa=X&ei=loy0Ur6AG8PDyQPBtIGwAQ&redir_esc=y#v=onepage&q=CCCVCC%20sanskrit&f=false>in the Sanskrit samples should be treated as wrong. Wrong?

  

Thanks,

Marcis



