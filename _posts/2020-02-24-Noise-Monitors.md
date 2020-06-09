---
layout: post
title: Noise Monitors 
subtitle: Polykid project
---

# Background

I made the Noise monitors for kindergarten last time, the user only wants to know the noise and do not access the internet.

However, we are the IoT team, We should access all devices to the TTN if possible, by the way, I try to update the monitors.

## Board

I did some test with TTGO last semester and not seccess, I going to ues Feather M0 this semester beacuse our team ues this for some room sensor and easy to debug.

# Purpose

I going to update the noise monitors, there have a simply plan:

### transfter code

This is the first thing I need to do, I think it's not difficult, because the code from Arduino nano to Feather should very similar, just need to double-check the Analog and digital pins.

### set up payload in TTN

We use the payload to send data from the node(device), room-sensor use a package and co2 use an array. My one should just send a single int, I need to discuss this with Bee or Henry.

### case and board desigh

After all things work well, I going to design the board to make the whole thing look pretty, of course, I need to make it as small as possible. the small board easy to hold and can save the material when I doing the 3D print.