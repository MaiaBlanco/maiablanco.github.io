---
layout: post
title:  "Watercooled AMD 5700XT Part 1: Upgrading from GCN to RDNA"
date:   2019-11-09 22:58:00 -0400
categories: electronics gaming watercooling GPUs
---
### Introduction
At the time of writing this, Nvidia's RTX graphics cards have been available for several months and AMD has finally released an entirely new GPU architecture to compete - the Radeon RX 5000 series.
These are the first [RDNA](https://en.wikipedia.org/wiki/RDNA_(microarchitecture)) architecture graphics cards, which means that AMD has finally retired the [GCN (graphics core next)](https://en.wikipedia.org/wiki/Graphics_Core_Next) architecture that they have used and refined since 2012.

With a firm budget in mind and wanting better graphics performance than my current setup, I found a reference Radeon RX 5700XT on Ebay, relatively below MSRP.
Normally, purchasing a reference card is a _terrible_ idea.
This is because the coolers in such GPUs have limited exhaust and a single loud blower fan (see image below). 
As the title suggests, I decided to water cool my shiny, not-quite-new 5700XT.
I expect this to mitigate the noise and heat associated with the reference cooler, and doing this gives me a fun project I can document on my site. Hooray!

![Reference cooler 5700XT](/images/watercooling_gpu/5700xt_top_down.jpg "Reference coolers. They look great, but sound terrible.")
This post will document the baseline performance improvement from replacing the
card, as well as thermals for the reference 5700XT card above. 
Then, I'll detail the parts and process I used to water cool the card, and then
report any improvements in performance and thermals I observe.
This approach should be general enough to apply to other current GPUs as well, both from Nvidia and AMD.

### Disclaimer
First, a necessary disclaimer: if you choose to do this sort of thing with your own (or someone else's) GPU, then the liability is entirely yours.
Simply removing the cooler on my card voided the warranty, so be aware of the risks you take when:
1. Disassembling and modifying expensive electronics
2. Introducing water-based cooling to computer hardware

Understand? Ok, then let's put some water on this card.

### Performance delta from GCN to RDNA
TODO: add table of superposition FPS

### Baseline Thermals on the 5700XT
add table of 5700 XT superposition thermals


### Watercooling
Watercooling GPUs seems to be gaining popularity as of late. 
The initial inspiration for this project came to me when I got ahold of an
extra Corsair H100i AIO cooler. I didn't need it for my CPU, but thought it
might work well on a GPU. 
With a quick web search I found that companies like Corsair and NZXT already
sell (or used to sell) metal brackets for adapting the mounting holes on
graphics cards to those on their own AIO coolers. 
But, with a Radeon HD 7970, pushing 7 years, I didn't think it would be worth it to get into watercooling for the card.


Some months later, I found this post on Reddit. It turns out that not only do
brackets exist, but so do AIO water coolers specifically for GPUs!
Better yet, 3D-printed brackets exist (such as this one) that I can print at
a fraction of the cost of either of the two premade options above.
My interest was rekindled, and I started collecting and printing parts to make this
project happen.

#### Watercooling Components
First, the 3D-printable bracket referenced in the link above. It is designed to
mesh with the gear-tooth style of mounting that some Corsair and ???? AIOs used
to use.

TODO: image of bracket here.


Then, an AIO cooler. For this I found a 240x120mm H105, but I think a 120x120mm
radiator would work just as well. The H105 was the specific one I chose because
it has the gear-tooth mounting scheme compatible with the bracket I printed.


Finally, a GPU on which to test. That's the reference 5700XT from the beginning
of this post.
Some additional components I needed were:
1. M3x30mm machine screws for mounting the cooler, with associated nuts and
			washers.
2. Small heatsinks for putting on the GPU memory units. Since this mod removes
			the main source of airflow and the original heatsink, the memories need new
heatsinks to have area for dissipating heat. 
3. Thermal tape and thermal paste for attaching the mini heatsinks and for
			putting between the GPU die and AIO, respectively.

These additional components can be found fairly easily online.

#### Removing the Reference Heatsink
Removing the reference heatsink from the 5700XT primarily involved removing
many screws. The first item that had to come off was the back plate and the
x-bracket on the back of the card that actually holds the heatsink in place
against the GPU die.

Next, additional screws holding the shroud and the blower fan onto the GPU
circuit board had to be removed. I also had to detach the PCIe bracket from the
display output ports, since it had one or two screw attaching to the shroud as
well.
With these all removed and with a bit of careful prying, the entire assembly
comes apart (below). 

TODO: open-faced GPU sandwich

Interestingly, this reference card does not use thermal paste for the GPU die!
Instead, there is a thermal pad in the center of the heatsingk that appears to 
be made of a rougher, less rubbery material than the surrounding thermal pads
for memory units, VRMs, and other components. Perhaps simply replacing this
with better thermal interface material would have improved the thermals for
this card.

Next, I mounted the AIO with the bracket I had printed, making sure to apply
a dab of loctite to each bolt and nut holding the AIO in place....
Perfect! Right?

TODO: photo of first try

And that's where I made a mistake. I was so busy making sure that no screws
would come loose, that I didn't check how the solvent that loctite comes in
would react with the ABS plastic of my bracket. The result? The bracket became
brittle and shattered:

TODO: shattered bracket.
 
As an interesting aside: you can see from the two side-by-side images below
that the damage caused by the lotite solvent is distinct from damage caused by
mechanically snapping the ABS bracket. 
When I bend the bracket by hand, the plastic turns white at the break, while
loctite left the bracket smooth with no color changes.


At any rate, I had to print a new bracket, and remounted the AIO making sure to
_avoid_ loctite, at least for the time being.

TODO: final mounting. 


#### Mounting the AIO


#### System Installation


### Watercooled Thermals


### Conclusions


