+++
title = "022 Harsha M"

+++
[[Harsha M	2019-01-07, 12:48:41 [Source](https://groups.google.com/g/bvparishat/c/pbUn1CgjPyQ)]]



Hi All,

  

Sorry for opening a closed thread.

  

Instead of OCR this is the algorithm I am thinking of following:  

 -- First split the letters in a sample printed text using imagemagic,.

 -- For every letter, if not already done manually map it to a unicode character or set of characters. -- This is a one time act for one particular font. --- this is **map**.

 -- Subsequently once all the letters are available to map, feed the entire scanned page to imagemagic and convert the pages to unicode using the above mapping -- this is **reduce**.

  

This helps us for one particular font, **no OCR** as it is a manual map.

  

Since we dont map handwritten/palm-leaf manuscripts, and limit it to scanned printed pages, we dont need huge data set during the learning phase. However as we continue this for more books, the previous data sets can be used for learning as well. **No ML** as the data set is limited. This **is a simple map-reduce algorithm**.

  

Has anybody attempted this? If yes give me some inputs. I would like to try this approach this year.

  

Regards,

Harsha

  

  

  

  

  

ಮಂಗಳ, ಜುಲೈ 17, 2018 ರಂದು 05:51 ಅಪರಾಹ್ನ ಸಮಯಕ್ಕೆ ರಂದು Devaraj Adiga \<[geta...@gmail.com]()\> ಅವರು ಬರೆದಿದ್ದಾರೆ:  























> 
> > 
> > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > > 
> > > > > > 
> > > > > > 
> > > > > > > 
> > > > > > > >  > > > style="font-family:&quot;courier new&quot;,courier,monaco,monospace,sans-serif;font-size:16px"> > > > > > > > > 
> > > > > > > >  > > > style="font-family:&quot;Helvetica Neue&quot;,Helvetica,Arial,sans-serif;font-size:13px;color:rgb(38,40,42)"> > > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > To unsubscribe from this group and stop receiving emails from > > > > it, send an email to [bvparishat+...@googlegroups.com](). > > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > 
> > 

> 
> > 
> > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > > 
> > > > > > 
> > > > > > 
> > > > > > > 
> > > > > > > >  > > > style="font-family:&quot;courier new&quot;,courier,monaco,monospace,sans-serif;font-size:16px"> > > > > > > > > 
> > > > > > > >  > > > style="font-family:&quot;Helvetica Neue&quot;,Helvetica,Arial,sans-serif;font-size:13px;color:rgb(38,40,42)"> > > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > To post to this group, send email to > > > > [bvpar...@googlegroups.com]().  
> > > > For more options, visit <https://groups.google.com/d/optout>.  
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > 
> > 

> 
> > 
> > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > > 
> > > > > > 
> > > > > > 
> > > > > > > 
> > > > > > > > 
> > > > > > > > --  
> > > > You received this message because you are subscribed to a topic > > > > in the Google Groups "भारतीयविद्वत्परिषत्" group.  
> > > > To unsubscribe from this topic, visit > > > > <https://groups.google.com/d/topic/bvparishat/pbUn1CgjPyQ/unsubscribe>.  
> > > > > > > > 
> > > > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > 
> > 

> 
> > 
> > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > > 
> > > > > > 
> > > > > > 
> > > > > > > 
> > > > > > > > 
> > > > > > > > To unsubscribe from this group and all its topics, send an email > > > > to [bvparishat+...@googlegroups.com](). > > > > > > > > 
> > > > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > 
> > 

> 
> > 
> > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > > 
> > > > > > 
> > > > > > 
> > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > To post to this group, send email to > > > > [bvpar...@googlegroups.com]().  
> > > > For more options, visit <https://groups.google.com/d/optout>.  
> > > > > > > > 
> > > > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > 
> > 

> 
> > 
> > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > > --  
> > > You received this message because you are subscribed to the Google > > > Groups "भारतीयविद्वत्परिषत्" group.  
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > 
> > 

> 
> > 
> > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > > To unsubscribe from this group and stop receiving emails from it, > > > send an email to [bvparishat+...@googlegroups.com](). > > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > 
> > 

> 
> > 
> > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > >   
> > > To post to this group, send email to > > > [bvpar...@googlegroups.com]().  
> > > For more options, visit <https://groups.google.com/d/optout>.  
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > 
> > 

> 
> > 
> > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > --  
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > >   
> > आ नो भद्रा: क्रतवो यन्तु विश्वत: ll  
> > Let noble thoughts come to us from every side.  
> > - Rig Veda, I-89-i. > > > > 
> > > > 
> > > >   
> > > > 
> > > > 
> > > > Professor & Head  
> > Department of Sanskrit Studies  
> > University of Hyderabad  
> > > > 
> > > > 
> > > > Prof. C.R. Rao Road
> > > > 
> > > > Hyderabad-500 046  
> > > > 
> > > >   
> > (91) 040 23133802(off) > > > > 
> > > > 
> > > >   
> > > > 
> > > > 
> > > > [http://scl.samsaadhanii.in](http://sanskrit.uohyd.ac.in/faculty/amba) > > > > 
> > > > 
> > > > <http://sanskrit.uohyd.ac.in/scl> > > > > 
> > > > 
> > > > [http://tdil-dc.in/scl](http://sanskrit.uohyd.ac.in/scl)  
> > > > 
> > > > 
> > > > <http://sanskrit.uohyd.ac.in/faculty/amba> > > > > 
> > > > 
> > > >   
> > > > 
> > > > 
> > > >   
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > 
> > 

> 
> > 
> > > 
> > > > 
> > > > --  
> > You received this message because you are subscribed to the Google > > Groups "भारतीयविद्वत्परिषत्" group.  
> > > > 
> > > > 
> > 
> > 

> 
> > 
> > > 
> > > > 
> > > > To unsubscribe from this group and stop receiving emails from it, > > send an email to [bvparishat+...@googlegroups.com](). > > > > 
> > > > 
> > 
> > 

> 
> > 
> > > 
> > > > 
> > > >   
> > To post to this group, send email to > > [bvpar...@googlegroups.com]().  
> > For more options, visit <https://groups.google.com/d/optout>.  
> > > > 
> > > > 
> > 
> > 

> 
> > 
> > > 
> > > > 
> > > > 
> > > > 
> > 
> >   
>   
>   
> --  
> > 
> > 
> >  Regards  
> Devaraj Adiga >
> 
> > 
> > 
> > 
> > 
> > 
> > 
> > --  

> You received this message because you are subscribed to the Google > Groups "भारतीयविद्वत्परिषत्" group.  

> To unsubscribe from this group and stop receiving emails from it, send > an email to [bvparishat+...@googlegroups.com]().



