+++
title = "007 Nityanand Misra"

+++
[[Nityanand Misra	2013-12-10, 13:21:45 [Source](https://groups.google.com/g/bvparishat/c/F3z1gYBqS8o)]]



  
  
On Tuesday, December 10, 2013 12:05:34 PM UTC+8, Krishnaprasad wrote:

> 
> > Misra Ji  
>   
> Once again thanks for giving most useful information. Now I understood > like this. I shall use XeLaTeX for typesetting and editing, and > finally I am going to convert it to any of the APS DV fonts.? (Because > for typesetting in XeLaTeX is easier and fonts from APS DV are > beautiful). If I have mistaken something please suggest me. And I hope > I am not giving hassle to you. And I hope to convert to APS DV fonts I > need extra software.  
>   
>   
> > 

  

No, typesetting will have to be done in the final font you want to use. The output of the typesetting in LaTeX is the PS/DVI/PDF document that would be printed as-is. All major and minor aspects including page size, chapter and section headings, page numbers, font size, paragraph spacing, indenting, non-breaking spaces, alignment, table of contents, etc are affected if the font is change, and will be messed up if the font is changed.  

  

This is how I work - I have experimented with both Unicode and non-Unicode (APS DV/Walkman Chanakya fonts).

  

1\. I complete all typing and editing in Microsoft Word using Unicode fonts. I do not begin typesetting at all until I am done with editing. I find the comments and track changes features in very useful for proofreading and editing. Plus if the work is in both Sanskrit and English, Word can help with spelling and grammar check.

2\. I convert the final draft in Word to clean HTML using any of the free online converters like [word2cleanhtml.com/](http://word2cleanhtml.com/). This gives me Unicode plain text with HTML tags. This is helpful since LaTeX's input is plain text and not rich text.

3\. If I am using a non-Unicode font for the typeset, I convert Unicode text to APS-DV/Chanakya using my own sed scripts, leaving the HTML tags as is. Here I take care of escape sequences in LaTeX. This step is not needed if i am typesetting in a Unicode font.

4\. I then convert the HTML tags to LaTeX controls using sed scripts.

  

Steps 1 to 4 are done for each chapter. This generates the XeLaTex files for each chapter.

  

5\. Finally I typeset the book in XeLaTeX using the chapter files.

  

I cannot show you an example output now - I am in Singapore currently on business and do not have access to my output files. However, I will share some sample output typesets with multiple fonts in a few days, with a basic guide to typeset Sanskrit books in XeLaTeX.

  



