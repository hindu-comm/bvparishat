+++
title = "005 dhaval patel"

+++
[[dhaval patel	2014-03-11, 12:57:01 [Source](https://groups.google.com/g/bvparishat/c/-tE_aQOrGnE)]]



I also had this kind of behavior with Google chrome when I was testing my PHP scripts in localhost.  

Please make sure that the font settings of chrome / any other browser you are using is set to utf-8 instead of default "automatic".  
  
The Google Chrome has a peculiar way of determining the font system used.  
It reads the initial lines. and determines the system used.  
  

In your case everything else is in roman script. So it may be taking it as non utf-8 fonts.  
  

Please try setting it to utf-8 if you have not done so so far.  



