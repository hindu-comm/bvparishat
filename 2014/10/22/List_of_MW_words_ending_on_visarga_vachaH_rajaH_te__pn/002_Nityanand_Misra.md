+++
title = "002 Nityanand Misra"

+++
[[Nityanand Misra	2014-10-22, 05:33:46 [Source](https://groups.google.com/g/bvparishat/c/pnYp3GxBRvs)]]



  
Here is what you should do if you plan to list the uninflected forms  
  
Use advanced search in Vacaspatyam online edition  
<http://www.sanskrit-lexicon.uni-koeln.de/scans/VCPScan/2013/web/webtc2/index.php>  
  
Search for words ending in r and s using the Suffix option. Only 36 words end in r. 661 words end in s. Export these to a text file - this will be your lookup file. Make sure both are in same transliteration format.  
Then you can take your list from MW, replace the Visarga by asterisk and add a carat in the front to get a list of regular expressions. Then loop over in a shell script to grep for the regex in the Vacaspatyam file.  
  
To be on the safe side I would also include the 54 Vacaspatyam listings ending in in ṣ, as one needs to watch out for cases like sajuṣ (ससजुषो रुः).



