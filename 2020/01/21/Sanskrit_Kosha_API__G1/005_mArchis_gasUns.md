+++
title = "005 Mārcis Gasūns"

+++
[[Mārcis Gasūns	2020-01-26, 15:06:55 [Source](https://groups.google.com/g/bvparishat/c/G1bNqthoNnM)]]



  
  
On Tuesday, 21 January 2020 19:18:24 UTC+3, dhaval wrote:

> 
> > 
> >   
> > 
> > 
> > Currently we have around 30 koshas available in digital format. >
> 
> > 
> > I have developed a small API to search the content matching a given > word from all the dictionaries. >
> 
> > 

  

Mesmerizing, as usual!



  

> 
> > -   `iast` (International Alphabet of Sanskrit Transliteration) > -   `itrans` (ITRANS) > -   `itrans_dravidian` (ITRANS with support for Dravidian short "e" >     and "o") > -   `kolkata` (National Library at Kolkata) > -   `slp1` (Sanskrit Library Phonetic Basic) > -   `velthuis` (Velthuis) > -   `wx` (WX) >
> 

How about Simple?



> 
> > 
> > 
> >   
> > 
> > 
> > 
> > **API description -**  
> > 
> > 
> > <https://kosha.sanskritworld.in/#/default> is the API for programmers. >
> 
> > 
> >   
> > 
> > 
> > 1\. <https://kosha.sanskritworld.in/v0.0.1/dictcode> >
> 
> > 
> > gives the codes and full form of dictionary name. >
> 
> > 
> >   
> > 
> > 
> > 2\. <https://kosha.sanskritworld.in/v0.0.1/query/%7Bquery%7D> >
> 
> > 
> > gives the details of all data matching \`query\` in all dictionaries. >
> 
> > 
> > e.g. <https://kosha.sanskritworld.in/v0.0.1/query/rAma> >
> 
> > 
> >   
> > 
> > 
> > 3\. > <https://kosha.sanskritworld.in/v0.0.1/query/%7Bquery%7D/koshas/%7Bkosha%7D> >
> 
> > 
> > gives the detail of a given \`query\` in given \`kosha\`. >
> 
> > 
> > If you are unsure of the \`kosha\`, see API 1 for short codes. >
> 
> > 
> > e.g. <https://kosha.sanskritworld.in/v0.0.1/query/rAma/koshas/ABCH> >
> 
> > 
> > This will give all details of rAma in dictionary अभिधानचिन्तामणि of > हेमचन्द्र। >
> 
> > 

  

Would love to see a standard, can it be united with<https://cceh.github.io/kosh/>in some way?

