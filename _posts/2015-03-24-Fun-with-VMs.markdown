---
layout: post
title: Discovering my virtual machine
date: 2015-03-25 07:03:00 -0600
---
I downloaded a copy of the Ubuntu 14.04 LTS Server edition a while ago. I thought it might help give me some Linux chops so that I could play around with setting up my old 2010 Mac Mini as a server. I had looked into a bunch of possibilities, and it seemed like there was a fair amount of problems with getting all of the components to work with Ubuntu [unless it was using 10.04][maverick].

I'd also eventually like to have a media PC that could be my Plex server. I'm not completely sure, but I think the Mac Mini processor won't quite be strong enough to do a even one fully encoded 1080p stream.

Anyway, I installed the server edition as an Oracle Virtual Box maybe at the beginning of February. I didn't really do much with it, because I didn't really have any idea what I might be able to do with it. I didn't even know if the thing could connect to the internet correctly... and at first, it couldn't. I didn't know how I should be thinking about it. I figured that because it was a virtual machine, it wouldn't really be able to connect to the internet like a normal PC.

I WAS SO WRONG! The GREAT thing about putting the internet adapter into "Attached to: Bridged adapter" mode is that now, it really just functions like a Linux box attached to my router somewhere (oh man, that reminds me: I have to write about OpenWRT). The router gives it an IP just like any other computer. NAT mode makes it the only client in an entirely new subnetwork, such that you'd need to add a whole bunch of new routing rules in order to access it from somewhere else. I think I tried a bunch of different ways of configuring the adapter a month or two ago and completely gave up.

A whole new computer and operating system! Sitting there, ready for me to play with and configure!
