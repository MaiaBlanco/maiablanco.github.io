---
layout: post
title:  "Espresso Adventures: Repairing Expobar Brewtus IV - Part One"
date:   2020-12-21 22:48:00 -0400
categories: electronics DIY coffee espresso
---
My relationship with coffee hasn't always been so...passionate. 
I drank tea in college, sometimes for the caffiene, 
more often as a defense against cold New York winters.
I once tried Keurig coffee;
I found the taste lacking and did't appreciate the caffeine kick.

Well, things have changed.

I started a PhD in 2017, and almost immediately began to develop a coffee --addiction-- --habit-- *obsession*.
So it goes, I suppose.

Enter the Expobar Brewtus IV:
![Itty Bitty Heat Sink](/images/8350_VRM_Cooling/tiny_heatsink.jpg "Tiny heatsink on VRMs")
{:height="10%" width="10%" :class="img-responsive"}

I discovered this chrome behemoth in the office kitchen, mothballed and nonfunctional.
What was my immediate action as a caffiene-dependent PhD student?

Pull out a Swiss Army Knife and figure fix it, obviously!

[][]PHOTO OF EXPOBAR INSIDES

The symptom: whenever the machine begins brewing an espresso, the boiler's overpressure valve hisses with a violent release of heat and steam.
No caffeine from this machine!

On investigation: 
Water enters the machine at the pump inlet, which pushes water into one of two boilers - steam or brew.
A problem: the solenoid valve and inlet pipes (called the labyrinth) for each purpose both appear to feed into the steam boiler! 
Aptly named.

This turns out to be by design - water destined for the brew boiler first runs through a channel in the steam boiler, sealed from the rest of the water being used for steam.
This pre-heats the brew water before it reaches the boiler, keeping thermals steady for extraction! Neat!

This piping arrangement leaves two possibilities for the overpressure condition during brew extraction.
First, the heat-exchange tube in the steam boiler coudl be leaking brew water into the surrounding steam boiler.
Second, the solenoid valve that isolates the brewt feed from the steam feed may not be sealing properly.
Either way, overpressure on the steam system when the brew boiler is under pressure points to a compromise in isolation of the two water systems. 

Possible Solutions: 
Fixing the heat exchanger would require brazing the inside of the boiler - after finding the point of leakage.
Replacing the solenoid would be much easier.
In either case, I set about disassembling the machine to know more.

[][]PHOTO OF PIECES

Post-deconstruction, I cleaned each component in a combined solution of diluted vinegar and espresso machine descaler. 
I found no obvious defects within the steam boiler, and no electrical issues in the solenoid switching.
Drawing a blank, I rinsed each component from the solution and reassembled it.

Not knowning what to try next, I decided to test pulling a shot.
Lo and behold...it works. What?

At this point, my best guess was that the solenoid valve had built up some scale, which caused an improper seal then shut for brewing.
As of May 2019, the Expobar pulled countless shots of espresso for PhD students in the office...a majority of which I likely consumed. 

On to research and caffiene!
