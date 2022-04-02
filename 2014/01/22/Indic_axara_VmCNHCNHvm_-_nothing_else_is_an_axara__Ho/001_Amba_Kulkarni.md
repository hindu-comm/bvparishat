+++
title = "001 Amba Kulkarni"

+++
[[Amba Kulkarni	2014-01-22, 20:12:50 [Source](https://groups.google.com/g/bvparishat/c/HoA3aDipL5U)]]



The ISCII91.pdf document describes the syntax in BNF form as follows:  
  
An Indian script word contains one or more syllables, the syntax for which is given in the following  
Backus-Naur Formalism (BNF).  
  
Word ::= {Syllable} \[Cons-Syllable\]  
Syllable ::= Cons-Vowel-Syllable \| Vowel-Syllable  
Vowel-Syllable ::= V \[D\]  
Cons-Vowel-Syllable ::= \[Cons-Syllable\] Full-Cons \[M\] \[D\]  
Cons-Syllabls ::= \[Pure-Cons\] \[Pure-Cons\] Pure-Cons  
Pure-Cons ::= Full-Cons H  
Full-Cons ::= C \[N\]  
  
Following conventions are used in the syntax given above:  
::= defines a relation.  
{} enclose items which may be repeated one or more times.  
\[\] enclose items which may not be present.  
\| separates items, out of which only one can be present.  
  

The version with regular expression is an improvement over this, since now more simple description is available.  
  

Sanskrit does not have Nukta, and hence for Sanskrit the regular expression may be simplified as:  
V\[m\]\|{CH}C(H\|\[v\]\[m\]) in order to avoid the over-generation (ati-vyaapti).  

  

-- Amba Kulkarni  
  

  
  





> --  
> निराशीर्निर्ममो भूत्वा युध्यस्व विगतज्वरः।। (भ.गी.)  
> ---  
> You received this message because you are subscribed to the Google > Groups "भारतीयविद्वत्परिषत्" group.  
> To unsubscribe from this group and stop receiving emails from it, send > an email to [bvparishat+...@googlegroups.com]().  
> To post to this group, send email to [bvpar...@googlegroups.com]().  
> Visit this group at <http://groups.google.com/group/bvparishat>.  
> For more options, visit <https://groups.google.com/groups/opt_out>.  

  
  
  
--  
आ नो भद्रा: क्रतवो यन्तु विश्वत: ll  
Let noble thoughts come to us from every side.  
- Rig Veda, I-89-i.  
Assoc Prof. and Head  
Department of Sanskrit Studies  
University of Hyderabad  

Prof. C.R. Rao Road

Hyderabad-500 046  

  
(91) 040 23133802(off)  
  
<http://sanskrit.uohyd.ernet.in/scl>  
<http://sanskrit.uohyd.ernet.in/faculty/amba>  
  

