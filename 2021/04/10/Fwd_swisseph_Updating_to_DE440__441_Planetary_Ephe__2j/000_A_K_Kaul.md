+++
title = "000 A K Kaul"

+++
[[A K Kaul	2021-04-10, 09:10:10 [Source](https://groups.google.com/g/bvparishat/c/2jYjQOWARz8)]]



Respected members of BVP,

Jai Shri Ram!

The below being a very interesting and informative mail especially for the ones who are "fixing" the dates of the Mahabharata war and "Rama Ravana Yuddha" etc., I am taking the liberty of forwarding it to this august forum.

With regards and Jai Shri Ram!

A K Kaul

  
  

---------- Forwarded message ---------  
From: **Todd Carnes** \<[toddc...@gmail.com]()\>  
Date: Sat, 10 Apr 2021, 04:21  
Subject: \[swisseph\] Updating to DE440/441 Planetary Ephemeris (Horizons)  
To: \<[swis...@groups.io]()\>  

  
  

I thought the group might find this interesting, especially with all the talk about Horizons in the group recently.

Todd  

  
  
-------- Forwarded Message --------

|           |                                                      | |-----------|------------------------------------------------------| | Subject:  | Updating to DE440/441 Planetary Ephemeris (Horizons) | | Date:     | Fri, 9 Apr 2021 12:57:58 -0700 (PDT)                 | | From:     | [Jon.D.G...@jpl.nasa.gov]()                          | | Reply-To: | [Jon.D.G...@jpl.nasa.gov]()                          | | To:       | [ssd-an...@list.jpl.nasa.gov]()                      |

  
  
During the week of April 12, the Horizons ephemeris system will be updated to replace the DE430/431 planetary ephemeris, used since 2013, with the new DE440/441 solution and sixteen most massive small-body perturbers.  
  
The new DE440/441 general-purpose planetary solution includes seven additional years of ground and space-based astrometric data, data calibrations, and dynamical model improvements, most significantly involving Jupiter, Saturn, Pluto, and the Kuiper Belt.  
  
For details, see "The JPL Planetary and Lunar Ephemerides DE440 and DE441", R.S. Park, et al., The Astronomical Journal, 161:105 (15pp), 2021 March.  
  
A) Impact on Horizons:  
  
For consistency with the new DE440/441 planetary solution, the catalog of 1.1 million small-body orbit solutions will be recomputed during this week using the updated perturbation model.  
  
Because it will take a number of days to complete the refit, there will be a period of time with the potential for some minor dynamical inconsistency.  
  
This means that Horizons will propagate requests for small-bodies still in the database with DE431-based solutions using the new DE441 perturber model, until the new DE441-consistent solutions execute and filter into the database.  
  
The temporary inconsistency will normally be much less than the asteroid or comet's solution uncertainties and therefore not meaningfully significant.  
  
The most visible change with this update may be ephemerides expressed with respect to the solar system barycenter (SSB), such as small-body SPK files.  
  
Inclusion of 30 new Kuiper-belt masses, and the Kuiper Belt ring mass, results in a time-varying shift of \~100 km in DE441's barycenter relative to DE431.  
  
Therefore, users of SSB-relative small-body SPK files sensitive to that level of accuracy should load in the matching planetary ephemeris for consistent calculations.  
  
B) Notes for small-body SPK file users  
  
For small-body SPK's generated prior to 2021-April-12, a DE430 planetary ephemeris should be loaded. For SPK files generated after the refit, DE440 should be used.  
  
Compatible planetary ephemeris SPK files may be retrieved here:  
  
<ftp://ssd.jpl.nasa.gov/pub/eph/planets/bsp/de430t.bsp>  
  
<ftp://ssd.jpl.nasa.gov/pub/eph/planets/bsp/de440.bsp>  
  
If you aren't sure which planetary ephemeris is needed for consistency with a given small-body SPK file, check the file comments ("commnt -r \<file_name>"). A notation like "source: SB431-N16" or "DE-0431" (or date of generation before April 12) indicates the older DE430 should be used with the SPK file.  
  
Regarding notation, DE431 is essentially a longer version of DE430 and can be used interchangeably. Similarly, DE441 refers to a longer version of the new DE440 solution.  

\_.\_,\_.\_,\_

------------------------------------------------------------------------

Groups.io Links:

You receive all messages sent to this group.

[View/Reply Online (#9687)](https://groups.io/g/swisseph/message/9687) \| [Reply To Group]() \| [Mute This Topic](https://groups.io/mt/81981896/1476078) \| [New Topic](https://groups.io/g/swisseph/post)  
[Your Subscription](https://groups.io/g/swisseph/editsub/1476078) \| [Contact Group Owner]() \| [Unsubscribe](https://groups.io/g/swisseph/leave/3311775/1476078/1955436197/xyzzy) \[[jyot...@gmail.com]()\]  

\_.\_,\_.\_,\_

