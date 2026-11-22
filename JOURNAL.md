---
title: "Rapid trigger device"
github: "https://github.com/victoraloxd/rapid-trigger-keypad"
description: "A 3-key keypad with Hall Effect magnetic switches, SSD1306 OLED display, and rapid trigger algorithm"
created_at: "2026-11-21"
total_time: "4h"
---

## November 21, 2026: Project Kickoff, Component Selection & Full Schematic

Today I started my 3-key Hall Effect keypad for Hack Club Fabricate!

So this is a proyect that i've already tried to make. in this attempt im doing it from scratch again, making sure not to make the same mistakes.
im using the magnetic sensor DRV5055, a 0.92 inch Oled display (for status and dope animations!), the gateron ks-20 orange and for the brain a seeed studio XIAO rp4020
today i´ve searched for the footprints and schematics of the components im using, i learnt that the sensor DRV5053 is unipolar, meaning that if the magnet poles on the switches are inverted the sensor will not be able to register any data. so i found another version of it the 5055 tha in bipolar and doesnt have that problem.
i decided to use de xiao rp4020 because the chip runs at 133mhz with a dual-core processor and fast 12-bit ADC. so i can achieve pretty high polling rates like 1000hz and above if im using USB HID making sure that the rapid trigger firmware feels responsive and instant. Also it is really tiny, which allows me to build a small, compact and portable device. In addition, because it has native usb support its very comfy to work with taking in count that im not that used to program.

then i got started on the scematics, after conecting all the components it whas looking messy, so i ask gemini on some advice and then i got a much better result (that im proud of)
![](https://cdn.hackclub.com/01a20145-b637-7224-a467-01c1a8930014/Captura%20de%20pantalla%202026-11-21%20222055.png)
also i had like 9 errors that where kicad pinpointing at the non-connected pins on the xiao rp4020.
Total time spent: 4h

