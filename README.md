
# README Laser Cutter

## Quick start
  1. 
    * Turn machine on and use the arrow keys on the machine to move the cutting head to the back right corner
    * Decide if you should use the knife bed or honnycomb bed 
    * REMEMBER TO ADJUST THE Z-HEIGHT TO THE CHOSEN CUTTING BED SO YOU DON'T RAM THE CUTTING HEAD AGAINST THE BED!
    * Put in your material (use only MDF, acrylic or cardboard for beginners) 
    * Move the cutting head to somewhere smooth an even on your material
    * Use the autofocus feature to set the z-height.
  2. 
    * Use LightBurn software to handle your cut file. 
    * choose cut/engrave settings for each layer in LightBurn 
    * Press the send button in lightburn to send the file to the cutter
  3.  
    * press the file button the the lasercutter and choose your file (usually the first on the list) 
    * Use the arrow keys on the lasercutter to move the cutting head to where you want to cut 
    * press the frame button to see where the laser intends to cut 
    * Close the lid 
    * start ventilation, pump and laserpower
    * Press start on the lasercutter
  4.  
    * DO NOT LEAVE THE LASERCUTTER UNATTENDED. 
    * STAY AND KEEP AN EYE THAT EVERYTHING IS OK THROUGHOUT THE WHOLE CUT.
    * DO NOT OPEN THE LID IMMEDIATELY AFTER THE CUT HAS FINNISHED.
    * WAIT AT LEAST 15 SECONDS FOR THE FUMES TO BE SUCKED OUT
  5.  
    * Turn off laserpower, ventilation and pump and then finally the machine.

___

## Material safety
The CO2 laser in the machine can cut most organic materials and plastics, but there are some dangerous ones. If you are unsure if something can be cut, ask first.

Safe to cut:

  * Woods 
  * Cardboard/ paper
  * Acrylic

DO NOT CUT any of these:

* PVC, Vinyl
* ABS
* HDPE
* Fiberglass, PCBs
* Carbon fiber
___

## Tuning the parameters
### Cutting
For cutting the basic parameters are speed, power and number of passes.  
In most cases power can be left at 100% and the speed can tweaked so the material is cut all the way through.  
If the material is so thick that it needs a speed below 10 mm/s consider cutting it in 2 passes.  

### Engraving
For engraving there are a number of parameters that affect the outcome:  
Speed and power together define the amount of laser energy that hits a unit of surface.  
Line interval specifies the distance between the individual engraving lines. Reasonable values: 0.05 superfine, 0.1 fine, 0.2 draft  
Z-offset defocuses the laser to make the spot wider. Don't forget that if the spot is wider, more power is required. DO NOT use positive values for Z-offset as the laser head will hit the bed. Recommended values for a given line interval:

| Line interval | Z-offset   |
| ------------- | ---------- |
| 0.05mm        | 0 to -4mm  |
| 0.1mm         | -2 to -6mm |
| 0.2mm         | -6 to -8mm |

___
## FAQ/common fixes
The corners, tips, small details of a cut/engraving are not cut through/weaker

* Try raising the minimum power (common values 10-25%) When the machine is cutting in tight radiuses/corners it has to slow down and that also poportionally reduces the laser power. Raising minimum power can override this.

When I press "frame" on the machine, it moves to a different location before framing the cut.

* Move the machine to where you want to start the cut and press "origin" then try "frame" again.

The PC in the lab can't find the machine

* Make sure the PC is connected to the correct WiFi AP, "Laser cutter"
 
___
## Software
### Lightburn
https://lightburnsoftware.com/ 
Properly the most complete software for the laser cutter but does require an 80 USD license. It automatically detects the machine when plugged in and accepts all kinds of formats, SVG, DXF, AI, and even bitmaps. Runs on everything, Windows, macs and linux. The university has a license that is installed on the dedicated maker space PC next to the laser cutter. 
 
### Inkscape Plugin
On the cheap, we have https://github.com/jnweiger/inkscape-thunderlaser which worked somewhat out of the box on ubuntu 20.04 with Inkscape. It does have some rough edges, for instance, when clicking "Apply" the plugin starts cutting right away where normally you would expect it to just upload the workpiece to the cutter and then take it from there.
 
### Communication protocol
The machine does not use g-code but instead a proprietary "rd" format. There is not much information about the protocol online, but it is possible to find some reverse engineering projects on Github 
 
