+++
title = "006 Nityanand Misra"

+++
[[Nityanand Misra	2017-03-10, 05:47:20 [Source](https://groups.google.com/g/bvparishat/c/yrxSm61KCUw)]]



  
  
On Thursday, 9 March 2017 22:31:23 UTC+8, Gstmadhav .raj wrote:

> 
> > Hi.. >
> 
> >   
> > 
> > 
> > My name is Madhva Raj. I am a developer in .net. Can i know what is > this unicode and in what way i can help in  bringing other Sanskrit > books to this unicode. I mean how can i contribute through Github. And > my favourite topic is Sandhyavandnam. How to Start  a Thread on > Sandhyavanndam and Mantrardha. Am i eligible to  open a Thred. >
> 
> > 
> >   
> > 
> > 
> > Thanking you
> > 
> > 
> >   
> > 
> > 
> > Madhva Raj >
> 
> > 
> > 
> > 
> >   
> > 
> > 

  

As you are a .Net developer, I hope you are comfortable with technical topics. Start with the Wikipedia articles on Unicode and UTF-8.

Simply speaking, Unicode is an encoding standard like ASCII. But it is much better than ASCII (whose one-byte encoding represents only 128 characters) in that with its 17 planes it can represent more than one million characters. Just its first plane, the Basic Multilingual Plane, with around 65,000 code points is enough to represent characters of almost all modern-day languages. As the below map shows, most of this space is for characters in Chinese, Japanese, and Korean.

<https://upload.wikimedia.org/wikipedia/commons/8/8e/Roadmap_to_Unicode_BMP.svg>

  

To bring Sanskrit books to Unicode, you need to scan them using a good OCR tool. If the books are already digitized as text (not images), various converters are available to convert from encoding schemes used by different fonts or IAST to Unicode.

