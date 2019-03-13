---
layout: post
title:  "Repairing a Corsair 750 TX ATX Power Supply"
date:   2017-03-04 21:35:29 -0400
categories: electronics repair
---
I built my first desktop somwhere between middle and high school, after struggling though games like Half-Life 2, Portal, and Team Fortress 2 on an old Dell Dimension 4770. That old machine barely supported PCIe GPU -- the other desktop I had salvaged from my school's tech waste required AGP cards and was not much older! With limited options, the 'aftermarket' GPU I added to the system was an _ATI_ Radeon 4670 (before the graphics company was owned by AMD!), and in spite of it's own limitations was likely bottenecked by the Pentium 4 and a measly 2.5 GB of main memory.

Suffice to say, the rig I built in 2010 far and away outgunned the Dell box. A quad-core (unlocked, thanks AMD!) Phenom II 955 with a *whole* 4GB of main memory, and an AMD 5770 GPU to top things off! All of this power-hungry hardware required a new PSU, the very same of which is the star of this blog post...

![PSU on the Operating Table](/images/ATX_psu_1.jpg "On the operating bench")
{:height="10%" width="10%" :class="img-responsive"}

The Corsair TX 750 served the power needs for my main desktop for over 5 years, *just* past the end of the official warrantly offered by Corsair. Considering that I was routinely my AMD CPU as a room heater during cold winters for two years, it held out pretty well.

Eventually, though, the PSU started to show signs of trouble: the odd shutdown here, needing to power cycles two or three times to have the system POST, and finally, in the words of [AvE](https://www.youtube.com/user/arduinoversusevil/videos), complete "failure to chooch."

#### Finding the Fault
![Where could that bug be?](/images/ATX_psu_inside.jpg "Where could that bug be?")
{:height="10%" width="10%" :class="img-responsive"}
In spite of having taken a few courses by this point in the Electrical Engineering program at my university, I have not previously debugged a power delivery circuit of this complexity before. So, I consulted the two best tools known to engineers and trouble-shooters: Google and StackOverflow! 

These resource guided me to check for shorted semiconductor components -- this indicates a dead diode or mosfet. Checking the active power factor correction circuit (aPFC) yeilded a shorted capacitor, a dead MOSFET, and a dead diode. Aside from these components, I also had to replace the input fuse since the failed components had caused a short from the mains inputs. 

![The fried components and their replacements](/images/ATX_psu_old_and_new.jpg "The fried components and their replacements")
{:height="10%" width="10%" :class="img-responsive"}

<!-- ![Safety while soldering - it's important!](/images/ATX_psu_safe_soldering.jpg "Safety while soldering - it's important!") -->

####  Working and Brighter than Ever!

![It's alive! And glowing!!](/images/ATX_psu_its_alive.jpg "It's alive! And glowing!!")
{:height="10%" width="10%" :class="img-responsive"}
Overall this repair turned out to not be too difficult to troubleshoot and repair, minus having to wait for the replacement parts to arrive in the mail. I even noticed that the PSU's cooling fan included a few slots for LEDs, which I happily soldered in! 

A year later, this PSU is still trucking along just fine, though I do not use it in my primary desktop since I never bothered to swap it back in. Instead it powers my home NAS. I will not comment on the wisdom of powering an important data repository with a home-refurbished power supply... :D
