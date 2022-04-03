+++
title = "003 Shrisha Rao"

+++
[[Shrisha Rao	2013-02-23, 07:01:19 [Source](https://groups.google.com/g/bvparishat/c/6xJgOFioVMw)]]



El feb 23, 2013, a las 6:06 a.m., Nityanand Misra \<[nmi...@gmail.com]()\> escribió:  
  
\> Arye Usha Rani Ji  
\>  
\> On Friday, February 22, 2013 4:14:22 PM UTC+8, Usha Rani wrote:  
\>  
\> I do not know Kannada script.  
\>  
\>  
\> I wanted to know if the Unicode Kannada script in the site could be converted to Devanagari Sanskrit.  
\>  
\> It is very easy since both scripts are Indic abugida, a conversion is a simple character replacement. This is not same as converting Devanagari to IAST or ITRANS as the latter format is not abugida. Fastest way to do it is to use sed on a UNIX/Linux/cygwin shell that supports Unicode. I used the following command  
  

I beg your pardon, but I do not believe it is that trivial because Devanagari spellings are quite a bit more complicated; e.g., अङ्ग, कम्पन, कञ्चन, परन्तप are all written the same way in Kannada as ಅಂಗ, ಕಂಪನ, ಕಂಚನ, ಪರಂತಪ. The suggested way would thus render in Devanagari as अंग, कंपन, कंचन, परंतप which is the \*Hindi\* style but probably not acceptable to most Sanskritists. I believe a similar issue arises with the Telugu script also.  
  
This can still be addressed by separate replacement rules that look at the context of the अनुस्वार (as is done in the RomDev mapping for XeLaTeX), but some further issues may arise with ligatures and other special characters (चन्द्र-बिन्दु, etc.). There is also a bug in the Unicode spec for Kannada itself.  
  
Regards,  
  
Shrisha Rao  
  

