+++
title = "002 Nityanand Misra"

+++
[[Nityanand Misra	2021-11-07, 22:05:22 [Source](https://groups.google.com/g/bvparishat/c/Eik4G2wYWMI)]]



On Sunday, 7 November, 2021 at 1:48:38 pm UTC+5:30 श्रीमल्ललितालालितः wrote:  

> 
> > Om, >
> 
> > 
> > I'm using LaTeX to typeset all notes/books. >
> 
> > 
> > I know that PDF created by XeLaTeX doesn't allow proper > search/copy-pasting of devanagari and similar fonts. From the > generated PDF of महावीरी, it is evident that searching becomes normal. > But, copy-pasting is still broken.  
> > 
> > 
> > I'll like to understand the usage of Harfbuzz renderer. How does it > work ? >
> 
> > 
> > Should I create an issue on Github for the same, or answering here is > possible?  
> > 
> >   

  

स्वामिचरणाः,

  

सादरं प्रणम्य निवेदयामि।

  

Could you please confirm which PDF viewer you are using? Also, which string did you try to search and/or copy-paste. In my experience, and that of Sh. Shreevatsa R., both searching and copy-pasting works perfectly in some PDF viewers: these include the Chrome (opening the PDF file in Chrome browser) and the default PDF viewer on Android devices. InAdobe Acrobat Reader on both Windows and macOS, this does not work.

  

On how Harfbuzz rendering (more precisely, text shaping) works, please see these links

  

  

<https://harfbuzz.github.io/>

<https://harfbuzz.github.io/why-do-i-need-a-shaping-engine.html>  

  

Here is an example you can try. The code in red enables Harfbuzz rendering.

  

Compiler: LuaLaTeX

Tex version: TexLive 2020

  

**FILE CONTENTS**

\\documentclass\[twoside\]{book} \\usepackage{babel} \\usepackage{fontspec} \\babelprovide\[mapdigits,main\]{hindi} \\defaultfontfeatures{Renderer=Harfbuzz,Script=Devanagari} \\babelfont{rm}{Noto Serif Devanagari} \\begin{document} \\noindent प्रसन्नतां या न गताऽभिषेकतस्तथा न मम्लौ वनवासदुःखतः।\\\\ मुखाम्बुजश्री रघुनन्दनस्य मे सदाऽस्तु सा मञ्जुलमङ्गलप्रदा॥ \\end{document}  

  

**COMPILED PDF**

Attached

  

**COPY-PASTED TEXT FROM PDF (in Chrome)**

प्रसन्नतां या न गताऽभिषेकतस्तथा न मम्लौ वनवासदुःखतः। मुखाम्बुजश्री रघुनन्दनस्य मे सदाऽस्तु सा मञ्जुलमङ्गलप्रदा॥  

  

**COPY-PASTED TEXT FROM PDF (in Acrobat Reader)**

प्रसन्नतां या न गताऽभिषे कतस्तथा न मम्लौ वनवासदुःखतः।

मुखाम्बुजश्री रघुनन्दनस्य मे सदाऽस्तु सा मञ्जुलमङ

्

गलप्रदा॥

  

As you see, the copy-pasted text works in Acrobat Reader also, but some spaces are inserted randomly for reasons unknown to me.



