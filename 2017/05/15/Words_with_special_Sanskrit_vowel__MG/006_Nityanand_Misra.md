+++
title = "006 Nityanand Misra"

+++
[[Nityanand Misra	2017-05-15, 08:54:22 [Source](https://groups.google.com/g/bvparishat/c/MGzDxXEmZ-o)]]



  
  
On Monday, 15 May 2017 10:13:38 UTC+8, Madhav Deshpande wrote:

> 
> > Dear Nityanandji, >
> 
> >   
> > 
> > 
> >   I see that there is a distinctly coded character forऌ, and one > does not have to resort to ल+ऋ>लृ. I was looking for the other > Nirnayasagara style version ल, but the unicode does not seem to offer > the two styles ofल as two separate codes. I know that fonts like > Sanskrit 2003 do offer the Nirnayasagara style typography, but the > unicode itself does not offer a choice. Am I correct in this > assumption? >
> 
> > 
> >   
> > 
> > 
> > Madhav >
> 
> > 
> > 
> > 
> >   
> > 
> > 

  

Dear Prof. Deshpande

  

That is correct, the [Unicode Devanagari Standard](http://unicode.org/charts/PDF/U0900.pdf) has only one code point for ल (U+0932). In Sanskrit 2003 font, the glyph for the code point U+0932 has the old Nirnay Sagar Press style (page 21 under [here](http://www.sanskritweb.net/itrans/itmanual2003.pdf)). This is also the case with Jana Sanskrit and Chandas fonts. Other fonts like Mangal and Arial Unicode MS have the newer style glyph (with the danda). Several fonts offer two glyphs for ल with both styles. The glyphs use two code points. A Unicode font would achieve this by mapping the non-default glyph to a code point in the Private Use Area (PUA) of the font.

  

Three years ago, I typeset the Hindi book Śrībhaktamāla: Mūlārthabodhinī Ṭīkā Sahita (ISBN 978-93-82253-04-4) in XeLaTeX using the font APS DV Stardust. The font is non-Unicode and offers two glyphs for ल. The more aesthetic Nirnay Sagar Press style glyph was used for the book, as can be seen in the title on the cover page under [here](https://www.academia.edu/25181805/Śrībhaktamāla_Mūlārthabodhinī_Ṭīkā_Sahita_)(download link [here](https://www.academia.edu/attachments/45497601/download_file?st=MTQ5NDgxODUzNCwxOTIuMTkzLjEzMi43LDU2ODkwMzM%3D)). The input text was in Unicode Devanagari which was converted to APS DV Stardust font using shell scripts, where I chose the specific glyph.

  

Nityananda

  



