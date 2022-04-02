+++
title = "003 Nityanand Misra"

+++
[[Nityanand Misra	2013-12-09, 07:25:47 [Source](https://groups.google.com/g/bvparishat/c/F3z1gYBqS8o)]]



  
  
On Sunday, December 8, 2013 5:28:59 PM UTC+8, Krishnaprasad wrote:

> 
> >   
> Thanks, I want to use the exact font to my upcoming sanskrit book. > Thanks once again, but I could not download any fonts which you > mentioned. Further help would be highly admired.  
> > 

  

I do not know if the APS DV fonts are free or if they are copyrighted. If they are copyrighted, they may not be easily located on the web. Check with your printing press if they have a copy. Many printing businesses dealing with Hindi books have the APS DV fonts, I personally know some of them.

  

Unless you are typesetting (in addition to authoring) the book yourself, your printing press should take care of the fonts. Anyway typing in APS DV fonts is a nightmare (as it is not Unicode compliant). The best way is to finalize and edit the draft in Unicode and then use machine conversion to the APS DV fonts. There are free converters available on the net, but they do not work well for conjuncts and some glyphs.What i have tried in the past, when I was experimenting typesetting with some non-Unicode compliant fonts, is to extract all the distinct one-vowel sounds (what Panini calls "ekaac" in 1-1-14निपात एकाजनाङ्)in the file and then find the right keystroke combination for the best rendering in the font and then do a sed substitution.

  

Such tools are useful for end-to-end publishers - font designer + author/editor + typesetter.

  

  

  



