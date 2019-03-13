---
layout: post
title:  "Repairing the Corsair 750 TX ATX Computer Power Supply"
date:   2018-07-10 22:58:33 -0400
categories: electronics repair
---
I built my first desktop somwhere between middle and high school, after struggling though games like Half-Life 2, Portal, and Team Fortress 2 on an old Dell Dimension 4770. If I remember correctly, that old machine barely supported PCIe GPUs; the other desktop I had managed to salvage from my school's tech waste required AGP cards and was not much older. The 'aftermarket' GPU I added to the system was an _ATI_ Radeon 4670, and in spite of it's own limitations was likely bottenecked by the Pentium 4 CPU and 2.5 GB of ram. To say nothing of the spinning rust that was my non-volatile storage medium...

Needless to say, when I built my first rig aroumd 2010 or so, it was a massive improvement. A quad-core (unlocked, thanks AMD!) Phenom II 955 _Black Edition_ with a whole 4GB of ram, and an AMD 5770 GPU to top things off! The PSU was upgraded of course, the very same of which is the star of this blog post...

INSERT IMAGE OF PSU HERE

This Corsair TX 750 watt PSU served the power needs for my main desktop for over 5 years, well past the end of the official warrantly offered by Corsair. Considering that in the last two of those years I was routinely using my AMD FX 8350 CPU as a room heater in my upsate New York apartment during cold winters, it did a pretty good job. 

Eventually, though, the PSU started to show signs of trouble: the odd shutdown here, needing to power cycles two or three times to have the system POST, and finally, in the words of AvE, complete failure to chooch.

#### Finding the Fault
In spite of having taken a few courses by this point in the Electrical Engineering program at my university, I have not previously debugged a power delivery circuit of this complexity before. So, off to the two best friends of alll engineers and trouble-shooters: Google and StackOverflow! Eventually, I figured out that I should check for shorted semiconductor components -- this indicates a dead diode or mosfet. Checking the active power factor correction circuit (aPFC) yeilded a shorted capacitor, a dead MOSFET, and a dead diode. Aside from these components, I also had to replace the input fuse since the failed components had caused a short from the mains inputs.

####  Working and Brighter than Ever!
Overall this repair turned out to not be too difficult to troubleshoot and repair, minus having to wait for the replacement parts to arrive in the mail. I even noticed that the PSU's cooling fan included a few slots for LEDs, which I happily soldered in! A year later, this PSU is still trucking along just fine, though I do not use it in my primary desktop since I never bothered to swap it back in. Instead it powers my home NAS. Definitely no raised eyebrows for powering an important data repository with a home-refurbished power supply... :D
