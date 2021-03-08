---
layout: post
title:  "Espresso Adventures: Repairing Expobar Brewtus IV - Part One"
date:   2020-12-21 22:48:00 -0400
categories: electronics DIY coffee espresso
---
#### Introducing the Brewtus IV:
This is the first of a series of entries detailing repairs I have made to an Expobar Brewtus IV.
Expobar is a Spanish company that manufactures "prosumer" espresso machines.
The Brewtus IV is a model sold by Whole Latte Love, a US company.

![The Chrome Coffee Behemoth](/images/expobar_post_1/chrome_behemoth.jpeg "The Chrome Coffee Behemoth"){:class="img-responsive"}

I discovered this chrome behemoth at the office kitchen, mothballed and nonfunctional.
What was my immediate decision as a caffeine-dependent PhD student?

Pull out a Swiss Army Knife and fix it, obviously!

Here's a look from the top at the insides. On the top of the image, you see two boilers. The one on the right is the brew boiler, whose temperature is controlled by a PID unit. On the left is the steam boiler, whose pressure (not temperature, directly) is controlled by a pressurestat. This second boiler is the one acting up.

![copper guts and glory](/images/expobar_post_1/copper_guts.jpg "complex looking, and yet simple."){:class="img-responsive"}

#### The symptoms:
Whenever the machine begins brewing an espresso, the boiler's overpressure valve hisses with a violent release of heat and steam. Due to the water released within the machine, a short circuit occurs and trips the in-wall circuit breaker.
No caffeine from this machine!

#### On investigation: 
Water enters the machine at the pump inlet, which pushes water into one of two boilers - steam or brew.
A problem: the solenoid valve and inlet pipes (called the labyrinth) for each purpose both appear to feed into the steam boiler! 
How aptly named. 

Below is a photo of the labyrinth, which threads into the bottom of the steam boiler. 
The small silver port at the bottom of the image is the inlet.
The path splits at a T-joint, which then feeds directly into the steam boiler (lower left), and also through a curved copper tube again into the steam boiler (upper left).

![Welcome to the Labyrinth](/images/expobar_post_1/welcome_to_the_labyrinth.jpg "The labyrinth feeds water into both boilers, but water for the brew boiler first passes through a head exchanger tube in the steam boiler."){:class="img-responsive"}

That the labyrinth feeds into only the steam boiler turns out to be by design - water destined for the brew boiler first runs through a channel in the steam boiler, sealed from the rest of the water being used for steam.
This pre-heats the brew water before it reaches the boiler, keeping thermals stable for extraction! Neat!

This piping arrangement leaves two possibilities for the overpressure condition during brew extraction.
First, the heat-exchange tube in the steam boiler coudl be leaking brew water into the surrounding steam boiler.
Second, the solenoid valve that isolates the brew feed from the steam feed may not be sealing properly.
Either way, the steam system is exposed to the the brew boiler's pressure.
This points to a compromise in isolation of the two water systems. 

#### Possible Solutions: 
Fixing a leak in the heat exchanger would require brazing the inside of the boiler - after finding the point of leakage.
Replacing the solenoid would be much easier.
In either case, I set about disassembling the machine to know more.

Post-deconstruction, I bathed each component in a combined solution of diluted vinegar and espresso machine descaler. 
Descaler is typically citric acid and some other acidic chemicals, so overall it's basically just a mild acid bath.
I found no obvious defects within the steam boiler, and no electrical issues in the solenoid switching.
Drawing a blank, I rinsed each component and reassembled.

Not knowing what to try next, I decided to test pulling a shot.

Lo and behold...it worked. What?

At this point, my best guess was that the solenoid valve had built up some scale, which caused an improper seal when it was supposed to be closed for brew mode.
Cleaning with descaling solution got rid of the scale, letting the valve seal again.

As of May 2019, the Expobar pulled countless shots of espresso for PhD students in the office...a majority of which I consumed. 

On to research and caffeine!
