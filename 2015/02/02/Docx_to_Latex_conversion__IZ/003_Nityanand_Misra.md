+++
title = "003 Nityanand Misra"

+++
[[Nityanand Misra	2015-02-03, 13:22:17 [Source](https://groups.google.com/g/bvparishat/c/IZ3NSCBlG1E)]]



  

I did this many months ago (sometime in 2013) with a simpler two-step approach - 1) convert content in a Word document to HTML 2) Convert HTML content to LaTeX.

  

For the first step, one can use Microsoft Word to save the document as an HTML file, but the HTML generated is horrible (the folks at Redmond do not believe in keeping things simple, do they?). There are tools like<http://word2cleanhtml.com/> (this is what I used) which do a much better job. I have not tried saving Word file in the Word XML format, I am not sure if that is easier.

  

The second step was a bash script using perl, sed, grep, et cetera.

  

I now typeset books in simple and customized XML. Can be easily converted to any format (HTML, LaTeX, EPUB, Kindle book, etc).



