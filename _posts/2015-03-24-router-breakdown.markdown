---
layout: post
title: The case of the broken router
date: 2015-03-25 10:52:00 -0600
---
I bought my router when I moved in to a new place about three years ago. I wanted to make sure I got the best deal from the evil that is Charter (that actually turned out really well, which I could probably write about). I was put in charge of the internet by default because... well, no one else thought it was very important. I bought the [Motorola SurfBoard SB6121][surfboard] and the [Buffalo WHR-HP-G300N][buffalo]. The modem was about $86 and the router was about $48. I am still super happy about both of these purchases: they are kickin' ass.

I had heard about how great [DD-WRT][ddwrt] was, and I did make sure that the router I bought was able to run it. Buffalo had advertised the router as having an [open source DD-WRT base][buffalo], so I figured it had the software set up automatically.

When I booted up the router, it didn't seem too much different from any of the other routers I'd had, so I figured I'd look into it more later on. My roommates and I had issues with the router needing reboots, so I looked into it and realized that the shipped firmware was actually not DD-WRT: it was something Buffalo called the "user-friendly" version. This would obviously not do! :grin:

I flashed the firmware to the "DD-WRT (Professional) firmware" (a pretty easy affair from the web interface) and figured I wouldn't have to worry about it anymore. I was wrong! This Buffalo-provided firmware was super shitty and would need a reboot a couple times a day!

Since this was STILL not working, I thought I'd try flashing the firmware again to a DD-WRT build provided on the [DD-WRT web site][ddwrt]. Again, a menu allowed me to flash the latest DD-WRT firmware and everything was hunky-dory... for another couple minutes. Unfortunately, that particular build (I was doing this back in ~April 2012) was just really crappy for the Buffalo WHR-HP-G300N, which I unfortunately figured out after a little bit of Googling.

Last, just wanting to be done, I thought I'd try the latest updated version of the "user-friendly" firmware from Buffalo... but no. Actually, [Buffalo encrypts their firmware so you can't use the web interface to flash the firmware anymore][buffddwrt]. I had to [flash the Buffalo firmware using my Mac's TFTP client][mactftp], which took a bunch of tries an a lot of excellent timing.

Thankfully, the user-friendly firmware update proved to be stable, so there I stayed for almost 2.5 years. More on this later!

[surfboard]: http://www.amazon.com/ARRIS-Motorola-SurfBoard-SB6121-DOCSIS/dp/B004XC6GJ0
[buffalo]: http://www.newegg.com/Product/Product.aspx?Item=N82E16833162033
[ddwrt]: http://www.dd-wrt.com/site/index
[buffddwrt]: http://www.dd-wrt.com/wiki/index.php/Buffalo#Out-of-the-box:_First-time-flashing_for_.27store-bought.27_Buffalo_models
[mactftp]: http://www.dd-wrt.com/wiki/index.php/TFTP_flash#Mac_OS_X_2
