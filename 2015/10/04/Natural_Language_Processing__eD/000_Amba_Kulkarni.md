+++
title = "000 Amba Kulkarni"

+++
[[Amba Kulkarni	2015-10-04, 19:35:23 [Source](https://groups.google.com/g/bvparishat/c/eDUjZjl-qvw)]]



Dear Prof. Kannan,  
  

  

On 3 October 2015 at 11:52, K S Kannan \<[ks.kann...@gmail.com]()\> wrote:  

> 
> > 
> > One of the most complex problems to handle in Natural Language > Processing is marking off word-boundaries, the hardest being the > **spoken** material (any language). The notorious Problem of Juncture > as it is called, it is quite common even in **written** sentences in > Sanskrit. >
> 
> > 
> > 
> > 
> > 

> 
> > 
> > 
> > 
> > A simple example is: >
> 
> > 
> > *na tena likhitam patram, pitur Ajn"A na lopitA !* >
> 
> > 
> >   
> > 
> > 
> > (which can also be construed as
> > 
> > 
> > *natena likhitam patram, pitur Ajn"A na lopitA !).*  
> > 
> > 
> >   
> > 
> > 

> 
> > 
> > 
> > 
> > Examples can be multiplied. >
> 
> > 
> >   
> > 
> > 
> > Handling the complex cases of *sabhan'ga-s'les"a* and > *abhan'ga-s'les"a , (*and *s'abda-s'akti-mUla-dhvani)*are, of course, > a far cry ! >
> 
> > 
> >   
> > 
> > 

  

In NLP, particularly in the field of Machine Translation, scientists are trying to build systems that will translate a text from one language into another automatically.  

However, everybody knows that it is impossible to develop such a system which will translate everything perfectly.  
  

In another effort, groups are developing systems that aim at sharing the load between man and machine rather than providing a perfect translation system. With the current technology, we can process a language string and extract only that much information which is coded in the language string. The clues for what information is coded in a language string and what is not coded are available in Panini's grammar. And we take insights from it while developing the system.  
  

With the help of machine, we provide all possible analyses. Based on the knowledge of 'yogyataa' and the context (extra-linguistic information), then a human being decides the meaning.  
  

Current systems provide help for both the sabhanga '[sle.sa](http://sle.sa) as well as abhanga '[sle.sa](http://sle.sa). In 2012, Dr. Varalakshmi presented her observations on the usefulness of current Sanskrit computational tools for understanding the literary texts such as nalopaakhyaan, for example.  

  

While the current systems can identify the saadhu 'sabdas, and hence split, for example 'natena' as 'na + tena', due to lack of the 'padaartha j\~naana' machine can not determine which splits are meaningless.  
  

For example, for the word 'natena', machine produces following possibilities:  
  

न+तेन/नते+न/नत+इन/नता+इन/नते+अन/नता+एन/नत+एन/नते+इन/न+ते+न/न+ते+अन/न+ते+इन/न+ता+इन/न+ता+एन/  
  
  

  

on <http://sankrit.uohyd.ac.in/scl> which uses head words from Monnier William's dictionary for its morphology.  
  

The same word, when given to Prof. Gérard Huet's system <http://sanskrit.inria.fr> produces 7 possibilities since the dictionary size is now limited. See the file attached.  

All these possibilities are displayed graphically, and one may choose the desired one by clicking on the tick marks / cross marks.  
  
Once I was informed that राजानोददतेसौख्यम् can be split in 0.8 million ways, and there is a manuscript / book(?) in Deccan College which lists all these possibilities. However, my system produces only 238 splits. (By the way I have not seen this manuscript yet, so I do not know whether all the splits produced by machine occur in this list of 8 Lakh possible solutions or not).  
  

Thanks and regards,  

Amba Kulakrni  
  

  

> 
> > 
> > 
> > 
> > KSKannan >
> 
> > 
> > 
> > 
> > 
> >   
> > 
> > On Sat, Oct 3, 2015 at 11:37 AM, K S Kannan > \<[ks.kann...@gmail.com]()\> wrote:  
> > > 
> > > > 
> > > >   
> > > > 
> > > > 
> > > > Lack of punctuation and spacing in Ancient Greek. The image is from > > Codex Sinaiticus, Philippians 1:1-2.  
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
> > > > ![Inline image > > 1](https://groups.google.com/group/bvparishat/attach/8538bab920a32/image.png?part=0.0.1&view=1)  
> > > > 
> > > > 
> > > > Source : Internet > > > > 
> > > > 
> > > >   
> > > > 
> > > > 
> > > >   
> > > > 
> > > > 
> > > > KSKannan > > > > 
> > > > 
> > > > 
> > > > 
> > > > 
> > > >   
> > > > 
> > > > On Sat, Oct 3, 2015 at 11:31 AM, K S Kannan > > \<[ks.kann...@gmail.com]()\> wrote:  
> > > > > 
> > > > > > 
> > > > > > Ancient Greek too had *scripta continua*. No space between words, > > > or even sentences. > > > > > > 
> > > > > > 
> > > > > >   
> > > > > > 
> > > > > > 
> > > > > > Read this Wiki note : > > > > > > 
> > > > > > 
> > > > > >   
> > > > > > 
> > > > > > 
> > > > > > [Ancient > > > Greek](https://en.wikipedia.org/wiki/Ancient_Greek "Ancient Greek")was > > > written*[scripta > > > ontinua](https://en.wikipedia.org/wiki/Scripta_continua "Scripta continua")*without[spacing](https://en.wikipedia.org/wiki/Space_(typography) "Space (typography)")or[interpuncts](https://en.wikipedia.org/wiki/Interpunct "Interpunct"). > > > Over time, a variety of symbols appeared. A system of dots > > > credited to[Aristophanes of > > > Byzantium](https://en.wikipedia.org/wiki/Aristophanes_of_Byzantium "Aristophanes of Byzantium")was > > > developed in the 3rd centuryBC: a[low > > > dot](https://en.wikipedia.org/wiki/Hypostigme "Hypostigme")⟨.⟩marked > > > an occasion for a short breath after a short phrase, > > > a[middot](https://en.wikipedia.org/wiki/Stigme_mese "Stigme mese")⟨·⟩marked > > > an occasion for a longer breath after a longer passage, and > > > a[high > > > dot](https://en.wikipedia.org/wiki/Stigme_teleia "Stigme teleia")⟨˙⟩marked > > > a full stop at the end of a completed thought. Other writers > > > employed[two dot > > > punctuation](https://en.wikipedia.org/wiki/Two_dot_punctuation "Two dot punctuation")⟨⁚⟩to > > > mark the ends of sentences or changing speakers. Less often, > > > arrangements of three⟨⁝⟩, four⟨⁞⟩and⟨⁘⟩, and five > > > dots⟨⁙⟩appeared. Such interline punctuation could be noted or > > > replaced by a variety > > > of[paragraphoi](https://en.wikipedia.org/wiki/Paragraphoi "Paragraphoi"), > > > long marks which trailed between lines of text; these might also > > > mark changes of speakers. Blank lines or > > > various[coronides](https://en.wikipedia.org/wiki/Editorial_coronis "Editorial coronis")marked > > > the ends of sections. (A > > > separate[coronis](https://en.wikipedia.org/wiki/Coronis_(diacritic) "Coronis (diacritic)")was > > > used to > > > mark[contractions](https://en.wikipedia.org/wiki/Crasis "Crasis"); > > > its early forms looked like an apostrophe between the two ellided > > > words.) Over time, the main punctuation came to be a[full > > > stop](https://en.wikipedia.org/wiki/Full_stop "Full stop")marked > > > by a single dot at varying heights, a[partial > > > stop](https://en.wikipedia.org/wiki/Semicolon "Semicolon")marked > > > by various forms > > > of[commas](https://en.wikipedia.org/wiki/Comma "Comma"), and > > > the[hypodiastole](https://en.wikipedia.org/wiki/Hypodiastole "Hypodiastole")⟨⸒⟩and[papyrological > > > hyphen](https://en.wikipedia.org/wiki/Papyrological_hyphen "Papyrological hyphen")⟨‿⟩or⟨͜⟩. > > > These served to show whether an ambiguous series of letters should > > > be read as (respectively) a single word or as a pair of > > > words.^([\[1\]](https://en.wikipedia.org/wiki/Greek_orthography#cite_note-nicky-1)) > > > > > > Following the[advent of > > > printing](https://en.wikipedia.org/wiki/Printing#History "Printing"), > > > most Greek punctuation was gradually standardized > > > with[French](https://en.wikipedia.org/wiki/French_punctuation "French punctuation"): > > > the[hypodiastole](https://en.wikipedia.org/wiki/Hypodiastole "Hypodiastole")was > > > fully unified with the comma, > > > the[comma](https://en.wikipedia.org/wiki/Comma "Comma")serves as > > > the[decimal > > > point](https://en.wikipedia.org/wiki/Decimal_point "Decimal point")(and > > > in this use is called the "hypodiastole"), the[full > > > stop](https://en.wikipedia.org/wiki/Full_stop "Full stop")serves > > > as the[thousands > > > separator](https://en.wikipedia.org/wiki/Thousands_separator "Thousands separator"), > > > and[guillemets](https://en.wikipedia.org/wiki/Guillemet "Guillemet")and[em-length](https://en.wikipedia.org/wiki/Em_dash "Em dash")[quotation > > > dashes](https://en.wikipedia.org/wiki/Quotation_dash "Quotation dash")typically > > > serve to indicate direct > > > speech.^([\[3\]](https://en.wikipedia.org/wiki/Greek_orthography#cite_note-3))The > > > principal difference is the[Greek question > > > mark](https://en.wikipedia.org/wiki/Greek_question_mark "Greek question mark")⟨;⟩, > > > which developed a shape so similar to > > > the[Latinate](https://en.wikipedia.org/wiki/Latin_script "Latin script")[semicolon](https://en.wikipedia.org/wiki/Semicolon "Semicolon")⟨;⟩that[Unicode](https://en.wikipedia.org/wiki/Unicode "Unicode")decomposes > > > its separate code point > > > identically.^([\[1\]](https://en.wikipedia.org/wiki/Greek_orthography#cite_note-nicky-1))The[ano > > > teleia](https://en.wikipedia.org/wiki/Ano_teleia "Ano teleia")middot > > > serves as the Greek semicolon but is so uncommon that it has often > > > been left off of > > > Greek[keyboards](https://en.wikipedia.org/wiki/Computer_keyboard "Computer keyboard").^([\[2\]](https://en.wikipedia.org/wiki/Greek_orthography#cite_note-lookgreek-2)) > > > > > > 
> > > > > > 
> > > > > >   
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > >   
> > > > > > 
> > > > > > On Sat, Oct 3, 2015 at 9:25 AM, Hnbhat B.R. > > > \<[hnbh...@gmail.com]()\> wrote:  
> > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > On Sat, Oct 3, 2015 at 8:17 AM, 'sadasivamurty rani' via > > > > भारतीयविद्वत्परिषत् \<[bvpar...@googlegroups.com]()\> wrote:  
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > > 
> > > > > > > > > >  > > > > style="color:rgb(0,0,0);font-family:arial,helvetica,sans-serif;font-size:16px;background-color:rgb(255,255,255)"> > > > > > > > > > > 
> > > > > > > > > > 1\. Is this question in discussion related to Devanagari > > > > > writing style or Sanskrit phonetic presentation style in any > > > > > script? To be more clear - "Won't the problem focussed in this > > > > > discussion occur if the passage is written in other than > > > > > Devanagari i.e. Roman script or any other regional script?"  
> > > > > > > > > > 
> > > > > > > > > > 
> > > > > > > > > >   
> > > > > > > > > > 
> > > > > > > > > > 
> > > > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > mātṛśulkād upagatāṃ te śriyaṃ na viṣehire / > > > > > > > > 
> > > > > > > > 
> > > > > > > > rarakṣuś ca pituḥ kautsās te bhavanti sma gautamāḥ // Saund_1.22 > > > > // > > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > > The above is usual way of writing in Roman script. The above is > > > > a verse in Saundarananda in Roman schript encoded in IAST roman > > > > script encoded by a westerner.  
> > > > The same verse converted into Devanagari raises the question, as > > > > Usha had asked: > > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > *1. मातृशुल्काद् उपगतां* ते श्रियं न विषेहिरे / > > > > > > > > 
> > > > > > > > 
> > > > > > > > *ररक्षुश् च* पितुः *कौत्सास् ते* भवन्ति स्म गौतमाः //
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > > Is at acceptable in Devanagari writing in comparison to the > > > > present practice of writing we of older generation are used to > > > > as: > > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > *मातृशुल्कादुपगतां*ते श्रियं न विषेहिरे / > > > > > > > > 
> > > > > > > > 
> > > > > > > > *ररक्षुश्च*पितुः*कौत्सास्ते*भवन्ति स्म गौतमाः //
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > > or more recent one practice of writing: > > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > *मातृशुल्काद्* *उपगताम् ते श्रियम्* न विषेहिरे / > > > > > > > > 
> > > > > > > > 
> > > > > > > > *ररक्षुः च पितुः कौत्साः ते* भवन्ति स्म गौतमाः //
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > > particularly in Devanagari, and/or any other Indian language; > > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > > 
> > > > > > > > > >  > > > > style="color:rgb(0,0,0);font-family:arial,helvetica,sans-serif;font-size:16px;background-color:rgb(255,255,255)"> > > > > > > > > > > 
> > > > > > > > > > 
> > > > > > > > > > 
> > > > > > > > > > 2. If this problem occurs while writing the passage in other > > > > > regional or Roman scripts also can this be problem of > > > > > Devananagari only? or of the other scripts too? > > > > > > > > > > 
> > > > > > > > > > 
> > > > > > > > > >   
> > > > > > > > > > 
> > > > > > > > > > 
> > > > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > > In Tamil script there is no combined conjunct letter and there > > > > may be some other scripts, which do not use comjunct letters. > > > > The question relates specifically to Devanagari writing > > > > following the style followed in Roman IAST. (Simple roman script > > > > do not find place in preparing e-texts by scholars). > > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > > 
> > > > > > > > > >  > > > > style="color:rgb(0,0,0);font-family:arial,helvetica,sans-serif;font-size:16px;background-color:rgb(255,255,255)"> > > > > > > > > > > 
> > > > > > > > > > 
> > > > > > > > > > 
> > > > > > > > > > 3. In such case is this a problem with script or Sanskrit > > > > > phonetic principles?
> > > > > > > > > > 
> > > > > > > > > > 
> > > > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > > 
> > > > > > > > > >  > > > > style="color:rgb(0,0,0);font-family:arial,helvetica,sans-serif;font-size:16px;background-color:rgb(255,255,255)"> > > > > > > > > > > 
> > > > > > > > > > The above has been taken with both phonetic principle परः > > > > > संनिकर्षः संहिता and whether it is followed in writing as we > > > > > know as given in the 2nd Devanagari writing with word space > > > > > which is taken/mistaken as violating the परः संनिकर्षः संहिता, > > > > > or a moderated system of writing, with or without word space, > > > > > according to convenience in writing the conjunct letters as > > > > > ररक्षुश्च,कौत्सास्ते, without word space, in pursuance of परः > > > > > संनिकर्षः in संहिता, andगतां ते श्रियं न with space even it > > > > > is संहिता, without space as गतन्ते, श्रियन्न when writing is > > > > > convenient than गतन् ते, श्रियन् न a mixture of both with and > > > > > without space. This is the long and short of the discussion is > > > > > centered. And यथासंभवं the problem could be applied to other > > > > > scripts also where they are applicable. > > > > > > > > > > 
> > > > > > > > > > 
> > > > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > கதாம் தே  ச்ரியம் ந ஁in Tamil, it writes only the conjunct > > > > letters are written as ablove only split. > > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > > దుపగతాం తే శ్రియం న in Telugu as in Devanagari we use.  
> > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > > It has extended, the विसन्धि and संहिता as the normal way of > > > > संहिता and श्लोक-s excepting श्लोकार्ध.
> > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > >   
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > 
> > > > > > > > --  
> > > > निराशीर्निर्ममो भूत्वा युध्यस्व विगतज्वरः।। (भ.गी.)  
> > > > ---  
> > > > You received this message because you are subscribed to the > > > > Google Groups "भारतीयविद्वत्परिषत्" group.  
> > > > To unsubscribe from this group and stop receiving emails from > > > > it, send an email to [bvparishat+...@googlegroups.com]().  
> > > > To post to this group, send email to > > > > [bvpar...@googlegroups.com]().  
> > > > Visit this group at > > > > <http://groups.google.com/group/bvparishat>.  
> > > > For more options, visit <https://groups.google.com/d/optout>.  
> > > > > > > > 
> > > > > > > > 
> > > > > > 
> > > > > >   
> > >   
> > > > > > 
> > > > > >   
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > --  
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > Dr. K.S.Kannan > > > > > > 
> > > > > > 
> > > > > > Professor,
> > > > > > 
> > > > > > 
> > > > > > Centre for Ancient History and Culture, > > > > > > 
> > > > > > 
> > > > > > 
> > > > > > Jain University > > > > > > 
> > > > > > 
> > > > > > 319, 17th Cross, 25th Main, > > > > > > 
> > > > > > 
> > > > > > 6th Phase,J P Nagar, Bangalore - 560 078 > > > > > > 
> > > > > > 
> > > > > > (Ex-Director, Karnataka Samskrit University)  
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > > > 
> > > > 
> > > >   
> >   
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
> > > > Dr. K.S.Kannan > > > > 
> > > > 
> > > > Professor,
> > > > 
> > > > 
> > > > Centre for Ancient History and Culture, > > > > 
> > > > 
> > > > 
> > > > Jain University > > > > 
> > > > 
> > > > 319, 17th Cross, 25th Main, > > > > 
> > > > 
> > > > 6th Phase,J P Nagar, Bangalore - 560 078 > > > > 
> > > > 
> > > > (Ex-Director, Karnataka Samskrit University)  
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
> >   
> > 
> > --  
> > 
> > 
> > 
> > 
> > 
> > 
> > 
> > 
> > 
> > 
> > Dr. K.S.Kannan >
> 
> > 
> > Professor,
> > 
> > 
> > Centre for Ancient History and Culture, >
> 
> > 
> > 
> > Jain University >
> 
> > 
> > 319, 17th Cross, 25th Main, >
> 
> > 
> > 6th Phase,J P Nagar, Bangalore - 560 078 >
> 
> > 
> > (Ex-Director, Karnataka Samskrit University)  
> > 
> > 
> > 
> > 
> > 
> > 
> > 
> > 
> > 
> > 
> > 
> > 
> > --  
> निराशीर्निर्ममो भूत्वा युध्यस्व विगतज्वरः।। (भ.गी.)  
> ---  
> You received this message because you are subscribed to the Google > Groups "भारतीयविद्वत्परिषत्" group.  
> To unsubscribe from this group and stop receiving emails from it, send > an email to [bvparishat+...@googlegroups.com]().  
> To post to this group, send email to [bvpar...@googlegroups.com]().  
> Visit this group at <http://groups.google.com/group/bvparishat>.  
> For more options, visit <https://groups.google.com/d/optout>.  
> > 
> > 

  
  
  
--  

आ नो भद्रा: क्रतवो यन्तु विश्वत: ll  
Let noble thoughts come to us from every side.  
- Rig Veda, I-89-i.  
Assoc Prof.  
Department of Sanskrit Studies  
University of Hyderabad  

Prof. C.R. Rao Road

Hyderabad-500 046  

  
(91) 040 23133802(off)  
  
[http://sanskrit.uohyd.ac.in/scl](http://sanskrit.uohyd.ernet.in/scl)  
[http://sanskrit.uohyd.ac.in/faculty/amba](http://sanskrit.uohyd.ernet.in/faculty/amba)  
  

