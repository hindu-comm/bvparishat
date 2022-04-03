+++
title = "003 Nityanand Misra"

+++
[[Nityanand Misra	2013-02-18, 06:14:24 [Source](https://groups.google.com/g/bvparishat/c/gOyocUxhrxc)]]



Dear Prof Aklujkar

  
  
On Monday, February 18, 2013 2:11:53 AM UTC+8, Ashok Aklujkar wrote:

> As printing through typesetting was introduced, the scripts made a few > compromises. With the coming of the computer age, we may need to make > a few more compromises or compromises of a different sort. Therefore, > there would be nothing wrong in using the viraama a bit more > frequently if so doing we preserve the great ability of the scripts to > reproduce speech accurately.  
>   

  
Truly said, in fact to date I find the typesetting in old Sanskrit books much better - right from late 19th century publications of Vedas (e.g. the commentary by Jwalaprasad Mishra on Shuklayajurveda), the Nirnay Sagar Press titles and even Sanskrit books published as late as 1990s when computers were not used for typesetting. For digital publications, LaTeX is by far the best typesetting system (even though it is daunting for those used to WYSIWYG editors like Word) but until recently there were hardly any options for typesetting Hindi/Sanskrit documents. Typesetting in Adobe InDesign or Corel with non Unicode fonts like APS-DV family produced more beautiful options. But things are changing and with XeLaTeX one can now compose the text using Unicode and fonts like Sanskrit 2003 are a great improvement from Wikner's skt package.  
  
I agree with you about use of viraamas, and I am also in favour of not using Western punctuation like commas, semicolons, quotes, et cetera. In fact if I had my way, I would typeset even without space which is a Western import in Indian writing - and have both gadya and padya compositions typeset like the Sanskrit inscriptions at Dilwara temples, Adalaj step-well, etc.  


>   
> Dear Shri Misra,  
>   
> I am delighted to get the good news that the extraordinary epic > Śrībhārgavarāghavīyam of ;Srii-raama-bhadraacaarya is now available in > electronic form.  
>   
> I have one suggestion to make regarding text composition. Words such > as buddhi and a:nghri should not be printed as बुिद् ध and अिङ् घ्र > The printing should be बुद्् धि and अङ् घ्रि, \*\* unless, of course, > one can print the ligatures in the normal way with the preceding > consonant shortened or placed in the upper part of the resultant > sign.  
>   
> \*\*(Please ignore the spaces in between. The Devanagari-Qwerty > keyboard I have to use here does not enable me to print the > viraama/halanta sign without leaving a space after it vacant; maybe > this is my ignorance about that keyboard),  
>   

  

As the underlying text in my XeLaTeX source files is Unicode (no font), this is in reality a font issue rather than one of text composition. The typesetting is in Unicode, and as is the advantage with Unicode, it can be used with a wide range of fonts and easily converted to IAST, Howard Kyoto, ITRANS, et cetera. I would not need to change the text, but only the display font to fix the above. If you are able to download the PDF, the font Sanskrit 2003 being embedded in it, the conjunct ligatures are printed perfectly with the preceding consonant placed in upper part - see verses 1-2 and 1-14 on page १ (page 9) in PDF.

For the online HTML version, I have set the font as "Arial Unicode MS" since it is installed by default on Windows machines and most of our website viewers are on Windows platform. This shows "buddhi" properly but not "aṅghri" on Windows machines. As you have mentioned you are using Apple MacBook Air, they may not display correctly. I am yet to address this problem. One option I have is to list a set of fonts for the HTML version in order of priority, starting with Sanskrit 2003 and others which display the conjunct ligatures properly, and then keep Arial Unicode MS at end.Then we may advise users to install Sanskrit 2003 for best display results. Other option, of which I am not sure of, is to embed the Sanskrit 2003 font in our website as a web-font so that readers do not need to install the font. I will discuss this issue with other website volunteers and come up with a solution. It will take some time as we will use the same solution for all our HTML pages, so please bear with us. In any case, we will not need to change the composed text as it is in Unicode, which is independent of the display font or platform.

Till we resolve this, may I suggest using the PDF for best viewing results? Or please use the IAST version for online reading. I have not accessed Google Groups from MacBook Air, so I am not sure how you can download a PDF posted here, but you can download [it under  
](http://goog_1262147476)

<http://jagadgururambhadracharya.org/pdfs/JR2002Sribhargavaraghaviyam.pdf>  


>   
> I am aware that the practice you have followed is now found in a > number of Devanagari publications. It should be discouraged.  
>   

  
I agree. It is a lot to do with font selection. For example, see the third foot of the Mangalacharana of the Gītarāmāyaṇam (download under <http://jagadgururambhadracharya.org/pdfs/JR2011Gitaramayanam.pdf>, the verse is at the bottom page number 3 in PDF which has Devanagari page number १). The text is  
  
ऐश्वर्याद्यैः षडङ्घ्रिर्भजनजनिरसं रातु रामानुगेभ्यो  
aiśvaryādyaiḥ ṣaḍaṅghrirbhajanajanirasaṁ rātu rāmānugebhyo  
  
The rendering of aṅghri has the problem you mentioned. Gītarāmāyaṇam was typeset using the "APS DV Stardust" form. It is a beautiful font doubtless, and is popular with printers along with Kruti Dev and Chanakya, but has limited conjunct syllables ligatures - hardly any with the nasal consonants. In this age where Samskrita speakers are rare, typesetters and printers who know Samskrita are even rarer and they do not want to move from fonts like APS DV or Kruti Dev or Chanakya for the fear of losing business of Hindi books. These fonts are more than sufficient for Hindi which substitutes half nasal consonants with the Anusvara.  


> I very much appreciate the contributions you make to the BVP forum.  
>   

  
Likewise.  


> a.a.  
>   

  
Regards, Nityanand  

