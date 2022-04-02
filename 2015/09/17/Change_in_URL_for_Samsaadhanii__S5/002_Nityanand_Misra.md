+++
title = "002 Nityanand Misra"

+++
[[Nityanand Misra	2015-09-17, 20:23:59 [Source](https://groups.google.com/g/bvparishat/c/S5IppL6dfCg)]]



  

Thanks Dr. Kulkarni for the updated link to your wonderful resources.

  

I had a question about the Sandhi tool in Saṃsādhanī. Is this tool complete or is there still work left?

  

I don’t find the rule ओमाङोश्च (PS 6.1.92) being applied where it should be applied. As a result, some final forms are incorrect, and some show the incorrect sutra being applied. This may or may not be easy to implement. Examples follow below.

  

Example 1 from SK:शिव + एहि should result in शिवेहि, as एहि has आङ् so 6.1.92 will block 6.1.88 due to being later in the A (परत्वात्). The Sandhi tool gives the result शिवैहि.

  

The example is difficult as the Sandhi tool needs to parse the second word to infer that an आङ् is present. If there is, then apply 6.1.92 and not 6.1.88.  

  

|           |             |           |               |                     | |-----------|-------------|-----------|---------------|---------------------| | प्रथमपदम् | द्वितीयपदम् | समस्तपदम् | सन्धिः        | सूत्रम्/वार्तिकम्   | | शिव       | एहि         | शिवैहि    | वृद्धि-सन्धिः | वृद्धिरेचि (6।1।88) |

  

Example 2 from SK: शिवाय + ओम् should result in शिवायोम्, as the second work is ओम् so 6.1.92 will block 6.1.88 due to being later in the A (परत्वात्). The Sandhi tool gives the result शिवायौम्.

  

The example is easy as the Sandhi tool needs to just check if the second work is ओम्. If it is, then apply 6.1.92 and not 6.1.88.  

  

  

|           |             |           |               |                     | |-----------|-------------|-----------|---------------|---------------------| | प्रथमपदम् | द्वितीयपदम् | समस्तपदम् | सन्धिः        | सूत्रम्/वार्तिकम्   | | शिवाय     | ओम्         | शिवायौम्  | वृद्धि-सन्धिः | वृद्धिरेचि (6।1।88) |

  

Example 3 from MB: अद्य + अर्श्यात् (आ + ऋश्यात्) should result in अद्यर्श्यात्. The Sandhi tool gives the result अद्यार्श्यात्.

This again is quite difficult as one needs a parser to parse the form अर्श्यात् and conclude that there is आङ् at beginning.

  

Note: Chaukhambha's Mahābhāṣya edition edited by Bhargava Shastri has the reading अर्श्यात् = आ + ऋश्यात्. Even GRETIL digitized text by George Cardona [here](http://gretil.sub.uni-goettingen.de/gretil/1_sanskr/6_sastra/1_gram/pmbhasuu.htm)has arśyāt = ā + ṛśyāt. But there is no root in the dhātupāṭha which starts with ṛ immediately followed by tālavya ś. There is, however, a root ṛṣī gatau which is in the tudādigaṇa. TheMādhavīyā Dhātuvṛttī lists the form ṛṣyāt under the same. It is possible that the correct reading is indeed arṣyāt = ā + ṛṣyāt with themūrdhanya ṣ. I am not sure if Bhargava Shastri or George Cardona have discussed this anywhere.



  

|           |             |               |                   |                             | |-----------|-------------|---------------|-------------------|-----------------------------| | प्रथमपदम् | द्वितीयपदम् | समस्तपदम्     | सन्धिः            | सूत्रम्/वार्तिकम्           | | अद्य      | अर्श्यात्   | अद्यार्श्यात् | सवर्णदीर्घ-सन्धिः | अकः सवर्णे दीर्घः (6।1।101) |

  

Example 4 is my favourite for obvious reasons: नित्य + आनन्द should result in नित्यानन्द with a पररूप by ओमाङोश्च as the second word आनन्द has the preverb आङ्. The Sandhi tool gives the correct result, but the rule stated is incorrect. As the Mahābhāṣya makes clear in the example ofअद्यर्श्यात् (अद्यर्ष्यात्?), the rule ओमाङोश्च blocks अकः सवर्णे दीर्घः.

  

This is again difficult, but not as difficult as एहि and अर्श्यात् (अर्ष्यात्) as the आङ् in आनन्द is more obvious.

  

  

|           |             |            |                   |                             | |-----------|-------------|------------|-------------------|-----------------------------| | प्रथमपदम् | द्वितीयपदम् | समस्तपदम्  | सन्धिः            | सूत्रम्/वार्तिकम्           | | नित्य     | आनन्द       | नित्यानन्द | सवर्णदीर्घ-सन्धिः | अकः सवर्णे दीर्घः (6।1।101) |

  
Thanks, Nityanand



