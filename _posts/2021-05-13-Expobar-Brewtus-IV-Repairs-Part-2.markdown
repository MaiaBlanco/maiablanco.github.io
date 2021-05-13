---
layout: post
title:  "Espresso Adventures: Repairing Expobar Brewtus IV - Part Two"
date:   2021-05-13 15:50:00:00 -0400
categories: electronics DIY coffee espresso
---

In the previous post I introduced the Expobar Brewtus IV - a behemoth 
espresso machine that was in my workplace office in 2019. 
In the fall of 2018, I got the machine to brew again without issues.

The machine worked for another semester and a half, failing sometime 
in the summer of 2019.
As I was away during this summer, I found out that the machine 
had broken down when I returned in the Fall. 

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

An aside: As opposed to debugging more complex electronics such as 
computer power supplies, debugging an espresso machine is 
more straightforward.
Components are not as small and electrical components 
tend to be fairly simple relays, thermistors, and resistive 
heating coils. 
There are no diodes or mosfets in the internal circuitry, save for 
the PID controller.
The PID controller for the brew tank 
involves some closed-source circuitry but is self-contained 
and in my experience less likely to fail than other components 
in the espresso machine.

In testing for shorts, I discovered that the heating element for the 
brew water tank was shorted to the tank itself. 
Since the entire tank is meant to be grounded, as soon 
as mains voltage flowed to the heating element connectors, 
it shorted to ground and shut down the machine.

This is a simple equipment failure, but is difficult to do without 
the right tools. 
The replacement heating element is stocked by Whole Latte Love,
the company that partnered with Expobar to design the Brewtus IV.
This element costs ~$80, but the most difficult aspect if this repair 
is removal of the old heating element.
I purchased a 1/4" impact driver and a 1 and 7/16" socket as 
specified in the service instructions provided by WLL.
Try as I did, the shorted heating element was stuck fast in the 
brew boiler.

In retrospect, the best option is to take the boiler out 
of the espresso machine and bring it to an automotive repair
shop.
This is what I ended up doing, and in mere seconds the heating 
element was removed from the boiler.
While the documents provided by WLL suggest an oil filter 
wrench to hold the boiler as you drive the heating element 
out, this is not necessary if you have a professional-grade 
(read: powerful) impact driver. 
You can hold the boiler in hand as the impact driver doesn't 
use sustained, but instead breif and intense peak torque 
to loosen and remove the element.

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

In my case, I used Loctite 





https://www.home-barista.com/espresso-machines/tips-on-replacing-expobar-office-boiler-heater-other-things-to-do-at-same-time-t37990.html
https://www.home-barista.com/repairs/brew-boiler-leak-and-threadlocker-t13677.html
