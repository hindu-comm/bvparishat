+++
title = "001 Nityanand Misra"

+++
[[Nityanand Misra	2013-12-16, 06:11:22 [Source](https://groups.google.com/g/bvparishat/c/W9HVqrCG2vE)]]



  
  
On Sunday, December 15, 2013 3:52:55 PM UTC+8, Mārcis Gasūns wrote:

> 
> > 
> > Namaste  
> > 
> > 

> 
> > 
> >   
> > 
> > 
> > I have  
> > 
> > 
> > -   abdhina……vanītaka  
> -   abhavanma……tayoga >
> 
> > 

> 
> > 

  

Not good for a reader. The reading experience is spoiled by splitting "tayoga" instead of "yoga". 

> 
> > 
> > -   
> > 
> > 

> 
> > 
> > -     
> > 
> > 
> > I do not do no morphological analysis. I'm (my PC) is not aware of > "yoga" in "abhavanmatayoga". I split letters, not samasas, upasargas > or whatsoever morphological elements apart. 35619 words out of 255000 > had to be split as they are longer than 15 characters and would not > fit into my column. In the attachment - the whole list of words split. >
> 
> > 
> >   
> > 
> > 
> > M.G. >
> 
> > 

  

If you ask me, a hyphenation scheme which ignores Samaasa, Sandhi, Upasarga, etc is not useful at all in Samskrita. The reading experience can be ruined by splitting the word at the wrong place. Given the flexibility of Samskrita, allowing for possibility of entirely new usages, I doubt if a hyphenation algorithm can do a satisfactory job.

  

  

When I was typesetting Śrībhārgavarāghavīyam in XeLaTeX, I used the Sanskrit hyphenation in TeX for the introduction by Abhirāja Rajendra Miśra and the review by Devarṣi Kalānātha Śāstrī. See the pages 4, 5 and 6 (numbered i to iii) and Page 188 (numbered १८०) in the PDF under here - <http://jagadgururambhadracharya.org/pdfs/JR2002Sribhargavaraghaviyam.pdf>

  

I was not happy with the results. Some hyphenations were just not right. At that time I somehow managed to keep the "bizarre" hyphenations to a minimum by changing the indentation, font size, para spacing et cetera. But still I could not avoid some bad splits. An example - on page praṇītāni (प्रणीतानि) was split as praṇī-tāni (प्रणी-तानि) by TeX. I hated it.

  

Now I have learned better. I fully control hyphenation by using sloppypar with nohyphenation. Two examples -

  

The first example is a sentence with a 200+ word Samaasa from[Adhyātmarāmāyaṇe'pāṇinīyaprayogāṇāṃ Vimarśaḥ](http://jagadgururambhadracharya.org/works/arapv/prastavana.php)

  

वैष्णव­सम्प्रदाये प्रमुखतया निखिल­कोटि­ब्रह्माण्डाधीशो जगदीशः पुरन्दर­त्रिपुर­हर­वसु­विरिञ्चि­पावक­पवमान­हिमभानु­चित्रभानु­कृशानु­निखिल­नक्षत्र­गण­सकल­सुरासुर­यक्ष­गन्धर्व­किन्नर­चारण­सिद्ध­साध्य­नर­नाग­लोक­पाल­नाक­पाल­काल­कराल­व्याल­माल­मौलि­सम्पूजित­पादारविन्द­लेखाधीश­मुकुटमणि­संलालित­चरण­सरोज­रजो­मकरन्द­त्रैलोक्य­लक्ष्मी­नवनलिन­ललित­लोचन­लसित­कमन­कटाक्ष­संवीक्षित­शुभेक्षित­भव्य­सौन्दर्य­सार­सर्वस्व­सकल­सुषमा­सार­भूत­मनोरम­सार्वभौम­शर्वरी­प्राण­वल्लभ­संव्रीडक­मदन­मान­पीडक­वदन­सरसीरुह­निसर्ग­निहित­सुधित­सुधा­माधुरीक­श्रीवत्स­लाञ्छन­शरच्छशाङ्कानन­मधुर­मन्द­स्मित­तुहिनांशु­दीधिति­विहित­प्रपन्न­हृदय­सरसी­कैरव­विकास­ललित­लीला­विलास­महा­लक्ष्मी­निवास­क्षीर­सागर­सम्मन्थन­सञ्जात­कण­संस्पर्श­भग्न­भक्त­भूरि­भव­भय­व्रण­पाणि­पल्लव­जगती­तल­पाथो­विप्लव­नाशित­प्रणिपात­क्लव­विरचित­गणिका­गजाजामिल­पङ्किल­पङ्क­कलङ्क­भव­विहित­भव­संस्तव­करुणार्णव­सकल­शरण्य­वरण्य­तरुणारुण­सरसिज­चरण­तरुण­तमाल­नील­सरसीरुह­मरकत­मणि­कालिन्दी­कीलाल­विनिन्दक­भुवनाभि­राम­श्याम­शरीर­दामिनी­द्युति­विनिन्दक­संवीत­पीत­परिधान­म्लान­मदमत्त­मनोभव­धीर­मधु­कैटभ­नरक­मुर­प्रचुर­महासुर­भूरि­मद­गर्वित­गजेन्द्र­गण्डस्थल­विनिर्गत­शोणित­करकमल­कलित­कौमोदकी­धर­शङ्ख­चक्र­धर­कमल­कलित­कमल­कर­केयूर­कुण्डल­कटक­वनमाला­नूपुरादि­भूषण­मण्डित­सकल­कला­कलाप­पण्डित­कमलामल­मुख­चन्द्र­चकोर­वैकुण्ठ­विहरण­परायण­नारायण­प्रभविष्णु­विष्णुर्हृदय­मन्दिरे महीयते।

  

For this, I would use only soft-hyphens (&shy; in HTML, and \\- in TeX). And the TeX code will read

  

\\begin{sloppypar}\\hyphenrules{nohyphenation}\\justifying वैष्णव­सम्प्रदाये प्रमुखतया निखिल­कोटि­ब्रह्माण्डाधीशो जगदीशः पुरन्दर\\-त्रिपुर\\-हर\\-वसु\\-विरिञ्चि\\-पावक\\-पवमान\\-हिमभानु\\-चित्रभानु\\-कृशानु\\-निखिल\\-नक्षत्र\\-गण\\-सकल\\-सुरासुर\\-यक्ष\\-गन्धर्व\\-किन्नर\\-चारण\\-सिद्ध\\-साध्य\\-नर\\-नाग\\-लोक\\-पाल\\-नाक\\-पाल\\-काल\\-कराल\\-व्याल\\-माल\\-मौलि\\-सम्पूजित\\-पादारविन्द\\-लेखाधीश\\-मुकुटमणि\\-संलालित\\-चरण\\-सरोज\\-रजो\\-मकरन्द\\-त्रैलोक्य\\-लक्ष्मी\\-नवनलिन\\-ललित\\-लोचन\\-लसित\\-कमन\\-कटाक्ष\\-संवीक्षित\\-शुभेक्षित\\-भव्य\\-सौन्दर्य\\-सार\\-सर्वस्व\\-सकल\\-सुषमा\\-सार\\-भूत\\-मनोरम\\-सार्वभौम\\-शर्वरी\\-प्राण\\-वल्लभ\\-संव्रीडक\\-मदन\\-मान\\-पीडक\\-वदन\\-सरसीरुह\\-निसर्ग\\-निहित\\-सुधित\\-सुधा\\-माधुरीक\\-श्रीवत्स\\-लाञ्छन\\-शरच्छशाङ्कानन\\-मधुर\\-मन्द\\-स्मित\\-तुहिनांशु\\-दीधिति\\-विहित\\-प्रपन्न\\-हृदय\\-सरसी\\-कैरव\\-विकास\\-ललित\\-लीला\\-विलास\\-महा\\-लक्ष्मी\\-निवास\\-क्षीर\\-सागर\\-सम्मन्थन\\-सञ्जात\\-कण\\-संस्पर्श\\-भग्न\\-भक्त\\-भूरि\\-भव\\-भय\\-व्रण\\-पाणि\\-पल्लव\\-जगती\\-तल\\-पाथो\\-विप्लव\\-नाशित\\-प्रणिपात\\-क्लव\\-विरचित\\-गणिका\\-गजाजामिल\\-पङ्किल\\-पङ्क\\-कलङ्क\\-भव\\-विहित\\-भव\\-संस्तव\\-करुणार्णव\\-सकल\\-शरण्य\\-वरण्य\\-तरुणारुण\\-सरसिज\\-चरण\\-तरुण\\-तमाल\\-नील\\-सरसीरुह\\-मरकत\\-मणि\\-कालिन्दी\\-कीलाल\\-विनिन्दक\\-भुवनाभि\\-राम\\-श्याम\\-शरीर\\-दामिनी\\-द्युति\\-विनिन्दक\\-संवीत\\-पीत\\-परिधान\\-म्लान\\-मदमत्त\\-मनोभव\\-धीर\\-मधु\\-कैटभ\\-नरक\\-मुर\\-प्रचुर\\-महासुर\\-भूरि\\-मद\\-गर्वित\\-गजेन्द्र\\-गण्डस्थल\\-विनिर्गत\\-शोणित\\-करकमल\\-कलित\\-कौमोदकी\\-धर\\-शङ्ख\\-चक्र\\-धर\\-कमल\\-कलित\\-कमल\\-कर\\-केयूर\\-कुण्डल\\-कटक\\-वनमाला\\-नूपुरादि\\-भूषण\\-मण्डित\\-सकल\\-कला\\-कलाप\\-पण्डित\\-कमलामल\\-मुख\\-चन्द्र\\-चकोर\\-वैकुण्ठ\\-विहरण\\-परायण\\-नारायण\\-प्रभविष्णु\\-विष्णुर्हृदय\\-मन्दिरे
महीयते।\\end{sloppypar}

  

The second example is a sentence with two long words which I want to hyphenate only if they must be, and one words I want to hyphenate in all cases fromŚrīgītātātparyanirṇaya -

  

इस प्रकार चतुर्थ अध्याय भी भगवत्तत्त्वज्ञानपूर्वक कर्मसंन्यासयोग रूप ईश्वर-शरणागति की मङ्गलमय सरणि में ही अध्यवसित हुआ।  

  

For this, I would use a mixture of soft-hyphens (&shy; in HTML, and \\- in TeX) and hyphens (- in HTML and TeX). And the TeX code will read

  

\\begin{sloppypar}\\hyphenrules{nohyphenation}\\justifying\\noindent इस प्रकार चतुर्थ अध्याय भी भगवत्तत्त्व\\-ज्ञान\\-पूर्वक कर्मसंन्यास\\-योग रूप ईश्वर-शरणागति की मङ्गलमय सरणि में ही अध्यवसित हुआ।\\end{sloppypar}

  

Any editor would like to have maximum control over the typesetting result. Which is why I use TeX. And if I do not trust a feature in TeX to give me the required control of the result, I do not use it. Which is why I do not use TeX hyphenation and would rather do it myself. To me, each syllable and letter in the works that I edit is a priceless gem from my Guru, which I cannot afford to leave in the unsafe hands of a hyphenating tool that cannot do justice to the text.

  

  

