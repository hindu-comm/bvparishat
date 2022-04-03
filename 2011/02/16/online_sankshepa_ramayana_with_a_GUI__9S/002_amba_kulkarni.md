+++
title = "002 amba kulkarni"

+++
[[amba kulkarni	2011-02-16, 13:13:17 [Source](https://groups.google.com/g/bvparishat/c/9SZR27J_79M)]]



Dear Sir,  
  
Thank you for your valuable feedback. It will definitely help us in improving the tool further.  
Below I have tried to answer your questions.  
  

2011/2/16 Sivasenani Nori \<[sivas...@gmail.com]()\>

  

> 
> > Madam >
> 
> > 
> > 
> > 
> > 
> > It is a wonderful tool, the importance of which for a beginner cannot > be over-emphasised. 100 Slokas is about the optimum kind of work load > where one gets to understand the concepts and encounters most of the > frequently used forms. On top of it, the selection is genuine > classical language (including usages not explained by Panini?); most > importantly, it is rAmakathA giving, as is said, both puNyam and > purushArtham. >
> 
> > 
> > 
> > 
> > 
> > It is very heartening to note that we nowhave some good quality > resources to learn Sanskrit. The entire team which worked on this > needs to be thanked by the Sanskrit-loving community. Kindly pass on > to the team,the gratitude of many who silently appreciate this. The > Chitrapur Math site > (<http://www.chitrapurmath.net/sanskrit/sanskrit_Iesson.asp>) is seen > as one of the best places online to learn Sanskrit. The present site > complements that very nicely. >
> 
> > 
> > 
> > 
> > 
> > There are a few specific questions on the notation used: >
> 
> > 
> > 
> > 
> > 
> > a\) What is the schematic followed in the analysis of vibhaktis? For > instance, what does 'B' in 'B-A' mean? The latter clearly is the > case - A for prathamA, B for dvitIyA and so on. For some verbs 'B-v' > is indicated, for instance, in the case of paripapraccha, but not so > for others, for instance: SrooyatAm. I thought 'v' in 'B-v' in > paripapraccha might indicate present tense, as a similar notation is > used for bibhyati, icchAmi etc.; but, I see that 'B-v' is also the > lable for 'abraveet'. >
> 
> > 
> > 
> > 

This row is purely for the Graphical User Interface. The user interface chooses the colour of the row by referring to the contents of this row.  
As you have guessed correctly, B-A stands for prathama vibhakti, and so on. B-v stands for verb. All the verbs are shown in the red color.  
More help on the interface is available at the 'Help' button on the right hand corner. (<http://sanskrit.uohyd.ernet.in/~scl/sankshepa_ramayanam/ramayana-interface/anusaaraka/help.html>)  
  

> 
> > b\) Similarly in the vigrahavAkyAs for samAsas, there isa problem > with the notation used, T7 etc. >
> 
> > 
> > 
> > 

A tagging scheme for tagging the compounds has been developed by the Sanskrit Consortium. This tagset contains around 55 tags.  
We will make a link to this tagset available on the webpage in a couple of days.  
  

> 
> > c\) Many kridanta-avyayas like tumunantAs, ktvAntAs etc. are not > marked, like jñAtum and SrutvA; similarly particles like ch and hi, > adverbs like ''param', and other avyayas are not marked. I can > understand that this might not have been within the scopeof the > project - but from a beginner's view-point,words like 'sAmpratam' do > require some explanation. >
> 
> > 
> > 

  
Yes, there is no uniformity in the analysis. The whole purpose of this exercise was to see how the technology can be used to develop various tools that will ease the learning process, and help us in accessing texts in Sanskrit. So we took the analysis as was available in the book.  

> 
> > 
> > 
> > 
> > d\) Similarly in the case of the tiÑgantas; even if one were not a > mImAmsaka, onedoes not deny the importance ofverb in a sentence; I > found that identifying the verb first helps me in deciphering aSloka > the fastest.The beginner is left wondering about the details of the > verb - in which lakAra is paripapraccha? What is the dhAtu in that? > And so on. One reason why some modern teachers seem to by shying away > from introducing the bAlarAmAyaNa or nalopAkhyAnam as an introductory > text is because the number of lakAras taught are now reduced to five - > that leaves the internet-savvy beginner all the more clue-less about > lakAras like lit. >
> 

  
The colours in the GUI help you in identifying the verbs. All the verbs are marked in Red colour. The details of the lakaara etc. are also available in the row D. So if you open this row, by clicking on Show/Hide rows, and then selecting D, the morphological analysis will be available to you.  
The design of the interface is such that user has control over the display. User can choose which rows to display and which to not as per his requirement. For example, somebody might be interested in only the Hindi translation and may not like to look at the English one. In that case, he can close the English row(G). Similarly somebody might be interested in looking at the morphological analysis of each word, then he can open row D and so on.  
  

> 
> > 
> > 
> > 
> > A related question. What is the level of automation involved? Say, is > anusArakaat thelevel where it could take aRaghuvamSam and do 70% of > so of the analysis of the text into pada-pATha, identification of each > componentas a subanta or tiÑganta and then thegender, prAtipadika, > case and number / dhAtu, tense/mood, person and number. This abilit > gives the chance for a reasearcher to determine the mudrA or mark of a > particular author using the statistical analysis (as some scholars > attempt to determine whether Sri Sankara wrote a particular work > depending on the usage of mAyA, avidyA and ISvara in particular > senses) of a part of the text. >
> 

  
The Sankshepa Ramayanam version was developed almost manually.  
However, now we have certain tools such as morphological analyser, sandhi and samaasa splitters, which can be used to develop such interfaces for any text automatically.  
  
The current version of the Sanskrit-Hindi anusaaraka uses some of these tools. It is available at <http://sanskrit.uohyd.ernet.in/~scl/SHMT/shmt.html>  
  
As of now it accepts only simple texts (with pada-paa.tha, with anvaya, and with compound words split, and with eka-tinga).  
This gives a reasonable output. It also gives automatic kaaraka analysis.  
Sandhi splitter is not yet integrated with this tool. Some experiments are also on to combine the sandhi splitter of the Huet's Heritage engine (<http://sanskrit.inria.fr>) with the anusaaraka.  
  
One of the long sentences we tried is:  
  
बाल्यकाले रामः दशरथस्य आज्ञया मुनेः विश्वामित्रस्य यज्ञम् राक्षसेभ्यः रक्षितुम् मुनिना सह वनम् अगच्छत्.  
  
We also tried the very first sholka of the ramayanam:  
तपः-स्वाध्याय-निरतम् तपस्वी वाग-विदाम् वरम् नारदम् परिपप्रच्छ वाल्मिकीः मुनि-पुङ्गवम्.  
  
If we give this sholka with anvaya as below, machine produces better kaaraka analysis.  
तपस्वी वाल्मिकीः तपः-स्वाध्याय-निरतम् तपस्वी वाग-विदाम् वरम् मुनि-पुङ्गवम् नारदम् परिपप्रच्छ.  
  
Regarding your comment on Statistical analysis, the tools are now ready. People can start using them for various kind of analysis etc.  
  
They might need some improvement further. Once people start using them, we will get a better feedback on the shortcomings and we can improve them further.  
  
Here I would also like to mention the work of Oliver Hellwig, who uses statistics for developing Sanskrit analysis tools.You can access his Digital Corpus for Sanskrit at <http://kjc-fs-cluster.kjc.uni-heidelberg.de/dcs/index.php>.  
  
Thank you once again for your feedback.  
  
With regards,  
Amba Kulkarni  
  



