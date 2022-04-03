+++
title = "004 Nityanand Misra"

+++
[[Nityanand Misra	2013-02-23, 07:23:10 [Source](https://groups.google.com/g/bvparishat/c/6xJgOFioVMw)]]



  
  
On Saturday, February 23, 2013 9:31:19 AM UTC+8, Shrisha Rao wrote:

> El feb 23, 2013, a las 6:06 a.m., Nityanand Misra \<nmi...@gmail.com\> > escribió:  
>   
> \> Arye Usha Rani Ji  
> \>  
> \> On Friday, February 22, 2013 4:14:22 PM UTC+8, Usha Rani wrote:  
> \>  
> \> I do not know Kannada script.  
> \>  
> \>   
> \> I wanted to know if the Unicode Kannada script in the site could be > converted to Devanagari Sanskrit.  
> \>  
> \> It is very easy since both scripts are Indic abugida, a conversion > is a simple character replacement. This is not same as converting > Devanagari to IAST or ITRANS as the latter format is not abugida. > Fastest way to do it is to use sed on a UNIX/Linux/cygwin shell that > supports Unicode. I used the following command  
>   
> I beg your pardon, but I do not believe it is that trivial because > Devanagari spellings are quite a bit more complicated; e.g., अङ्ग, > कम्पन, कञ्चन, परन्तप are all written the same way in Kannada as ಅಂಗ, > ಕಂಪನ, ಕಂಚನ, ಪರಂತಪ. The suggested way would thus render in Devanagari > as अंग, कंपन, कंचन, परंतप which is the \*Hindi\* style but probably > not acceptable to most Sanskritists. I believe a similar issue arises > with the Telugu script also.  
>   

  
Dr. Rao, I beg your pardon that you have missed a crucial point here. Please be reminded that neither ಅಂಗ (the \*Kannada\* style) nor अंग (the \*Hindi\* style) is true Sanskrit style, and neither would be acceptable to Sanskritists like you or me. Both Kannada and Hindi speakers claim that their scripts are completely phonetic but this practice of replacing all five पञ्चमवर्ण in संयुक्तs by ಂ or ं is non-phonetic and unscientific, quite unlike how Sanskrit texts are written in Devanagari or IAST.  
  
Most online Devanagari to ITRANS/IAST/Howard Kyoto transliterators render अंग as aṃga and not aṅga. "Garbage in garbage out."  
  


> This can still be addressed by separate replacement rules that look at > the context of the अनुस्वार (as is done in the RomDev mapping for > XeLaTeX), but some further issues may arise with ligatures and other > special characters (चन्द्र-बिन्दु, etc.). There is also a bug in the > Unicode spec for Kannada itself.  
>   

  
This is also easy and can be achieved by adding a few more regular expressions or better still by writing a simple lexer in lex/flex.  


> Regards,  
>   
> Shrisha Rao  
>   

