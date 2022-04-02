+++
title = "028 Shreevatsa R"

+++
[[Shreevatsa R	2020-05-06, 14:20:17 [Source](https://groups.google.com/g/bvparishat/c/7dFy27hsLgg)]]



On Wed, 6 May 2020 at 01:21, Narayan Prasad \<[hin...@gmail.com]()\> wrote:  

> 
> > Why is it said two characters, when out of these two one is already in > use in Telugu?  
> > 
> > Consider the word "gurramu" (horse). >
> 
> > 
> > 
> > I have checked in two dictionaries - C.P. Brown's Telugu-English > Dictionary (2nd edition, 1979/1992, AES) giving the spellingగుర్రము. >
> 
> > 
> >   
> > 
> > 
> > But the 1998 (first edition) of English-Telugu dictionary > gives:గుఱ్ఱము. (see the attached pics.) >
> 
> > 
> > 
> > About 35 years back I saw only the latter spelling in a very > preliminary Telugu book. >
> 
> > 

  

For this, the reasoning given in [the proposal](https://www.unicode.org/L2/L2020/20119-two-telugu-letters.pdf) (fourth paragraph on the first page) is:

  

\> As for ṟ /r/, the Telugu equivalent (ఱ U+0C31) when geminated has a different phonetic realization to that of Tamil. In Telugu, ఱ్ఱ ṟṟa, as expected, is realized as a geminate trill /rra/ but in Tamil ற்ற ṟṟa is uniquely realized as /tt̺ʳ̺ə/.  

\> \[…\]Using this hybrid orthography, the original Tamil phonetic realization of the source text was appropriately preserved in the Telugu script without any loss. It also provided a visual cue to readers that these are Tamil phonemes and care must be taken in pronouncing these characters in accordance to Tamil phonology

  

This may be debatable (I don't know), but the bigger point as I understand it is that for whatever reason, various books printed in the Telugu script have found it (and continue to find it) necessary to use these two characters, so given Unicode'smission of encoding the world's writing systems as actually used in practice, this makes sense (to me at least).

Also, note that a lot of the scripts in Unicode do contain characters that are only used for transcribing “other” languages in that script: the Devanagari block has the short e/o (कॆ, कॊ as opposed to के, को) for transcribing (say) Tamil or Telugu or Kannada, and of course the Latin script has diacritics like ṭ or ḍ — so these characters in the Telugu block marked as “Tamil transcriptional” aren't so unusual.

