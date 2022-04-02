+++
title = "000 Amba Kulkarni"

+++
[[Amba Kulkarni	2013-10-20, 08:20:54 [Source](https://groups.google.com/g/bvparishat/c/Zl1bbr9Yg8E)]]



Dear members,  
  

I received the following mail from a person who is developing Devanagari UNicode fonts for Vedic Sanskrit.  
He has some doubts regarding the position of Vedic accent marks vis-a-vis the anuvaaras and anunaasikas.  

  

Will the scholars well-versed with the Vedic writing system help him?  
  
With regards,  
Amba  
  

  

=====================================================================

> ----- Original Message ----- >
> From: "Steve White" \<[swh...@zipcon.net]()\> >
> Sent: 10/03/13 02:50 PM >
> To: Sanskrit Team member >
> Subject: Re: Devanagari test file -- vedic mark encoding and position >
> 
> > 
> > 
> >     Hi Nandu, 
> >     I will attempt to "pose the question" as best I can. 
>     (although several very good responses have been given already.) 
>     Question 1B is pretty well answered.  The others seem to be debatable. 
> >     Q1:  Are there prescribed encoding orders for vedic tone marks 
>          relative to 
>         A) nasalizations (anusvara, visarga, candribindu) 
>          and 
>         B) vowel marks (matra)? 
> >     Q2: what is the preferred graphical position of vedic tone marks 
>          relative to these same other sets of marks? 
> >      ---------------------------------------- 
> >     I should point out there are three distinct "orders" of letters and marks: 
> >     1) the phonological, or "logical" order 
> >     2) the order the letters are input or typed 
> >     3) the encoding order, in which they should appear in Unicode text 
> >     4) the order they should or may be displayed (but often a mark is 
>     displayed over or under another, position isn't really an "order".) 
> >     Different replies on this thread have addressed different ones of these. 
> >      ---------------------------------------- 
> >     Since I first started asking these questions, I've revisited the 
>     relevant Unicode and OpenType documents.  And it's clear why this is 
>     problematic.  The current documents don't quite answer the questions. 
> >     * Unicode Book Chapter 4 Character Properties 
>     * Unicode Book Chapter 9 South Asian Scripts I 
>     http://www.unicode.org/versions/Unicode6.3.0/ 
>     * OpenType terms - especially the "Notation" section 
>     http://www.microsoft.com/typography/otfntdev/indicot/terms.htm 
>     * OpenType on Indic Shaping Engine 
>     http://www.microsoft.com/typography/otfntdev/indicot/shaping.htm 
> >     The Unicde and OpenType standards are pretty clear regarding the 
>     *encoding* order of tone marks with respect to vowels and consonants. 
> >     OpenType clearly shows 
>         [VM] + [SM] (vowel marks before stress/tone marks) 
>     (And I now realize: the inherant 'a' of each consonant makes it 
>     consistent to attach these directly to a consonant glyph.) 
> >      ---------------------------------------- 
>     However, under any interpretation of the docs I have been able to imagine, 
>     I do not see anywhere an explicit statement of where nasalizations 
>     (bindus) such as anusvara and candrabindu may appear in the encoding, 
>     particularly, where they may be encoded with respect to tone marks. 
> >     There is one rough statement in the Unicode doc 
>         "These marks indicate nasalization or final nasal closure of a 
>         syllable" 
>     But does that mean, their encoding must antecede all other marks 
>     in the syllable? 
> >     Unicode classifies most of the Indic marks with the interesting 
>     word "reorderant", which I gather to mean their graphcal representation 
>     might not follow the encoding... I'm really not sure what it means. 
> >     Am I missing something? 
> >     Steve 
> >     AND A FOLLOW-UP 
> > > ----- Original Message ----- > > > > From: "Steve White" \<[swh...@zipcon.net]()\> > > > > Sent: 10/05/13 03:44 PM > > > > To: Sanskrit Team member > > > > Subject: Re: Devanagari test file -- vedic mark encoding and > > position > > > > 
> > > > 
> > > > 
> > > >     Hi again, 
> > > >     Let me give concrete examples of the problem. 
> >     Below are HTML strings, using Unicode character codes, together with 
> >     the Unicode they produce. 
> > > >     These are not rendered properly on Windows or Linux, although the 
> >     encodings are right, to the best of my understanding (of answers from 
> >     your colleagues and from my readings of the standards). 
> > > >         ka+visarga+bindu 
> >         &#x0915;&#x0903;&#x0902; 
> >         कःं 
> > > >         ka+udatta+bindu 
> >         &#x0915;&#x0951;&#x0902; 
> >         क॑ं 
> > > >     This seems not to be a font issue, but rather a behavior of the font 
> >     shaping engine. The effect happens in any font with the capacity to 
> >     show a mismatched mark with a dotted circle. 
> > > >     (Curiously, I made a font with the positioning tables built in for these 
> >     encodings, but neglected to provide dotted circle.  The marks were 
> >     positioned correctly!!  I have no explanation for this.) 
> > > >     With the Siddhanta font and Windows fonts, a different encoding works: 
> >         ka+bindu+udatta 
> >         &#x0915;&#x0902;&#x0951; 
> >         कं॑ 
> >     This is handled by Windows and Linux.  But my understanding was, the 
> >     bindu should come last! 
> > > >     Your thoughts will be much appreciated! > > > > 
> > > > 
> >     
> > 
> > 

  
  
  
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
  

