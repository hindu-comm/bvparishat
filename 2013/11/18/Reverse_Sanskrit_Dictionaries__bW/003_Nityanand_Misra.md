+++
title = "003 Nityanand Misra"

+++
[[Nityanand Misra	2013-11-20, 05:52:08 [Source](https://groups.google.com/g/bvparishat/c/bWzw1cAbWjw)]]



  
  
On Tuesday, November 19, 2013 3:50:03 PM UTC+8, Mārcis Gasūns wrote:

> 
> > Namaste,  
>   
> On Tuesday, 19 November 2013 04:27:22 UTC+4, Nityanand Misra wrote: >
> > 
> > > > 
> > > > Are you planning a Samskrita -> Samskrita reverse dictionary? Or do > > you mean an English/Russian -> Sanskrit dictionary?  
> > > > 
> > > > 
> > 
> > None of the above. Reverse dictionaries are words indexes with some > grammatical data and without meanings. Because it's based on real > books, maybe 20-21 by the end, than there is no need to add them, but > one could look up in the "usual" dictionaries. Otherwise instead of > 1100 pages it would take 4400/ >
> 
> > 
> > 
> > 
> > 

  

Well reverse dictionaries are of different types, giving words for concepts or meanings, words for an ending suffix or morphemes or phonemes, etc. But all dictionaries, including reverse dictionaries, are lists of sorted key-value pairs. Key is what you use to lookup, value is what you get when you lookup the key. If your key (concept or ending syllable or suffix etc) is in Samskrita, and values also in Samskrita, then it is a Samskrita-Samskrita reverse dictionary. If your keys are not in Samskrita, Russian or English, what are they in? Are they hashmaps or md5sums? If not, then it is most likely one of the above and not none of the above.



> 
> > > 
> > > > 
> > > > Yes, I'm aware of this website. More than that - how many OCR > > mistakes have you submitted to them? Lot's of fixing needs to be > > done. But web is web. Print is print. I go for print. I'm no fan of > > web. Even the dictionaries you mentioned I use locally. Because it's > > much faster that way.  
> > > > 
> > > > 
> > 
> > 
> > 
> > 

  

I have not submitted OCR mistakes, but the online MW does provide a link to the scan of the page for every lookup.



> 
> > > 
> > > > 
> > > >   
> > > > 
> > > > 
> > > 
> > > > 
> > > > A very good English-English reverse dictionary is published by > > Readers' Digest Reverse Dictionary > > (<http://www.readersdigestdirect.co.in/reverse-dictionary>) which > > gives words for meanings, and much more infomation. For example if > > you look up "stair", it would give you a diagram showing what is > > "tread", "rise", "baluster" et cetera. > > > > 
> > > > 
> > 
> > Let me explore it, never heard of it before, thanks. Do you have a > scanned page of it? >
> 
> > 
> > 
> > 
> > 

  

I would if I could but I can't so I won't. I don't have it with me now.



> 
> > > 
> > > > 
> > > > In a sense the 19th century dictionaries Sabdakalpadruma and > > Vacaspatyam doubled up as thesauruses > > > > 
> > > > 
> > 
> > No they did not. I will show you it one day, I hope. I have some > interesting numbers, but not enough time to analyze them. Maybe you > can help me? >
> 
> > 
> > 
> > 

  

They list synonyms for many words, which is what a thesaurus does.



> 
> > 
> > 
> > 
> > > 
> > > > 
> > > > and reverse dictionaries too, > > > > 
> > > > 
> > 
> > No, I guess. >
> 
> > 
> > 
> > 
> > 

  

They list types, parts, related concepts which is what RD's reverse dictionaries does.



> 
> > > 
> > > > 
> > > > as under most words they haveतत्पर्यायाः (synonyms),तत्प्रकाराः > > (types),तल्लक्षणम् (characteristics), etc.
> > > > 
> > > > 
> > 
> > What stands behind etc. What more "types" are you aware in them as > well, please tell me. >
> 
> > 
> > 
> > 

  

Look up "Chandas"छन्दस् in Sadbakalpadrumah - an entry spanning multiple pages and you will know.

> 
> > 
> > 
> > 
> > > 
> > > > 
> > > > How do I read your bell shaped frequency count tables?
> > > > 
> > > > 
> > 
> > It shows how many words are of particular length. On the left, 1st > column - length of words. Above row - name of dictionary. >
> 
> > 
> >   
> > 
> > 

  

That is obvious. What is not is what are the rows - column A is missing? I am a statistician for a good part of my job. I see frequency count tables day in and day out - but a frequency count table without row and column labels is like a plot without X and Y axis labels. So send another snap with the missing column and a legend and I can read it better. I want to know if the distribution looks skewed.



> 
> > 
> > 
> > 
> > I've got one idea. I want to kill visargas and -m (4759 cases) at the > end of the word in Apte, so it would have the same word forms as MW. > Is it ok, or do I miss something? >
> 
> > 
> >   
> > 
> > 

  

Your string-length concept may be flawed as you seem to apply it to the transliteration and not on the syllable-length which is what matters in Samskrita. Do you count length of "dh" (ध्) as two or as one? In your table "Sample stats from my dictionary word ending in:", the percentages do not add up to 100% (98.5%) - it is incomplete. I do not seeentries for diphthong vowels "au" and "ai" and aspirated consonants like "dh" etc, whereas most Samskrita dictionaries have words ending in these. Do you count them separately? Or under words ending in "i", "u" or "h". For Samskrit prosody, rhyme, creative writing and crosswords,अज and कार्त्स्न्य are both two-syllabled which is what matters. You would have length 3 for the first one and length 8 for the second one.

  

You probably want something that counts the syllables in the original language and not the letters in the transliteration. Something what this does -

<http://sanskrit.sai.uni-heidelberg.de/Chanda/HTML/>



