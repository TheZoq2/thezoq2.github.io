---
layout: post
title: A 3d printed split mechanical keyboard
date: 2017-03-25 15:29:20 CET
---

I recently built a split planck nechanical keyboard. This is a build log of the process
from a CAD file to a finnished keyboard.

The end result
--


The cad models
--
The first step in the process was to create a CAD model of the frame for the keyboard. I did
this using a rust library that I have written that generates openSCAD models. The library can be found (here)[https://github.com/TheZoq2/Rust-Scad]. The bevels on the edges of the
frame are done in blender because it is hard to work with edges in openSCAD.

Printing the frame
--
All the printing for this project was done on a lulzbot mini. The keycaps are printed
in white ABS while the frame is printed in PLA. The frame was relativley straight forward
to print and it would have worked on the first attempt.


Printing the keycaps
--
The keycaps were a bit harder to print. On my old keyboard I made the keycaps out of PLA
which worked fine but the surface on them was pretty rough. ABS allows you to smooth the
plastic using acetone which gives them a much nicer surface.

Actually printing the keys was a bit tricky. When I made my old keyboard, I used a different printer which, while terrible in many ways, did really well with finer details. My lulzbot
with stock configuration did alright but the surface was a lot less smooth so I had to 
do a lot more work to smooth the keys propperly. Luckily, at some point I got the idea 
of trying to use slic3r instead of cura to generate the GCODE which after a bit of tewaking
gave me some really good results.


Smoothing the keycaps
--


In the end, 3d printing keycaps is a fun project but a lot of work is required to get
the keys nice and it might be a better idea to just buy a cheap set of keycaps.



Silent switches
--
Because of previous plans to build an ergodox, I had lots of blue gateron switches
laying around. While blue switches are nice, they are not the perfect choise for 
portable keyboards that you intend to use around others. After some googling, I found
a process referd to as jailhousing the switches.

At first I used some very thin solder wire wrapped around the stem several times. However,
this wasn't consistent and would not work every time. Luckily I had some thicker solder
wire aswell which worked out a lot better.


In the end i'm happy with the way that these switches feel, they feel a bit like
browns and blues but they have a much higher actuation point. Perhaps I will grow
to dislike them in the future but for now, they are pretty good.


Wiring the electronics
--



The firmware
--
