+++
title = "001 Nityanand Misra"

+++
[[Nityanand Misra	2014-03-10, 09:08:29 [Source](https://groups.google.com/g/bvparishat/c/-tE_aQOrGnE)]]



  
  
On Monday, March 10, 2014 10:13:51 AM UTC+8, BIPIN KUMAR JHA wrote:

> नमोनमः,  
> php सन्दर्भिता या काचित् समस्या आसीत् तस्याः समाधानं  
> श्रीनित्यानन्दनमिश्रमहाभागेन\* (Nityānanda Miśra  
> <http://nmisra.googlepages.com>) कृतम् अस्तु धन्यवादाः।  
>   

  
For the benefit of others, here is what the problem was. Bipin Jha Ji has Excel data with some columns in Unicode Devanagari. He was saving it as a CSV and then importing in a MySQL database table using phpMyAdmin. This resulted in question mark characters in the columns expected to have Unicode text.  
  
The reason is that when Excel saves a spreadsheet as CSV, it saves the file in the ANSI encoding and not Unicode UTF-8 encoding. This is the default Excel option and I did not find a way to change the encoding.  
  
The solution suggested was to go to Save As in Excel and choose Unicode Text which saves the file in UTF-8 as a tab separated file, with a csv extension. The tabs can then be replaced by commas or semicolons using Search and Replace in a text editor Notepad++ or by using sed on command line in Cygwin. Then the upload would be fine.  
  
The second problem seems to be a font display problem, I am not sure what the solution is.  




