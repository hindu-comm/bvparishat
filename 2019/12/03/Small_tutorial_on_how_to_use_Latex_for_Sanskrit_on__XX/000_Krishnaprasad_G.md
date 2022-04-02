+++
title = "000 Krishnaprasad G"

+++
[[Krishnaprasad G	2019-12-03, 13:12:46 [Source](https://groups.google.com/g/bvparishat/c/XXRlceuKRdw)]]



Dear all  

I have struggled when I wanted use Latex for Sanskrit. There is no good beginner's tutorial on the internet. So here is the small tutorial Part 1. (part 2 etc will contain the explanationof current codealong with more options to try)

  

Please check PDF file for the Pictures.

  

1 Google for Miketex Windows and download and install. <https://miktex.org/download>

  

2 After installation open tex file (which appears as notepad).

 

3 copy and paste the below code into the untitled-1.tex file. (you can replace Sanskrit line as you like) and save the file as Test.tex

\\documentclass\[12pt,titlepage,openany\]{book}

\\usepackage{polyglossia}

\\setdefaultlanguage{sanskrit}

\\usepackage{fontspec}

\\newfontfamily\\sanskritfont{Sanskrit2003}

\\fontspec{Sanskrit2003}



\\begin{document}



\\fontsize{16.5pt}{20pt}{\\selectfont



मङ्गलाचरणम्।\\\\

लक्ष्मीकौस्तुभवक्षसं मुररिपुं शङ्खासिकौमोदकी-\\\\

हस्तं पद्मपलाशताम्रनयनं पीताम्बरं शार्ङ्गिणम्।\\\\

मेघश्याममुदारपीवरचतुर्बाहुं प्रधानात्परं\\\\

श्रीवत्साङ्कमनाथनाथममृतं वन्दे मुकुन्दं मुदा॥१॥\\\\

न्यायाभासतमश्छन्नशास्त्रतत्त्वार्थदर्शिकाम्।\\\\

कुमारिलमतेनाहं करिष्ये शास्त्रदीपिकाम्॥२॥\\\\





अनेन सूत्रेण प्रारीप्सितस्य शास्त्रस्य श्रोतृप्रवृत्तिसिद्धये धर्मज्ञानं प्रयोजनं कथ्यते। यदा हि धर्मजिज्ञासा कर्तव्येत्युक्ते शास्त्रमारभ्यमाणं दृश्यते तदा नूनमिदं शास्त्रं धर्मज्ञानप्रयोजनमित्यवगम्यते॥

}

\\end{document}



4 Select XeLaTeX from the drop down button on the left corner on the topside.

  

5 Click on the green button on the left corner on the topside. (whick looks like Play button on music player)

  

6 If you are asked to install any missing packages give permission.

  

7 Wait a moment, and the PDF file will be generated as Test.PDF in the same folder where you have saved Test.TeX



