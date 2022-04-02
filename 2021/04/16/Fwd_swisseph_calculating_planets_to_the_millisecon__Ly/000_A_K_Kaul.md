+++
title = "000 A K Kaul"

+++
[[A K Kaul	2021-04-16, 23:20:32 [Source](https://groups.google.com/g/bvparishat/c/Lyx2s8IUr1E)]]



  
A very informative message especially regarding implications for earlier versions of DE!

AKK  

---------- Forwarded message ---------  
From: **Ron Scott** \<[r1...@hotmail.com]()\>  
Date: Fri, 16 Apr 2021, 22:39  
Subject: Re: \[swisseph\] calculating planets to the millisecond  
To: \<[swis...@groups.io]()\>  

  
  

Hi Eric,

In addition to the other considerations that Alois mentioned, keep in mind that the latest JPL ephemeris (DE441) that came out this week is different from the one a week before (DE431), of which SE-based software (e.g., Solar Fire, Planetdance, Astrolog, etc., implement, as well as from previous versions.

Those who've already done the comparisons this week know that all the primary planets have changed, so this means all other objects have changed as well. The time of the next New Moon has changed to 3 milliseconds EARLIER. Saturn's longitude seems to be most affected, and at both the New Moon in May and in June is 0.015 arc seconds LATER.
And, when the next ephemeris (DE451) is released in a few years, one could bet it will be different as well.

JPL Horizons also uses a different internal time scale (TDB) that considers the irregularities of the Earth's rotation, whereas SE-based software is limited to TT (previously ET), of which is a uniform scale.
So, a slight difference there. Another difference is the choice of which delta-T values to use.

More important, though, than any of these considerations is whether or not our wall-clock time input is properly converted to a usable UT from which to calculate the planets. As you might know, not only is sidereal time rotational by definition, but universal time is as well (i.e., in its primary form UT1). Some astrological programmers are "too busy with other concerns" or they have "other hobbies" that they would like to enjoy rather than dealing with this last consideration or, as some prefer, just deny there's a problem altogether. The standard conversion to sidereal time is done properly, since it's mathematically treated as rotational; however, in the case with the other, we don't see the difference that should be there for every local meridian within a time zone where every Tom, Dick and Harry has arbitrarily synchronized his clock to the LMT of the standard meridian, with a UT result that's homogeneous - NOT different as with ST. Any good astronomer knows the arbitrary synchronization of LMT across longitudes cannot result in the same UT (GMT) for all observers, yet this is what our charts are saying if wall-clock time rather than LMT is used for input. You've heard the expression: "Garbage in, garbage out."

Regards,

Ron Scott

\_.\_,\_.\_,\_

------------------------------------------------------------------------

Groups.io Links:

You receive all messages sent to this group.

[View/Reply Online (#9700)](https://groups.io/g/swisseph/message/9700) \| [Reply To Group]() \| [Mute This Topic](https://groups.io/mt/82129924/1476078) \| [New Topic](https://groups.io/g/swisseph/post)  
[Your Subscription](https://groups.io/g/swisseph/editsub/1476078) \| [Contact Group Owner]() \| [Unsubscribe](https://groups.io/g/swisseph/leave/3311775/1476078/1955436197/xyzzy) \[[jyot...@gmail.com]()\]  

\_.\_,\_.\_,\_

