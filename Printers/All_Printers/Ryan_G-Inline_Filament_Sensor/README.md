# Inline Filament Sensor

This mod aims to be a relatively lightweight filament sensor that will work
with any printer that uses 1.75mm filament and a reverse bowden tube with a 4mm
outer diameter.

The sensor can be placed right above the toolhead to be used
with [Trad Rack](https://github.com/Annex-Engineering/TradRack) or any other MMU
that can make use of a toolhead filament sensor with a trigger point above the
extruder gears, or it can be placed wherever you want to be used as a runout
sensor.

Note: if used with an MMU, it is required that your printer's toolhead or
extruder has its own bowden coupling/collet to prevent the reverse bowden tube
from coming out.

![Inline filament sensor](Images/with_5mm_collet.png?raw=true)

## Printed parts and collet types

One printed part is required. Different variants are provided for different
bowden tube collet options. The following bowden tube collet types are
supported:

- "5mm collet" (E3D V6, Bondtech LGX)
- "6mm collet" (UM2)

The filename of each variant of the sensor_housing STL will contain either
`(5mm_collet)` or `(6mm_collet)` to indicate the collet type it is meant for.
The printed part also has "5" or "6" engraved in the bottom.

"5mm" and "6mm" refer to the approximate diameter of the part of the collet that
the collet clip goes around, highlighted in blue below:

![5mm and 6mm collets](Images/5mm_and_6mm_collets.png?raw=true)

All variants of the filament sensor are shown below:

| 5mm collet variant                        | 6mm collet variant                        |
| ---                                       | ---                                       |
| ![](Images/with_5mm_collet.png?raw=true)  | ![](Images/with_6mm_collet.png?raw=true)  |

## BOM

The following hardware is required:

| Component/Item                        | Qty Required  | Notes                                                                 |
| ---                                   | ---           | ---                                                                   |
| 4mm Ball Bearing                      | 1             | See Trad Rack BOM/sourcing guide for recommended sources              |
| Omron D2F-L Microswitch               | 1             | See Trad Rack BOM/sourcing guide for other variants that will work    |
| Collet                                | 2             | See [collet types](#collet-types) for collet type options             |
| Collet clip                           | 2             | Recommended to prevent the bowden tube from moving                    |
| M2 x 10mm Pan Head Self Tapping Screw | 2             | longer screws will also work but will stick out                       |

Some example sources for collets and collet clips:
- 5mm collet - [KB3D](https://kb-3d.com/store/spare-parts/487-bondtech-push-fit-collar-for-bowden-coupling-175mm-7350011413331.html)
- 5mm collet clip - [KB3D](https://kb-3d.com/store/e3d/48-e3d-bowden-collet-clip-175mm-1644688775189.html)
- 6mm collet and collet clip - [AliExpress](https://www.aliexpress.us/item/2255801046836641.html)

See the
[Annex BOM/sourcing guide](https://docs.google.com/spreadsheets/d/1O3eyVuQ6M4F03MJSDs4Z71_XyNjXL5HFTZr1jsaAtRc/edit?usp=sharing)
for recommended sources for all other components.

## Wire management and sensor orientation

The sensor housing has a bar that the wires can be zip-tied to. It is highly
recommended to make use of this to avoid stress at the solder joints:

![Wiring example](Images/wiring_example.jpg?raw=true)

The filament sensor can use either end as the inlet or outlet. It is recommended
to orient the sensor based on which way you want the wires to go: either to the
toolhead or directly back to the control board.

## Trigger point

The sensor housing has a notch located at the height of the center of the ball,
which approximately corresponds to the position of the filament tip when the
sensor is triggered. This may be useful for measuring toolhead config lengths
for Trad Rack or other MMUs.

![Trigger point notch](Images/trigger_point_notch.png?raw=true)
