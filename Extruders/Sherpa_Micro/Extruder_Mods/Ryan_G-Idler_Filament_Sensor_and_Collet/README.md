# Sherpa Micro Idler Filament Sensor and Collet Mod

This mod adds a collet for bowden tube retention, as well as a filament sensor
that detects the idler arm movement when it gets pushed outwards by the
filament. An M3 screw can be adjusted to control the angle of the idler arm at
which the sensor triggers. 

This mod is meant to be used with 
[Trad Rack](https://github.com/Annex-Engineering/TradRack) or any other MMU that
can make use of a filament sensor with a trigger point at the extruder gears.

![Modded Sherpa Micro](Images/with_5mm_collet.png?raw=true)

## Printed parts

This mod is based on
[release 2 of the Sherpa Micro](https://github.com/Annex-Engineering/Sherpa_Micro-Extruder/releases/tag/R2RC2).
The housing_core and idler_arm printed parts need to be replaced with versions
from this folder. All other printed parts should be taken from the Sherpa Micro
repo.

Different variants of housing_core are provided for different bowden tube collet
types. See [collet types](#collet-types) for details.

## Collet types

The following bowden tube collet types are supported:

- "5mm collet" (E3D V6, Bondtech LGX)
- "6mm collet" (UM2)

The filename of each variant of the housing_core STL will contain either
`(5mm_collet)` or `(6mm_collet)`to indicate the collet type it is meant for.

"5mm" and "6mm" refer to the approximate diameter of the part of the collet that
the collet clip goes around, highlighted in blue below:

![5mm and 6mm collets](Images/5mm_and_6mm_collets.png?raw=true)

All variants of the mod are shown below:

| 5mm collet variant                        | 6mm collet variant                        |
| ---                                       | ---                                       |
| ![](Images/with_5mm_collet.png?raw=true)  | ![](Images/with_6mm_collet.png?raw=true)  |

## BOM

In addition to the hardware required for a stock Sherpa Micro, the following
hardware is required for this mod:

| Component/Item                        | Qty Required  | Notes                                                                 |
| ---                                   | ---           | ---                                                                   |
| Omron D2F Microswitch                 | 1             | See Trad Rack BOM/sourcing guide for other variants that will work    |
| Collet                                | 1             | See [collet types](#collet-types) for collet type options             |
| Collet clip                           | 1             | Recommended to prevent the bowden tube from moving                    |
| M3 x 20mm Socket Head Cap Screw       | 1             |                                                                       |
| M2 x 10mm Pan Head Self Tapping Screw | 2             | M2 x 12mm also works                                                  |

Some example sources for collets and collet clips:
- 5mm collet - [KB3D](https://kb-3d.com/store/spare-parts/487-bondtech-push-fit-collar-for-bowden-coupling-175mm-7350011413331.html)
- 5mm collet clip - [KB3D](https://kb-3d.com/store/e3d/48-e3d-bowden-collet-clip-175mm-1644688775189.html)
- 6mm collet and collet clip - [AliExpress](https://www.aliexpress.us/item/2255801046836641.html)

See the
[Annex BOM/sourcing guide](https://docs.google.com/spreadsheets/d/1O3eyVuQ6M4F03MJSDs4Z71_XyNjXL5HFTZr1jsaAtRc/edit?usp=sharing)
for recommended sources for all other components.

## Other notes

- Based on release 2 of the Sherpa Micro extruder
- Widened filament path at inlet from 2mm to 2.4mm (diameter of inscribed
  circle)
- Increased clearance between housing core and idler arm from 1mm to 1.5mm
  (when idler arm face is vertical)
