+++
title = "002 Bipin Jha"

+++
[[Bipin Jha	2014-03-10, 09:15:54 [Source](https://groups.google.com/g/bvparishat/c/-tE_aQOrGnE)]]



  

On Mon, Mar 10, 2014 at 9:08 AM, Nityanand Misra \<[nmi...@gmail.com]()\> wrote:  

> 
> > For the benefit of others, here is what the problem was. Bipin Jha Ji > has Excel data with some columns in Unicode Devanagari. He was saving > it as a CSV and then importing in a MySQL database table using > phpMyAdmin. This resulted in question mark characters in the columns > expected to have Unicode text.  
>   
> The reason is that when Excel saves a spreadsheet as CSV, it saves the > file in the ANSI encoding and not Unicode UTF-8 encoding. This is the > default Excel option and I did not find a way to change the > encoding.  
>   
> The solution suggested was to go to Save As in Excel and choose > Unicode Text which saves the file in UTF-8 as a tab separated file, > with a csv extension. The tabs can then be replaced by commas or > semicolons using Search and Replace in a text editor Notepad++ or by > using sed on command line in Cygwin. Then the upload would be fine.  
>   
> The second problem seems to be a font display problem, I am not sure > what the solution is. >
> 

  

Thank You Nidyanandji to explaining accordingly....Now, I may request to all of you to help me regarding 'The second problem'

  

Thank You  
  

With Regards  
  
\*Bipin Kumar Jha\*  
\*साहित्यविभागीयाध्यापकः

<http://sanskrit.nic.in/*>  
  

\*शोधच्छात्रः- CISTS, IIT, Bombay

  

  
तमेव धीरो विज्ञाय प्रज्ञाकुर्वीत ब्राह्मणः।  
नानुध्यायाद् बहूञ्छब्दान्वाचो विग्लापनं हि तदिति॥  
बृहदारण्यकोपनिषदि 4-4-21  
\*A wise seeker knowing should knowledge acquire,\*  
\*Not involving in words, understanding desire,\*  
\*All are mere words save the Self realization,\*  
\*Only tiring of speech is all verbalization!\*  

