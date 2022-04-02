+++
title = "010 Praveen R. Bhat"

+++
[[Praveen R. Bhat	2020-07-04, 14:06:35 [Source](https://groups.google.com/g/bvparishat/c/l9wYVeHFVGc)]]



Namaste Swamiji,

  

I've just been able to set this up and run the script successfully. I was getting the following error continuously (on Windows 7):

\>\>\>"'charmap' codec can't encode characters in position 0-12: character maps to \<undefined>

  

and the txtfiles came up empty, till I realised that the files are not unicode. I am never coded in Python, so with a little search I was able to add the attribute:encoding="utf-8" to the text file. It looks like it is working now.

  
with open(fname, "w", encoding="utf-8") as f:  

  f.write(html)"on the txtfiles turning out 0 bytes

  

The script is still running, but the files look pretty good. Thanks a lot.  

  

Kind rgds,  
--Praveen R. Bhat  
/\*येनेदं सर्वं विजानाति,तं केन विजानीयात्।Through what should one know That owing to which all this is known! \[Br.Up. 4.5.15\] \*/  

  

  





> To view this discussion on the web visit > [https://groups.google.com/d/msgid/bvparishat/CAJH_SbzsbxjhCjRDJkvN7u9kvXv8-jheEyF3SdCSyi-hs44NUw%40mail.gmail.com](https://groups.google.com/d/msgid/bvparishat/CAJH_SbzsbxjhCjRDJkvN7u9kvXv8-jheEyF3SdCSyi-hs44NUw%40mail.gmail.com?utm_medium=email&utm_source=footer).  

