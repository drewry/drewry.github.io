---
layout: post
title: Returning to Windows, Well Not Quite
modified:
categories: 
excerpt:
tags: []
comments: true
image:
  feature:
date: 2016-04-10T18:22:22-04:00
---

About a week ago I decided it was time to build a gaming PC and thus return to Windows. I started working on an Unreal Engine 4 project in my spare time and I needed something powerful enough to handle all of the intense graphics of modern gaming. Throughout this process I made note of a few things that really surprised me: 

0. How cheap PC parts have become these days. I was able to get all of my parts for under a grand allowing me to meet and surpass the system requirements I will need for my game development.
0. How insanely difficult it is to work with Windows... __still__.
0. Fry's is still awesome.

![The Juggernaut]({{ site.url }}/images/the_juggernaut.jpg)

## Procuring Parts
I was already off to a good start as a friend of mine gave me a cool master case that he had for an old gaming PC. Once I dusted off the case, it was time to upgrade everything else.

Here are the parts I found:

* ASUS Z170 Pro Gaming Motherboard: __{% raw %}<strike>$169.99</strike>{% endraw %} $159.99 after rebate__
* GTX 950 Gaming 2G video card: __{% raw %}<strike>$174.99</strike>{% endraw %} 164.99 after rebate__
* Intel i5-6600 processor: __$239.99__
* 16 GB DDR4 RAM: __$134.99__
* 2 TB hdd: __$129.99__
* AC 1300 mb/s wireless networking card: __$59.99__
* Existing power supply
* Existing case with 6 fans
* Windows 7 Professional: __$120.00__

__Total cost: $874.95__

Rebates are still a pain in the ass, I had to get the receipt, cut off the original serial number from the box and physically print the form, sign it and snail mail everything.

## Installing Windows
I opted to get Fry's to connect all of the parts and test them for an additional $49.99. It was worth it to me as I wasn't fully sure that the power supply was still good and I wanted to get everything tested in one spot. That way if anything needed to be replaced it would already be where I would get the parts. That and moving the thing to and from the car was enough to nearly break my back.

As soon as I got home, as I hoped, it turned right on. No BIOs issues, parts exploding, nor any other catastrophic issues -- thank you Fry's. Now to get my fresh copy of Windows installed! But oh wait it's on a CD, crap I didn't even think about a disk drive! Ah yes, Compact Disks, those mystical plastic disks that once used to be the key to my favorite childhood games. Of course the original disk drive for the case didn't work with the new motherboard. I thought to myself, "Okay, no worries, it's 2016! Certainly I should be able to install Windows with a flash drive or an external drive or __literally__ anything other than a CD, right?"

So I was off to Google to look through how to do it. Some tutorials involved 10-15 steps and all of them appeared to use a completely different approach. After looking for a while I found a video on youtube that just required a quick format, copying some files and booting. Seemed easy enough, the video was only 3 minutes so it coudln't be that hard. So I booted up the PC and the Windows installation screen loads.  "Awesome! That was easy," I thought to myself. But then I get to step 2...

![A required CD/DVD driver is missing.]({{ site.url }}/images/windows.png)

What does that even mean Microsoft?! I'm not using a CD/DVD so why would I need a driver for it, why can't you recognize I'm installing from a flash drive?! After I calmed down a bit, I found a resource saying that the mounting of the flash drive was done improperly... Well I didn't actually mount it the first time, I just copied files. So I thought that maybe by taking the easy way out I screwed it up somehow. So I downloaded an ISO mounting tool and mounted it to the drive this time. I booted it up and tried again...same damn message!

I kept looking through more forums of people saying to just take the drive out and put it in another USB port, no luck. I tried mounting it with the official tool from Windows, still no luck. I'm really frustrated at this point and on the brink of admitting defeat. Then, as I'm sitting exhausted and distraught in my office chair I look over to my old computer just sitting there. Sitting there with a working (and fairly modern) CD/DVD drive. "Yes, that will work," I shouted to myself. So I pop open the case, remove the drive, and put it in the new PC. The drive works immediately and I put the CD in and finally get passed the second screen.

## Final Thoughts
Now I was ready to install the rest of my software. Most of the installations go okay. However, I have a tough time getting all of the drivers to play nicely. Visual Studio's installation froze and crashed on me 3 different times. The PC on rebooting decided to update 125 updates, during which it had a failure and had to revert everything. After roughly 2 days of trying to get everything setup in my spare time I was in utter disbelief at how bad the Windows ecosystem __still__ was. As a Mac user for the better part of this decade I was blown away at the user experience on Windows.

I really should have known better, as I grew up a Windows user. These kinds of frustrations were the day-to-day norm, so I guess you could say in some ways all of the bugginess was nostalgic. But after this I realize how spoiled I have been by Apple's grade of quality, and many mac users today will tell you that Apple's software quality has gone down considerablly -- which it has.  But it is no where near as bad as Microsoft.

I feel bad saying that, but it is true. I feel bad because I want to believe in Microsoft. I want to believe that the future is bright for Windows. Partly because I'm going to be doing a lot more work on my Windows machine. But also because I'm really excited about augmented reality, virtual reality and everything in between. And I know that the best way to develop for these technologies will be on a Windows machine. 

In all fairness my use case was not that of the typical consumer and everything is generally running pretty smoothly now -- after turning off all of the default settings. And I truthfully do love my Windows machine, who I affectionately named __The Juggernaut__. I love its power and the fact that every game I could ever want to run is available to me. I do love the ability to customize just about everything, from the parts to the end user experience. I guess with that you lose some of the sleekness and simplicity that Apple gives and in exchange you receive many late nights with headaches and the feeling of hopelessness and despair. Too bad those are our choices, I guess there's always Linux :)