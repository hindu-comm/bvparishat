+++
title = "006 Nityanand Misra"

+++
[[Nityanand Misra	2015-03-22, 08:32:20 [Source](https://groups.google.com/g/bvparishat/c/5q4huzVJlnE)]]



  
  
On Saturday, March 21, 2015 at 3:36:59 PM UTC+5:30, Mārcis Gasūns wrote:

> 
> > Namaste, Nityanand, >
> 
> > 
> > 
> > 
> >  I'm unaware of Indian astronomy. Can you please tell me what is the > meaning of each for the columns, please? Some I think I understand but > might be wrong. Thanks >
> 
> > 
> > 
> > दिनाङ्क मास पक्ष तिथि समाप्ति काल वार नक्षत्र समाप्ति काल योग समाप्ति > काल करण समाप्ति काल सूर्योदय सूर्यास्त व्रत पर्वोत्सवादि >
> 
> > 
> >   
> > 
> > 
> > 

  

Please see below for quickly drafted answers (not proofread or cross-verified, the members on the list may point out mistakes if any). For more details you may need to refer texts of Indian astronomy.  

दिनाङ्क – Date as per Gregorian calendar.

मास – Lunar month.

पक्ष – Bright (waxing moon) or dark (waning moon) fortnight

तिथि – Lunar date, defined as the ceiling of (longitude of sun – longitude of moon) / 12 at the time of sunrise. If greater than 15, then 15 is subtracted from this result. The difference in longitudes gives a continuous variable in the close-open interval \[0,30). After the conditional subtraction, one gets a continuous variable in the close-open interval \[0,15). This variable is then descretized by sampling it at the time of sunrise, and then by the mathematical the ceiling function. The duration of a Tithi ranges between 54 ghatis (21 hours, 36 minutes) to 66 ghatis (26 hours, 24 minutes). The difference in time is due to Kepler's laws of planetary motion which applies to elliptical orbits – the line joining the orbiting body and the focus covers equal area in equal time, hence the longitude covered in every 24 hour period is different. For an in-depth treatment of computation, please see <http://www.tifr.res.in/~vahia/tithi-calculations.pdf>

समाप्ति काल = The local time when the Tithi (defined above) will change after sunrise. Hours greater than 24 means the Tithi ends after the midnight following the sunrise. अ.रा.. stands for अहोरात्र, which means the Tithi will not change even at the next sunrise.  

वार = Day of the week (Sunday, Monday, ...)

नक्षत्र = At the time of the sunrise, ceiling of (longitude of the moon / 13°20’). The division of the longitude of the moon by 13 degrees 20 minutes gives a continuous variable in the close open interval (0,27). The discretization by ceiling results in an integer from 1 to 27, hence 27 names of the Naksatras.

समाप्ति काल = The time when the Naksatras (defined above) will change after sunrise. Hours greater than 24 means the Naksatra ends after the midnight following the sunrise. अ.रा.. stands for अहोरात्र, which means the Naksatra will not change even at the next sunrise.

योग = At the time of the sunrise, the ceiling of ((longitude of sun + longitude of moon) modulo 360) / 13°20'. The summation of longitudes gives a continuous variable in the close open interval (0,720 degrees). Modulo operations maps this to the close open interval (0,360 degrees). The division by 13 degrees 20 minutes gives a continuous variable in the close open interval (0,27). The discretization by ceiling results in an integer from 1 to 27, hence 27 names of the Yogas.

समाप्ति काल = The time when the Yoga (defined above) will change after sunrise.

करण = Half of a Tithi. Two Karanas make up a Tithi. The exact computation is involved, as there are 7 variable and 4 fixed Karanas. You need to refer texts on this topic.  

समाप्ति काल = The local time when the Karana (defined above) changes. Hours greater than 24 means the Karana ends after the midnight following the sunrise.  

सूर्योदय = Time of sunrise in 24 hour format.

सूर्यास्त = Time of sunset in 24 hour format.

व्रत पर्वोत्सवादि = Festivals on the day (too many yes, but that is what India is known for).  

> 
> > 
> > > 
> > > > 
> > 
> > 

