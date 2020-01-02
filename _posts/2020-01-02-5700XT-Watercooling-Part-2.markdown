---
layout: post
title:  "Watercooled AMD 5700 XT Part 2: Performance and Thermal Metrics"
date:   2020-01-02 10:16:00 -0000
categories: electronics DIY computers GPU graphics performance gaming
---
### Performance delta from GCN to RDNA
[In my last post](http://www.markblan.co/electronics/gaming/watercooling/gpus/diy/2019/11/16/5700XT-Watercooling-Part-1.html), I documented upgrading my desktop's graphics card (GPU) from an older GCN (graphics core next) architecture to a modern, RDNA-based GPU: an AMD FX 5700 XT. The more interesting part of the upgrade is that I replaced the blower-fan air cooler on the 5700 XT with an all-in-one (AIO) water cooler. The water cooler was initially designed for CPU cooling, but with a 3D printed bracket, I was able to mount it to the GPU's printed circuit board (PCB). The radiator on this AIO is actually larger than the original Corsair H100 I am _still_ using for my CPU, and is very effective for cooling the new GPU.

To get a sense of both the performance improvement due to upgrading the GPU, and the improvement in cooling from installing the AIO on the graphics card, I ran Unigine Superposition. Superposition is a graphics-intensive gaming benchmark that stressed both my old and new cards to their limits. 

I ran two configurations: the medium 1080p preset, and a custom 1440p setting to max out the resolution of my monitor. Because I had to run the same benchmark on each GPU, the texture settings I ran were constrained by the amount of VRAM available on the older HD 7970 GPU. Therefore for the 1440p custom test, I set extreme shaders but only medium textures. Between tests, I allowed the GPU under test to return to a steady-state temperature.

#### Results on 1080p Medium Preset for Unigine Superposition
This first table gives the results for the 1080p medium preset. The table shows the performance in frames per second (FPS) as well as temperatures and recorded GPU utilization during the benchmark run. The fourth column shows the score given by the Superposition benchmark. Clearly, the 5700 XT performs much better than the 7-year-old 7970. The minimum FPS was improved by between 1.4x and 1.6x, depending on the cooling configuration of the 5700 XT. The maximum and average FPS improvements were at least 1.9x, and again this gets even better with GPU on water cooling. The effect of the AIO is evident in the maximum temperatures reached: on water, the 5700 XT reaches a maximum temperature near that of the _steady state, unloaded_ temperature on the original air cooler! The 5700 XT scores higher on water because it is able to maintain higher clocks and reach higher overall utilization.


| Card              	| FPS Min 	| FPS Max 	| FPS Avg 	| Score 	| Max Temp (c) 	| Max GPU Utilization 	|
|-------------------	|---------	|---------	|---------	|-------	|--------------	|---------------------	|
|  HD 7970          	| 37.40   	| 58.20   	| 45.64   	| 6102  	| 74           	| 98%                 	|
| RX 5700 XT        	| 53.35   	| 124.69  	| 86.88   	| 11615 	| 72           	| 81%                 	|
| RX 5700 XT, Water 	| 62.77   	| 133.30  	| 92.42   	| 12356 	| 54           	| 95%                 	|

#### Results on 1440p Custom test for Unigine Superposition
The second table shows the performance, thermal, and utilization metrics under the custom 1440p settings. Both GPUs have a much harder time rendering with extreme shaders at this resolution; clearly even the new 5700x XT is not up to no-holds-barred 1440p rendering. This is pretty evident since the GPUs all reach 99% utilization (reported by MSI Afterburner), where in the 1080p test the 5700 XT had more idle time. But, it is more than 2x faster than the older 7970, and with the AIO, runs much cooler and quieter to boot!

| Card              	| FPS Min 	| FPS Max 	| FPS Avg 	| Score 	| Max Temp (c) 	| Max GPU Utilization 	|
|-------------------	|---------	|---------	|---------	|-------	|--------------	|---------------------	|
|  HD 7970          	| 7.08    	| 10.02   	| 8.46    	| 1131  	| 78           	| 99%                  	|
| RX 5700 XT        	| 18.07   	| 24.54   	| 21.32   	| 2850  	| 81           	| 99%                 	|
| RX 5700 XT, Water 	| 18.38   	| 21.87   	| 25.28   	| 2932  	| 57           	| 99%                 	|


### Closing Remarks
While my chosen method of watercooling the 5700 XT is unorthodox and requires some DIY know-how and tools, the results show modest improvements in performance and greater improvements in peak GPU core thermals across both tests. All in all, it was fun to put this upgrade together and the reductions in thermals and fan noise are worth it to me.

My remaining concern is that the VRAMs are no longer directly cooled by a strip of metal from the main heatsink. However, I did affix small heatsinks to each VRAM which had thus far done a decent job of controlling memory temperatures. 
