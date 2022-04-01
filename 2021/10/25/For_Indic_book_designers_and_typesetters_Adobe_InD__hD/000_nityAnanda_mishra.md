+++
title = "000 Nityānanda Miśra"

+++
[[Nityānanda Miśra	2021-10-25, 07:38:42 [Source](https://groups.google.com/g/bvparishat/c/hDjS1ANWp_o)]]



*namo vaḥ*

  

I do not use Adobe InDesign (or any other similar desktop publishing software). I have typeset nearly twenty books and several papers and presentations in LaTeX. Many of these used IAST or Devanagari text and some books were entirely in Hindi or Sanskrit. With XeLaTeX, the use of Devanagari Unicode is quite easy. This is not the case with Adobe InDesign, where a simple operation of copy-pasting Devanagari text from another application needs numerous settings changes and operations to work as expected: ten to fifteen mouse and keyboard operations to get something working when this should all be seamless in a desktop publication application.

  

Recently an InDesign user told me they could not get copy-pasted Unicode Devanagari text working in Adobe InDesign. I installed a trial version of Adobe InDesign, played around, got it working, documented the steps, and finally duly uninstalled Adobe InDesign as I find LaTeX much better.  
  

If one wants to use Adobe InDesign to design/typeset Indic documents or books, here are the steps to copy-paste Unicode Devanagari text and get it working in Adobe InDesign. I have not tried with other Indic scripts but assume similar operations might be needed.

  
1) Copy-paste the Unicode Devanagari text from Word, Chrome, any other application or the Internet into a text box in Adobe InDesign. By default, the matra glyphs and conjunct consonants will be messed up, see the first image.

  
2) Select the copy-pasted text  
  

3\) Click on ‘Window’ → ‘Styles’ → ‘Paragraph Styles’ → ‘New Paragraph Style’, see the second image  
  

4\) In the ‘New Paragraph Style’ pop-up, make the following changes—  
  4a) Under General → Style Name, give this new style a name (e.g., HindiStyle or DevanagariStyle)  
  4b) Under ‘Advanced Character Format’, click ‘Language’ dropdown and choose ‘Hindi (India)’, see third and fourth images  
  4c) Under ‘Justification’, click ‘Composer’ dropdown and choose ‘Adobe World-Ready Composer’, see fifth and sixth images  
  4d) Now click OK at the bottom of the screen, see the seventh image  
  

5\) With the text selected, choose this new HindiStyle (or DevanagariStyle) from the ‘Paragraph Styles’ menu as the paragraph style. This will fix everything, as shown in the eighth image (before choosing the new style) and the ninth image (after choosing the new style).  
  

