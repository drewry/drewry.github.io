---
layout: post
title: Building My Connected Shower
modified:
categories: 
excerpt:
tags: []
comments: true
image:
  feature:
date: 2016-03-27T08:03:10-05:00
---

I recently moved into a new home with my fiancée. Of course one of the first things you do when you are unpacking and settling into a new place is plan all of your new connected home devices! Something I noticed about my daily routine was that before I could get out of bed I was spending about 15-20 minutes reading through the headlines, checking the weather, etc. Sure, part of this was simple procrastination to keep from having to get out of bed. But another part was that I didn't feel like I could start my day until I had this daily influx of information.

So I came up with the idea of having a connected smart shower. Doing so would enable me to read the headlines and get this data every morning but save me time as I could do this while showering. I wanted something that wouldn't be too distracting, something that would seamlessly integrate with the existing fixtures. But also something that I could easily read the information I wanted, when I wanted it.

![The Shower]({{ site.url }}/images/shower_pic4.jpg){: .image-pull-right}

## Brainstorming
So I started brainstorming some ideas with my fiancée for how to do this. One of our favorite features of the new house was that the shower was nice and open. Instantly we came up with the idea of using a projector to beam the information I wanted. We also thought about having a TV screen mounted somewhere, but it seemed expensive and dangerous with the moisture.

Once I figured out where the display would go it was off to the internet to find parts. I knew that I wanted the interface to be built from a website. Web technologies are usually my comfort zone, but I also wanted something that I could easily update by refreshing a page. I started looking at stick PCs like the [Intel Compute Stick](http://www.newegg.com/Product/Product.aspx?Item=N82E16883800005&nm_mc=KNC-GoogleAdwords-PC&cm_mmc=KNC-GoogleAdwords-PC-_-pla-_-Desktop+PC-_-N82E16883800005&gclid=Cj0KEQjwid63BRCswIGqyOubtrUBEiQAvTol0dvtM3XgfgQ88nhdeb4Mc1cmDvMM7KsRZdCT8yDAW5gaAhYg8P8HAQ&gclsrc=aw.ds){:target="_blank"}.

After looking at several and debating on which to go with, I ultimately decided on the [Chromebit](http://www.newegg.com/Product/Product.aspx?Item=N82E16883221147&nm_mc=TEMC-RMA-Approvel&cm_mmc=TEMC-RMA-Approvel-_-Content-_-text-_-){:target="_blank"}. It seemed like it had slightly more power for about the same price and the simplicity of Chrome OS for my purposes was appealing. I knew that I wanted to just plug it in and start configuring with a bluetooth keyboard and mouse. I've had enough issues with linux drivers incompatibility in the past that I didn't want to go through that hassle.

Next I needed a display, so I found the [cheapest, smallest projector I could find on the internet](http://www.gearbest.com/projector/pp_3252.html){:target="_blank"}. I've never used a portable projector before, I read several reviews that the display was really fuzzy for mirroring a desktop, which concerned me a little bit. But I didn't want to spend a lot of money on this project and I knew I could overcome the display issues by just making the interface simple. Afterall this was just for me and my fiancée to use -- a simple black background and white text is more than perfect for our purposes...especially for under $35!

Finally I needed a way to interact with the UI. I've been obsessed with the Amazon Echo since I first learned about it, so I knew that I wanted something voice enabled. But the echo seemed liked overkill for a simple shower interface. I found a [super tiny microphone](http://www.amazon.com/VONOTO-Microphone-Notebook-Recognition-Software/dp/B00R5O816Y?ie=UTF8&psc=1&redirect=true&ref_=od_aui_detailpages00){:target="_blank"} I could plug in to the single USB port of the chromebit. I thought maybe I could design my own echo using some combination of the webkit speech API and some backend service. Ultimately I scrapped this idea once I saw that the projector came with a remote and I could just put the interface on a timed loop.

## The Result
After standing on a chair hammering and nailing, I finally managed to get everything setup. The first issue I ran into was not taking distance into account for the size of the projected display. When I first started testing the projector I noticed it was super blurry and very small. Then I realized that I was an idiot and that I needed a decent distance in order for it to properly project.

I made some tweaks on where I would mount the projector and tested the screen resolution, tweaking the height and leveling the projector by cutting off pieces of foam for balance. After endless trial and error positioning the projector, I finally had it setup like I wanted.

![Turning on the chromebit]({{ site.url }}/images/shower_pic2.jpg)

Testing the display on the shower wall. Trying to configure a chromebit with a fuzzy display was a real challenge.

![The mounting for the display]({{ site.url }}/images/shower_pic1.jpg)

The finished mounting with some cable management. This might look beter than it actually is, there is still a good bit of electrical tape making it all stay in place :)

![First interface test]({{ site.url }}/images/shower_pic3.jpg)

My first test of the interface just outputting basic messages to see how it looks on the shower.

## Conclusion
I still have some work ahead of me. I have neglected actually connecting my interface to the API endpoints I need for the data, something I will be doing over next weekend. But I feel accomplished as the initial setup is done. Now I just need to experiment with the right timing for the interface loop and maybe working with a voice interface in the future to toggle pausing, expanding information on articles, etc.

Total cost of the project is well under $200. Here's the breakdown:

- Chromebit - $79.99
- Projector - $33.68
- Microphone (as of yet unused) - $4.99
- Mounting supplies from Home Depot - $15.00
* Bluetooth keyboard and mouse (only needed for initial setup) - $60