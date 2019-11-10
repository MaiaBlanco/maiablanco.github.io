---
layout: post
title:  "Watercooled AMD 5700XT Part 1: Upgrading from GCN to RDNA"
date:   2019-11-09 22:58:00 -0400
categories: electronics gaming watercooling GPUs
---
At the time of writing this, Nvidia's RTX graphics cards have been available for several months and AMD has finally released an entirely new GPU architecture to compete - the Radeon RX 5000 series.
These are the first [RDNA](https://en.wikipedia.org/wiki/RDNA_(microarchitecture)) architecture graphics cards, which means that AMD has finally retired the [GCN (graphics core next)](https://en.wikipedia.org/wiki/Graphics_Core_Next) architecture that they have used and refined since 2012.

With a firm budget in mind and wanting better graphics performance than my current setup, I found a reference Radeon RX 5700XT on Ebay.
Normally, purchasing a reference card is a _terrible_ idea.
This is because the coolers in such GPUs have limited exhaust and a single loud blower fan (see image below). 
As the title suggests, I decided to water cool my shiny, not-quite-new 5700XT.
This sidesteps the problems of noise and heat associated with the reference cooler and gives me a fun project I can document on my site. Great!

![Reference cooler 5700XT](/images/watercooling_gpu/5700xt_top_down.jpg "Reference coolers. They look great, but sound terrible.")

This initial post will document the process of attaching an all-in-one (AIO) watercooler to the GPU. 
The approach should be general enough to apply to other current GPUs as well, both from Nvidia and AMD.
First, a necessary disclaimer: if you choose to do this sort of thing with your own (or someone else's) GPU, then the liability is entirely yours.
Simply removing the cooler on my card voided the warranty, so be aware of the risks you take when 
1. Disassembling and modifying expensive electronics
2. Introducing water-based cooling to computer hardware

Understand? Ok, then let's put some water on this card.
