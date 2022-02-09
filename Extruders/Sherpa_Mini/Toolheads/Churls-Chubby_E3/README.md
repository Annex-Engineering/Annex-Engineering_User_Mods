# Chubby Toolhead for the Ender 3

This is a complete toolhead for the Ender 3 (v1 carriage) that uses Sherpa Mini, QuickDraw, dual 5020 part cooling fans, and the stock creality hotend.

![Image of Stiffy](./Images/Chubby.png)

## Parts Required

**Required**
- Sherpa Mini with K front plate
- 1x 4010 axial fan (hotend cooling)
- 2x 5020 blower fan (parts cooling)
- 4x M3X20mm
- 6x M3x25mm
- 2x M3x16mm
- 2x M3x12mm
- 3x M3x6mm
- 2x M3 nuts
- 10X Heatset Inserts (3x5x4mm)

**Optional**
- [QuickDraw](https://github.com/Annex-Engineering/Quickdraw_Probe) 
	- Print, assemble, and install Quickdraw, dock, and holder (see [CAD](./CAD/Stiffy.EASM))
		- Set the X position of dock between the X home position and the bed with the opening facing left. There should be about 2mm between the bed and the back of the dock.
		- Set the Y position of dock so that Stiffy's magnets are aligned with QuickDraw's magnets when it is docked.
		- Set the Z position of the dock so that Stiffy's and QuickDraw's magnets barely touch after homing Z with the stock Z endstop. 
	- Download Dalegaard's [XZ_dockable_probe.py](https://gist.github.com/dalegaard/3f1b8695275a15b1888119304d79b88d) module and modify [klipper config](./QuickDraw_klipper_config.cfg)
	- Note: The stock endstop locates the dock height then QuickDraw defines Z0 once the homing routine is complete.
	- Homing video: 

[![Homing video](https://img.youtube.com/vi/NMOQogjF0p8/0.jpg)](https://youtu.be/NMOQogjF0p8)

