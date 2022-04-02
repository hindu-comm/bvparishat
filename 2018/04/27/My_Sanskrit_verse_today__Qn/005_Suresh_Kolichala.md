+++
title = "005 Suresh Kolichala"

+++
[[Suresh Kolichala	2018-04-30, 20:57:31 [Source](https://groups.google.com/g/bvparishat/c/Qnumf3ljccg)]]



Wow! Thanks Andrew for your response. Frankly, I didn't expect anyone to respond, let alone someone from Microsoft. So, I am extremely surprised. Thanks for your support. Yes, it is only on the browsers where *dyu* appears as*duya*. I hope theHarfbuzzdevelopers can issue a fix soon.

  

Furthermore, I am not sure if it is a good decision to display dyu with explicit virama, but that's a different discussion.I have many other questions on the implementation of Nirmala UI for other Indian languages. I will reach out to you offline.

  

Thanks again,

Suresh.  

  

  

  

On Sat, Apr 28, 2018 at 3:34 AM, Andrew Glass \<[xad...@live.com]()\> wrote:  

> 
> >  style="font-size:12pt;color:#000000;font-family:Calibri,Helvetica,sans-serif"> >
> Dear Madhav and Suresh, >
>   
> > I do work at Microsoft, and we take font bugs seriously! 😊 >
>   
> > It turns out the problem in this case is with Firefox and Chrome on > Windows 10. These browsers use a font rendering technology called > Harfbuzz. In this case the Nirmala UI font renders this conjunct dyu > with explicit halant. Nirmala UI renders most conjucts horizontally, > often with explicit virama, as is commonplace when typesetting Hindi. > Nirmala UI has been optimized for Hindi becausemost text in > devanagari that rendersonWindows is in Hindi. Now the problem comes > in when Harbuzz tries to position the u-matra on the conjunct dy-. It > seems to get this wrong and try to position the u-matra on the d > component. If you paste this cluster into Notepad on Windows, you get > the correct and expected rendering with the u positioned below the ya. > This rendering is also correct ("dyu") in Microsoft's Edge browser - > which is how I determined that the problem is with Harfbuzz - as I do > see the problem you mentioned, "duya" on Chrome and Firefox. I will > share this observation with the developer of Harfbuzz. >
>   
> > Here is the rendering of this pada in Word on Windows 10 using the > Devanagari fonts that ship with Windows 10. >
>   
> > ![](https://groups.google.com/group/bvparishat/attach/eea50d9420955/pastedImage.png?part=0.1&view=1)  
> >   
> >   
> > Best wishes, >
>   
> > Andrew Glass  
> >   
>   
> > 
> > ------------------------------------------------------------------------ >
> 
> > **From:** INDOLOGY \<[indology-bounces@list.indology.info]()\> on > behalf of Suresh Kolichala via INDOLOGY > \<[indo...@list.indology.info]()\>  
> **Sent:** Friday, April 27, 2018 12:55 PM  
> **To:** Madhav Deshpande  
> **Cc:** Indology; Jayaram Sethuraman; e-shabda-charcha-peeth; > Bharatiya Vidvat parishad; Manik Thakar; Ranjana Date  
> **Subject:** Re: \[INDOLOGY\] My Sanskrit verse today >
> 
> > 
> > 
> > 
> > 
> > 
> > 



