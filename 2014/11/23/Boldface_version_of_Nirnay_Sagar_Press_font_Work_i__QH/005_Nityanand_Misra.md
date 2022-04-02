+++
title = "005 Nityanand Misra"

+++
[[Nityanand Misra	2014-12-06, 10:43:24 [Source](https://groups.google.com/g/bvparishat/c/QHV0ODrEA5s)]]



  
Namaste  
  
Update on the font design: I have been successful in making progress on the most crucial part of Devanagari font design - ligature substitutions using GSUB tables.  
  
<http://fontforge.github.io/gposgsub.html>  
  
I have not used VOLT at all and all has been done using the same free software packages I mentioned before (GIMP, Inkscape, Cygwin, Python with FontForge). Going by my reading of the FontForge library, I doubt if I would ever need to use VOLT.  
  
I have had offline discussions with several people and would like to clarify the following  

1.  The font being designed is indeed a Unicode font.
2.  The goal is not to have a boldface version of Sanskrit 2003 font.
    Sanskrit 2003 makes departures from Nirnay Sagar Press typography at
    several places. The goal is rather to digitize the boldface version
    of Nirnay Sagar Press typography.  
3.  The glyphs being used are from the boldface font of NSP books.
    Specifically I am using the following books by NSP: Amarakośa with
    Vyākhyāsudhā, Rāvaṇārjunīyam and Stavamālā.  
4.  I am open to feedback on glyphs on this list and in fact, prefer
    that to feedback off the list. After all, the font is for lovers of
    Sanskrit books, and so if the readers do not like a glyph, I have to
    change it! However, a public discussion helps as regarding some
    aspects of glyphs, different readers may have different preferences.
    Hence a public discussion helps to guage if some suggested
    improvements will be welcome unanimously by everybody, or if some
    people would prefer the glyph to stay as it is.  
5.  The effort is not a half-measure, and the end goal will be a fully
    functional font, no matter how long it takes.

With this, I attach a small sample of the font (Niramaya20141206.ttf). The attached file supports the following glyphs only  
Consonant: त  
Mātrā-s: आ, इ, उ, ऊ, ऋ  
Modifiers: Anusvāra, Anunāsika, Visarga  
  
A PDF file with a grid superimposed is attached. The XeLaTeX code for the file is below. I have to make changes to Anunāsika sign which is currently fusing with the इ Mātrā. The below signs (उ, ऊ, and ऋ Mātrā-s) do not fuse (see the last line in the PDF).  
  
Welcome your suggestions and feedback. It is a font for you all, so please let me know how you want to have it. :)  
  
Nityānanda  
  
\\documentclass{book}  
\\usepackage{pagegrid}  
\\usepackage\[margin=2.5cm\]{geometry}  
\\usepackage{polyglossia}  
\\setmainlanguage{hindi}  
\\setmainfont\[Script=Devanagari\]{Niramaya20141206}  
\\newfontfamily\\devanagarifont\[Script=Devanagari\]{Niramaya20141206}  
\\begin{document}  
\\fontsize{60}{75}\\selectfont  
\\noindent ततततः\\\\ ततंतँतः\\\\ तातांताँताः\\\\ तितिंतिँतिः\\\\ तुतुंतुँतुः\\\\ तूतूंतूँतूः\\\\ तृतृंतृँतृः\\\\ तृतुतूतु  
\\end{document}



