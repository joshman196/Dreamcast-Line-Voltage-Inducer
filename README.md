# Dreamcast Line Voltage Inducer PCB
PCBs designed to inject 9V into a phone line to play Dreamcast games online. It may be able to do 18V for PAL consoles/modems but this has not been tested. Comes in either a Surface Mount component PCB (tested) or a Through Hole component PCB (untested). It's intended use case is to be hidden inside of a generic RJ11 coupler with the battery snap/barrel jack coming out of a hole that you cut and is tested for this purpose, but should be able to work on the method of cutting the red wire of an RJ11 cable and soldering both sides of the red wire to the PCB.

Please note that while the Through Hole PCB should technically fit inside the case of these generic couplers, it has not actually been tested to see if it will and it is slightly larger than the Surface Mount version. The size was measured and it should fit but it may be very tight. Basically, I really had the surface mount version in mind when this was designed. The Through Hole PCB should work in terms of actually functioning correctly, though.

Yes, I'm aware the Dreamcast Live USB Modem exists and will be the go-to solution for most people. This repository exists if you just want to DIY a line voltage inducer, in case you already have a compatible USB modem or just feel like doing it for fun.

![WLwQWLT](https://github.com/joshman196/Dreamcast-Line-Voltage-Inducer/assets/114156648/7385febe-156f-481f-be75-710efa6102c5)

## Parts Required
### Surface Mount PCB
- 1x 0.47uF 50V 0805 Ceramic Capacitor - [I used this one](https://www.digikey.com/en/products/detail/samsung-electro-mechanics/CL21B474KBFNNNG/3894539)
- 1x 360 Ohm 0805 Resistor - [I used this one](https://www.digikey.com/en/products/detail/yageo/RC0805FR-07360RL/727886)
- 1x RJ11 coupler - [I used this one](https://www.amazon.com/dp/B09KX17R23?psc=1&)
- 1x Compatible USB Dial-up Modem (Dell NW147, Lenovo RD02-D400, TRENDnet TFM-561U, or a Zoom 3095)

### Through Hole PCB (Untested)
- 1x 0.47uF 50V Through Hole Capacitor - [This *should* work](https://www.digikey.com/en/products/detail/w%C3%BCrth-elektronik/860010672004/5726903)
- 1x 360 Ohm Through Hole Resistor - [This *should* work](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/CF18JT360R/1741690)
- 1x RJ11 coupler - [I used this one](https://www.amazon.com/dp/B09KX17R23?psc=1&)
- 1x Compatible USB Dial-up Modem (Dell NW147, Lenovo RD02-D400, TRENDnet TFM-561U, or a Zoom 3095)

**And either:**
- 1x 9V Battery Snap (or 2x if you have a PAL Console/Modem) - [Amazon](https://www.amazon.com/Battery-Connector-Plastic-Experiment-Equipment/dp/B08SL9X2YC)
- 9V Batteries - [Amazon](https://www.amazon.com/VONIKO-9V-Batteries-Alkaline-Battery/dp/B07RZ9PMQH/ref=sr_1_9?crid=9077FOBCDWF6&keywords=9v+battery&qid=1704714967&sprefix=9v+battery%2Caps%2C165&sr=8-9)

**OR**

- 1x 2.1mm Barrel Pigtail Cable - [I used this one,](https://www.ledsupply.com/accessories/dc-barrel-plug-pigtail-cable) make sure to select "2.1mm Female"
- 1x 9V Power Supply - [I used this one](https://www.amazon.com/dp/B0BLYS33ZP)

I have tested both a 9V battery and a barrel jack with a 9V power supply but I have not tested the 18V/2x9V batteries method for PAL consoles/modems as I do not own one. Theoretically, it should just work if you wire the batteries according to [this image](https://www.segasaturnshiro.com/wp-content/uploads/2022/06/LVI-PAL-1024x819.jpg). You can also (probably?) use an [18V power supply](https://www.amazon.co.uk/TKDY-Supply-Adapter-Electronics-Positive-Black/dp/B0BRPKVB5P/ref=sr_1_3?crid=2C0WTNA4J7N3&keywords=18v+power+supply&qid=1692327609&sprefix=18v+power+supp%2Caps%2C270&sr=8-3) with the barrel jack method as long as the barrel jack pigtails you buy are rated for at least 18V.

## Install Guide
1. Add the resistor and capacitor to the PCB.
2. Open up the coupler by pulling both sides apart.
3. Cut the red wire inside the RJ11 coupler and strip a bit of the insulation off both sides of it. You may be able to burn off the insulation with a soldering iron if you can't work well with the limited space.
4. Solder both ends of the cut red wire each to the "Red" solder pads on the PCB. It shouldn't matter which way they go.
5. Solder the 9V battery snap or barrel jack pigtail to the "+" and "-" solder pads on the PCB. Make sure you solder the red lead of the battery snap/pigtail to the "+" pad and the black lead to the "-" pad.
6. This is probably optional, but I also recommend that you wrap the PCB with kapton tape after soldering everything.
7. Cut a hole in the side of the RJ11 coupler for the battery snap/barrel jack wires to fit through. I used an off-brand X-acto Knife to cut this hole. Close/fit the coupler together after this.
8. Plug the power supply/battery into the inducer, plug your USB modem into a DreamPi (or PC, instructions later in this step), connect the phone lines from the USB Modem into your coupler, and from the other end of the coupler to your Dreamcast, turn on the DreamPi and connect your Dreamcast to the internet! If you don't have a dedicated DreamPi or any kind of Raspberry Pi to set up DreamPi on, you can use [this simple method](https://www.dreamcast-talk.com/forum/viewtopic.php?t=12731) on a PC to get online.

## Board Types/Pictures

### Surface Mount PCB (~10.287mm x ~5.207mm)
![WLwQWLT](https://github.com/joshman196/Dreamcast-Line-Voltage-Inducer/assets/114156648/7385febe-156f-481f-be75-710efa6102c5)
![20230816_221538](https://github.com/joshman196/Dreamcast-Line-Voltage-Inducer/assets/114156648/e033147f-3bba-42b8-867b-b44a83a18f96)
![20230816_221459](https://github.com/joshman196/Dreamcast-Line-Voltage-Inducer/assets/114156648/0a040784-087d-47ef-89cf-df0fc1243408)
![20230812_165747](https://github.com/joshman196/Dreamcast-Line-Voltage-Inducer/assets/114156648/a589aa6d-1d60-4130-9684-163ea989bfdc)

### Through Hole PCB (~14.224mm x ~7.112mm)
![zoSVirV](https://github.com/joshman196/Dreamcast-Line-Voltage-Inducer/assets/114156648/812123d8-5999-4744-a643-89d6e8038d44)
