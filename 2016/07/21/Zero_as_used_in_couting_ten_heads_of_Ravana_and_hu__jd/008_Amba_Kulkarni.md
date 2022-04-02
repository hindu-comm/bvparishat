+++
title = "008 Amba Kulkarni"

+++
[[Amba Kulkarni	2016-07-23, 11:21:26 [Source](https://groups.google.com/g/bvparishat/c/jdzwV53_3fg)]]



Namaste,  
  
I have seen the use of the word शून्य in छन्दशास्त्र of पिङ्गल.  
In the shlookas from 8.28-8.31, he is describing how to obtain powers  
of 2. (2^n in modern notation). The relevant shlokas, their  
translation, with an illustration and its equivalent mathematical  
expression is given below.  
(For more details you may refer to my unpublished paper:  
<http://arxiv.org/abs/math/0703658v2>)  
  
  
dviḥ arddhe (8.28)  
rūpe śūnyam (8.29)  
dviḥ śūnye (8.30)  
tāvadardhe tadguṇitam (8.31)  
  
If the number is divisible by 2(arddhe), divide by 2 and write 2(dvi).  
If not, subtract 1 (rūpe), and write 0 (śūnyam).  
If the answer were 0(śūnya), multiply by  
2(dvi), and if the answer were 2(arddhe),  
multiply (tadguṇitam) by itself (tāvad).  
  
So for example, consider 8.  
8  
4 2 (if even, divide by 2 and write 2)  
2 2 (if even, divide by 2 and write 2)  
1 2 (if even, divide by 2 and write 2)  
0 0 (if odd, subtract 1 and write 0).  
  
Now start with the 2nd column, from bottom to top.  
0 1\*2 = 2 (if 0, multiply by 2)  
2 2^2 = 4 (if 2, multiply by itself)  
2 4^2 = 16 (if 2, multiply by itself)  
2 16^16 = 256 (if 2, multiply by itself).  
  
This algorithm may be expressed in modern notation as  
  
power2(n) = \[power2(n/2)\] ^ 2 if n is even,  
= power2(n-1/2) \* 2, if n is odd,  
= 1, if n = 0.  
  
  
-- Amba Kulkarni  





\>\>\>\>\> an email to [bvparishat+...@googlegroups.com]() \<javascript:>.  

\>\>\>\>\> To post to this group, send email to [bvpar...@googlegroups.com]()  

\>\>\>\>\> \<javascript:>.  

\>\>\>\>\> For more options, visit <https://groups.google.com/d/optout>.  
\>\>\>\>\>  
\>\>\>\> --  
\>\>\>\> You received this message because you are subscribed to the Google  
\>\>\>\> Groups "भारतीयविद्वत्परिषत्" group.  
\>\>\>\> To unsubscribe from this group and stop receiving emails from it, send  

\>\>\>\> an email to [bvparishat+...@googlegroups.com]() \<javascript:>.  

\>\>\>\> To post to this group, send email to [bvpar...@googlegroups.com]()  

\>\>\>\> \<javascript:>.  

\>\>\>\> For more options, visit <https://groups.google.com/d/optout>.  
\>\>\>\>  
\>\>\>  
\>\>\> --  
\>\>\> You received this message because you are subscribed to the Google Groups  
\>\>\>  
\>\>\> "भारतीयविद्वत्परिषत्" group.  
\>\>\> To unsubscribe from this group and stop receiving emails from it, send an  
\>\>\>  

\>\>\> email to [bvparishat+...@googlegroups.com]() \<javascript:>.  

\>\>\> To post to this group, send email to [bvpar...@googlegroups.com]()  

\>\>\> \<javascript:>.  

\>\>\> For more options, visit <https://groups.google.com/d/optout>.  
\>\>\>  
\>\>  
\>\>  
\>\>  
\>\> --  
\>\> My web site : <http://murthygss.tripod.com/index.htm>  
\>\> and also my Sanskrit blog :  
\>\>  
\>\> <http://simplesanskrit.blogspot.com/>  
\>\>  
\>\>  

\>\> \<<http://simplesanskrit.blogspot.com/>\>  
\>\>  
\>\> \*<http://gssmurthy.blogspot.com> \<<http://gssmurthy.blogspot.com/>\>\*  

\>\>  
\>\>  
\>  
\> --  
\> You received this message because you are subscribed to the Google Groups  
\> "भारतीयविद्वत्परिषत्" group.  
\> To unsubscribe from this group and stop receiving emails from it, send an  
\> email to [bvparishat+...@googlegroups.com]().  
\> To post to this group, send email to [bvpar...@googlegroups.com]().  
\> For more options, visit <https://groups.google.com/d/optout>.  
\>  
  
  
--  
  

Fellow,  
Indian Institute of Advanced Study,  
Shimla  
  
आ नो भद्रा: क्रतवो यन्तु विश्वत: ll  
Let noble thoughts come to us from every side.  
- Rig Veda, I-89-i.  
Prof. (On leave)  
Department of Sanskrit Studies  
University of Hyderabad  
Prof. C.R. Rao Road  
Hyderabad-500 046  
  
(91) 040 23133802(off)  
  
<http://sanskrit.uohyd.ac.in/scl> \<<http://sanskrit.uohyd.ernet.in/scl>\>  
<http://sanskrit.uohyd.ac.in/faculty/amba>  
\<<http://sanskrit.uohyd.ernet.in/faculty/amba>\>  

