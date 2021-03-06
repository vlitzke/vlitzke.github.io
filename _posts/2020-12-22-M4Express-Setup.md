---
title: "Feather M4 Express Set-up"
author: Vivienne
date: 2020-12-21
layout: post
icon: fa-wrench
---

Yesterday my supervisor handed me parts to start building our own dataloggers, which included a Feather M4 Express Board, Accelerometer and GPS with associated cable wires, LED lights and so on from [Adafruit](https://www.adafruit.com/product/3857).

I downloaded Arduino [here](https://www.arduino.cc/en/software), then the additional boards manager which led me to Arduino SAMD Boards and Adafruit SAMD (check out the User Manual for the Feather M4 Express board. So far so good. Then I tried to download the Adafruit Board Driver, but Feather M4 Express was not there (tried two versions, adafuit_drivers_2.5.0.0 and 2.3.4.0 to make sure nothing got lost along the way, still nothing). I can select my board, but not the port, it is greyed out.

Laptop having issues recognizing the board when it is plugged into the USB port. I have tried several things, to no avail:
1. From [this forum](https://forum.arduino.cc/index.php?topic=424879.0), I downloaded the CH340g driver (as per this [cloning comment](https://forum.arduino.cc/index.php?topic=619090.0)).

2. Went to my device manager, manually downloaded ports (for COM7) downloaded both the COM7 port and the Adafruit circuit playground per this [thread](https://www.windows10forums.com/threads/ports-com-and-lte-not-showing-in-device-manager-in-windows-10.6057/).

3. Perhaps its the cable? see the first comment [here](https://www.thingsconnected.io/arduino-studio-com-port-grayed-windows-resolved/). According to Bob, *some USB cables have been made only for charging purposes and are missing the signal wires*. 

Also see [this](https://learn.adafruit.com/adafruit-feather-32u4-basic-proto/feather-help#faq-3): *A vast number of Itsy/Feather 'failures' are due to charge-only USB cables. We get upwards of 5 complaints a day that turn out to be due to charge-only cables! Use only a cable that you know is for data syncing. If you have any charge-only cables, cut them in half throw them out. We are serious! They tend to be low quality in general, and will only confuse you and others later, just get a good data+charge USB cable*

Problem solved!!! It was the cable. 
