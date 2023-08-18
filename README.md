# Dreamcast Line Voltage Inducer
PCBs designed to induce some voltage or something into an RJ11 telephone line to play Dreamcast games online. Comes in either a Surface Mount component PCB or a Through Hole component PCB. It's intended use case is to be hidden inside of a generic RJ11 coupler with the battery snap/barrel jack coming out of a hole that you cut and is tested for this purpose, but should be able to work on the method of cutting an RJ11 cable and soldering both sides of the red wire to the PCB.

Please note that while the Through Hole PCB should technically fit inside the case of these generic couplers, it has not actually been tested to see if it will. It may be very tight. Basically, I really had the surface mount version in mind when this was designed. The Through Hole PCB should work in terms of actually functioning correctly, though.

Yes, I'm aware the Dreamcast Live USB Modem exists and will be the go-to solution for most people. This repository exists if you just want to DIY a line voltage inducer, in case you already have a compatible USB modem or just feel like doing it because you don't care.

The text on the Surface Mount board is actually really small on the actual board, to the point that the "Red" silkscreen might not be readable in your case. You can use the picture below as a reference.
## Parts Required
### Surface Mount PCB
- 1x 0.47uF 50V 0805 Ceramic Capacitor - [I used this one](https://www.digikey.com/en/products/detail/samsung-electro-mechanics/CL21B474KBFNNNG/3894539)
- 1x 360 Ohm 0805 Resistor - [I used this one](https://www.digikey.com/en/products/detail/yageo/RC0805FR-07360RL/727886)
### Through Hole PCB (Untested)
- 1x 0.47uF 50V Through Hole Capacitor - [This *should* work](https://www.digikey.com/en/products/detail/w%C3%BCrth-elektronik/860010672004/5726903)
- 1x 360 Ohm Through Hole Resistor - [This *should* work](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/CF18JT360R/1741690)
### Both PCBs
- 1x RJ11 coupler - [I used this one](https://www.amazon.com/dp/B09KX17R23?psc=1&)

**And either:**
- 1x 9V Battery Snap (or 2x if you have a PAL Console/Modem) - [Like this,](https://www.amazon.com/Battery-Connector-Plastic-Experiment-Equipment/dp/B08SL9X2YC) but you can probably get it cheaper elsewhere
- 9V batteries duh lol

**OR**

- 1x 2.1mm Barrel Pigtail Cable - [I used this one,](https://www.ledsupply.com/accessories/dc-barrel-plug-pigtail-cable) make sure to select "2.1mm Female"
- 1x 9V Power Supply - [I used this one](https://www.amazon.com/dp/B0BLYS33ZP)

I have tested both a 9V Battery and a barrel jack but I have not tested the 18V/2x9V batteries method for PAL consoles/modems as I do not own one. Theoretically, it should just work if you wire the batteries according to [this image](https://www.segasaturnshiro.com/wp-content/uploads/2022/06/LVI-PAL-1024x819.jpg). You can also (probably?) use an [18V power supply](https://www.amazon.co.uk/TKDY-Supply-Adapter-Electronics-Positive-Black/dp/B0BRPKVB5P/ref=sr_1_3?crid=2C0WTNA4J7N3&keywords=18v+power+supply&qid=1692327609&sprefix=18v+power+supp%2Caps%2C270&sr=8-3) with the barrel jack method.
## Install Guide
1. Add the resistor and capacitor to the PCB.
2. Open up the coupler by pulling both sides apart.
3. Cut the red wire inside the RJ11 coupler and strip a bit of the insulation off both sides of it. You may be able to burn it off with a soldering iron if you can't work well with the limited space.
4. Solder both ends of the cut red wire each to the "Red" solder pads on the PCB. It doesn't matter which way they go.
5. Solder the 9V battery snap or barrel jack pigtail to the "+" and "-" solder pads on the PCB. Make sure you solder the red lead to the "+" pad and the black lead to the "-" pad.
6. This is probably optional, but I also wrap the PCB with kapton tape after soldering everything.
7. Cut a hole in the side of the RJ11 coupler for the battery snap/barrel jack to fit through. I used an off-brand X-acto Knife to cut this hole.
8. Plug the power supply/battery in, 2 phone lines for both ends of the coupler, and connect your Dreamcast to the internet! If you don't have a dedicated DreamPi or any kind of Raspberry Pi really, you can use [this method](https://www.dreamcast-talk.com/forum/viewtopic.php?t=12731) on a PC to get online. Use one of the community-recommended USB dial-up modems for this. In my case, I use a Zoom 3095 Modem, but there are others that will work.

## Board Types/Pictures

### Surface Mount
![WLwQWLT](https://github.com/joshman196/Dreamcast-Line-Voltage-Inducer/assets/114156648/10370181-e10c-40f7-9eb0-c1412f8678bd)
![20230816_221538](https://github.com/joshman196/Dreamcast-Line-Voltage-Inducer/assets/114156648/17cfb2f4-990b-4af2-bd4e-485754a6cb1d)
![20230816_221459](https://github.com/joshman196/Dreamcast-Line-Voltage-Inducer/assets/114156648/3300ed7b-8fe4-4ae7-95e4-ff06c91a18dc)
![20230812_165747](https://github.com/joshman196/Dreamcast-Line-Voltage-Inducer/assets/114156648/9d41c3ec-2efd-40a4-bd71-18f31202e9e6)

### Through Hole
![zoSVirV](https://github.com/joshman196/Dreamcast-Line-Voltage-Inducer/assets/114156648/b0443b02-31bf-4470-aa6c-f5dc69cdcb2c)
