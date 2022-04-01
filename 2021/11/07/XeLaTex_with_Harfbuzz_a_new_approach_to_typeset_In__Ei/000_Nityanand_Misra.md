+++
title = "000 Nityanand Misra"

+++
[[Nityanand Misra	2021-11-07, 08:23:20 [Source](https://groups.google.com/g/bvparishat/c/Eik4G2wYWMI)]]



Dear list members

  

I am pleased to announce the release ofthe Mahāvīrī LaTeX Source Code under the GNU General Public License. This is the source code of the first book that I typeset in LuaLaTex with Harfbuzz rendering. Harfbuzz rendering allows Unicode Devanagari text to be correctly copy-pasted and searched using many PDF viewers (including Chrome and PDF viewers on Android devices, there are some issues with Acrobat Reader though). Harfbuzz rendering also corrects the problems when reading PDFs uploaded on some websites like academia. I thank Sh. Shreevatsa R, a member of this list, for introducing me to Harfbuzz renderer some time ago and for hosting the source code on his GitHub page.

  

**BOOK PDF**

  

The book is *Śrī-Hanumān-Cālīsā* (*Mahāvīrī Vyākhyā Sahita*), fourth edition. The full book is freely downloadable [here](https://github.com/shreevatsa/latex-book-sources/blob/main/Mahaviri/Mahaviri_Hindi_2021.pdf) (on GitHub) and also [here](https://jagadgururambhadracharya.org/wp-content/uploads/2021/08/Mahaviri_Hindi_2021.pdf) (on the website run by volunteers of Shri Tulsi Peeth Seva Nyas). Another copy is available [here](https://www.academia.edu/50965409/), on Academia website. A physical copy of the book can be had from [here](https://www.amazon.in/dp/9382253076) (currently out of stock, but should be back in stock in around a week).

  

**LATEX SOURCE CODE**

  

The LaTeX source code used to typeset the book has been released [here](https://github.com/shreevatsa/latex-book-sources/tree/main/Mahaviri) to help other Indic book designers typeset Indic books using LaTeX/LuaLaTeX. The instructions to compile are also on the same page.

  

**TWO THINGS TO NOTE** 1) One problem with LuaLaTeX is that pstricks does not work with it. This is disappointing as pstricks is such a good package for designing book plates and book covers. After spending a lot of time to make pstricks work without any result, I finally decided to design the book cover and plate in XeLaTeX. With the cover and plate designed in XeLaTeX, I had to switch to importing images (and not PDFs) for the PDF I created to be uploaded on Academia. Had I not done this and imported PDFs created in XeLaTeX the Devanagari glyphs on the cover would have been messed up on Academia website.

2) An unexpected outcome was that seamless copy-pasting and searching of Unicode Devanagari does not work in all PDF viewers. For example, when I open the PDF in Chrome and copy-paste the contents of the title page, I get the below in Unicode with no error and can search for terms like विशिष्टशब्दार्थ (मूलपाठ, विशिष्टशब्दार्थ, सामान्यार्थ, व्याख्या, पद्यार्धानुक्रमणी, और शब्दानुक्रमणी सहित भक्तशिरोमणि गोस्वामी तुलसीदासकी सिद्ध रचना) But when I open the PDF in Adobe Acrobat Reader DC (my version is 2021.005.20060) on Windows and copy-paste the contents of the title page, this is what I get with random space characters inserted. (मूलपाठ, वि शि ष्टशब्दार्थ , सामान्यार्थ , व्याख्या, पद्यार्धा नुक्रमणी, और शब्दानुक्रमणी सहि त भक्तशि रोमणि गोस्वामी तुलसीदासकी सि द्ध रचना) Even searching with विशिष्टशब्दार्थ is not successful, one has to search for वि शिष्ट शब्दार्थ to find the string in the PDF in Acrobat Reader. Sh. Shreevatsa R informed me that even on Adobe Acrobat Reader DC 2021.005.20058 on macOS, the copy-pasting is not perfect and the output is with spaces like "मूलपाठ, वि शि ष्टशब्दार्थ , सामान्यार्थ , व्याख्या," etc on Chrome seems to handle the rendering perfectly, but not Adobe Acrobat. I have not tried other PDF viewers on my laptop. On my Android phone (Redmi K20 Pro), the copy-pasting is perfect as in Chrome and I can search for विशिष्टशब्दार्थ. Even on my old Android phone from 2016 (Samsung Galaxy J7 Prime), the copy-pasting is perfect and I can search for विशिष्टशब्दार्थ.   

  

**BOOK DETAILS** शीर्षक: श्रीहनुमान्-चालीसा—महावीरी व्याख्या सहित विषयवस्तु: गोस्वामी तुलसीदास कृत श्रीहनुमान्-चालीसा पर जगद्गुरु स्वामी रामभद्राचार्य कृत महावीरी व्याख्या का चतुर्थ संस्करण। विक्रम संवत् २०४० (सन् १९८३) में मात्र एक दिन में प्रणीत इस व्याख्या के विषय में डॉ. रामचन्द्र प्रसाद ने अपने रामचरितमानस के द्विभाषीय अनुवाद में “हनुमानचालीसा की सर्वश्रेष्ठ व्याख्या” और “वैदुष्यमण्डित टीका” कहा था (दिल्ली: मोतीलाल बनारसीदास, ISBN 978-81-208-0443-2, पृष्ठ ८४९, पादटिप्पणी १)। इस व्याख्या में श्रीहनुमान्-चालीसा के सभी ४३ पद्यों के विशिष्ट शब्दार्थ और अनुवाद सहित व्याख्या की गई है। तृतीय संस्करण की ही भाँति इस चतुर्थ संस्करण में पद्यार्धानुक्रमणी, शब्दानुक्रमणी, और हनुमान्‌जीकी आरती सम्मिलित हैं। भाषा: हिन्दी व्याख्याकार: जगद्गुरु रामानन्दाचार्य स्वामी रामभद्राचार्य संपादक: मनीषकुमार शुक्ल और नित्यानन्द मिश्र पुस्तकरूपरेखा: नित्यानन्द मिश्र अक्षर-संयोजन: नित्यानन्द मिश्र आवरण चित्र: भँवरलाल गिरधारीलाल शर्मा (सन् १९२४–२००७), राजस्थान चित्रकला के प्रसिद्ध पुरोधा प्रकाशक: जगद्गुरु रामभद्राचार्य दिव्याङ्ग विश्वविद्यालय प्रकाशन तिथि: अपरा एकादशी विक्रम संवत् २०७८ (६ जून २०२१) ISBN-13: 978-93-82253-07-5 ISBN-10: 93-822530-7-6 पुस्तक कोटि: पत्रपृष्ठ (paperback) पुस्तक आकार: Metric demy 8vo (138 mm x 216 mm) पृष्ठ संख्या: १०४ (x + ९४) चित्रपृष्ठ संख्या: एक अन्तःपत्र श्रेणी: 80 gsm आवरणपत्र श्रेणी: 300 gsm भार: लगभग १२५ ग्राम मूल्य: निःशुल्क अधोभारण, क्रय मूल्य ₹ १०१

  

I welcome your feedback and comments

  

Thanks,Nityānanda Miśra

  

