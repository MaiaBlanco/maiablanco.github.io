---
layout: post
title:  "Espresso Adventures: Repairing Expobar Brewtus IV - Part Two"
date:   2021-05-13 15:50:00:00 -0400
categories: electronics DIY coffee espresso
---

#### Introduction ####
In the previous post I introduced the Expobar Brewtus IV - a behemoth 
espresso machine that was in my workplace office. 
In the fall of 2018, I found it inoperative and with some careful
disassembly got it to brew again without issues.

The machine worked for another semester and a half, failing sometime 
in the summer of 2019.
As I was away during this summer, I found out that the machine 
had broken down when I returned the following Fall. 

#### Symptoms ####
The symptoms of this latest problem were simple:
when the machine was turned on, it instantly tripped the 
circuit breaker. 
It was clear that there was a short circuit somewhere in 
the machine.

I began by testing for short circuits with a multimeter.
Basically, no electrical connection in the machine should 
have a direct short leading to the chassis ground.
Therefore if the multimeter detects zero resistance from any 
electrical connection to the casing, copper piping, or brew tanks,
then the root cause is nearby.

>An aside: As opposed to debugging more complex electronics such as 
>computer power supplies, debugging an espresso machine is straightforward.
>Components are not as small and electrical components 
>tend to be fairly simple relays, thermistors, and resistive 
>heating coils. 
>There are no diodes or mosfets in the internal circuitry, save for 
>the PID controller.
>The PID controller for the brew tank 
>involves some closed-source circuitry but is self-contained 
>and in my experience less likely to fail than other components 
>in the espresso machine.

In testing for shorts, I discovered that the heating element for the 
brew water tank was shorted to the tank itself. 
Since the entire tank is meant to be grounded, as soon 
as mains voltage flowed to the heating element connectors, 
it shorted to ground and shut down the machine.

In the end, I was looking at replacing the element whose hex-socket 
bottom you see in this photo:
![They make sockets this big??!!](/images/expobar_post_2/large_hex_socket.jpg "Very Large Hex Socket (tm)."){:class="img-responsive"}

This is a much larger hex socket than I've seen working on my car, so I bought a 
hex head and a cute little refurbed impact driver for the job.
The replacement heating element came from WholeLatteLove.com.
![The impact driver is too small...](/images/expobar_post_2/huge_socket_tiny_impact_driver.jpg "Huge socket, tiny impact driver."){:class="img-responsive"}
>A word from the future: that impact driver is too small!


#### The Fix: Removing the Borked Element ####
This is a simple equipment failure, but is difficult to do without 
the right tools. 
The replacement heating element is stocked by Whole Latte Love,
the company that partnered with Expobar to design the Brewtus IV.
This element costs ~$80, but the most difficult aspect if this repair 
is removal of the old heating element.
I purchased the 1/4" impact driver and a 1 and 7/16" socket as 
specified in the service instructions provided by WLL.
I even bought a fancy oil filter wrench (in the photo below) and later 
a breaker bar.
Try as I did, the shorted heating element was stuck fast in the 
brew boiler.

![You're gonna need a bigger boat, er, driver!](/images/expobar_post_2/removing_heat_element.jpg "You're gonna need a bigger boat, er, driver!"){:class="img-responsive"}

In retrospect, the best option is to take the boiler out 
of the espresso machine and bring it to an automotive repair
shop.
This is what I ended up doing, and in mere seconds of applying 
their full-sized impact wrench the heating 
element was removed from the boiler.
While the documents provided by WLL suggest an oil filter 
wrench to hold the boiler as you drive the heating element 
out, this is not necessary if you have a professional-grade 
(read: powerful) impact driver. 
You can hold the boiler in hand as the impact driver doesn't 
use sustained, but instead brief and intense peak torque 
to loosen and remove the element.

Later, the element in the steam boiler shorted and I had to visit the same
auto shop to remove that one as well.
The build-up of mineral scale on the two old elements (middle and right) is obvious in the photo below, 
but it's not obvious why they shorted. 

![Side by side of new and old elements.](/images/expobar_post_2/compare_old_elems.jpg "Some scaling build up, but no obvious reason for shorting."){:class="img-responsive"}


#### The Fix: Re-Sealing the Boilers  ####
It is clear that Expobar designed the heating elements 
on the Brewtus IV to use some sort of thread sealant, 
with no gasket.
Searching on online forums makes it clear that 
most prosumer espresso machines are now designed 
with gaskets and possibly also sealant, rather than only sealant.
Further searching reveals some controversy over what 
thread sealants to use, given that not all are safe for 
contact with water at the >100 c operating temperatures of 
a boiler.
Some forum posters suggest using Teflon tape (PTFE) instead 
of sealant, while others favor sealant because it can be easier
to remove for future repairs.

In my case, I used [Loctite 567](https://www.henkel-adhesives.com/us/en/product/thread-sealants/loctite_567.html) to seal the boiler heating element. It is rated as food
safe up to...just below the target temperature of the boilers.
Not ideal, but it's really hard to find something better.

I ended up using this sealant and carefully applying it to leave the innermost 
threads bare, to avoid getting too much in the boiler.
After letting the sealant 'cure' for days outside of the espresso machine, 
I flushed a lot of water through the brew and steam systems.

It still took some time for me to have confidence that the water in the machine was uncontaminated.
In particular, steam from the steam boiler tended to have an odd smell for some time 
until it subsided.

The upshot of using this sealant is that it's advertised to remain workable after application.
So, next time an element goes bad, I can more easily remove it with my tiny impact driver 
instead of going to an auto shop.


#### Conclusions ####
This was a pretty involved repair that required me to buy some new tools, most of which were
insufficient for the job. 
I read nearly the entire Loctite catalog to find a 'safe' sealant and quite a few online forum threads of other espresso enthusiasts before settling on a sealant that seemed acceptable. 

For all this effort, the machine is running pretty smoothly now.
There is a slight leak at the brew heating element, so I will eventually need to 
remove and re-seal that one. When that time comes I'll try teflon tape, as I think it will be safer for the water and my health.

In a future post, I'll detail a design flaw in the brew temperature regulation of the 
Brewtus IV and how I resolved it. Not to fear, the machine is still running and brewing
delicious espressos.

#### References ####
- [https://www.home-barista.com/espresso-machines/tips-on-replacing-expobar-office-boiler-heater-other-things-to-do-at-same-time-t37990.html](https://www.home-barista.com/espresso-machines/tips-on-replacing-expobar-office-boiler-heater-other-things-to-do-at-same-time-t37990.html)
- [https://www.home-barista.com/repairs/brew-boiler-leak-and-threadlocker-t13677.html](https://www.home-barista.com/repairs/brew-boiler-leak-and-threadlocker-t13677.html)
