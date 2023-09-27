# M5-Based Tophat

This mod allows assembly of the K3 tophat using M5 bolts and heat set inserts instead of printed dowels and glue. The design is inspired by [yhaiovyi's tophat](https://github.com/everycoloryouare/Annex-Engineering_User_Mods/tree/main/Printers/K3/yhaiovyi-K3_Glueless_Tophat) mod, but keeps the original K3 design aesthetic.

![Exploded](Images/top_lid_assembly_exploded.png)

## Goals
- Allow for easy assembly and disassembly
- Improve rigidity
- Maintain original design aesthetic

## Important Printing Notes
- The Fabreeko kit comes with slightly smaller heat set inserts measuring 7.5mm in diameter instead of 8mm. If you are using these inserts then print the corner parts (tophat_lid_structure_a_fabreeko_x4_rev1) in the <i>STLs/for_frabreeko_heat_set/</i> folder instead.
- These are large pieces that fit tightly together and are therefore sensitive to material shrinkage. A 0.5-1.0% shrinkage will cause the corner bolt holes (which are separated by 280mm on a side) to be off by 1.4-2.8mm and the top panel will not line up correctly.
- To compensate for shrinking there are two options:
    - Scale both tophat_lid_structure_a_x4_rev1 and [a]_tophat_lid_structure_b_x4_rev1 in X and Y. So for a 0.6% shrinkage amount scale X and Y by 100.6%. This may cause the press fit magnets to be loose necessitating gluing the magnets.
    - Or print one of the pre-compensated [a]_tophat_lid_structure_b_XX_percent_x4_rev1 files in the <i>/STLs/tophat_lid_structure_b_pre-compensated</i> folder where the "XX_percent" corresponds to the material shrink amount. So if the material shrinks by 0.6% print the file [a]_tophat_lid_structure_b_0.6_percent_x4_rev1.stl. A good starting point for ABS and ASA is around 0.5% or 0.6%.

If you are unsure about what compensation to use, print only 2x tophat_lid_structure_a_x4_rev1 and 1x [a]_tophat_lid_structure_b_x4_rev1 using either method with a best guess for the shrink amount and test fit the panel. You can then adjust and print [a]_tophat_lid_structure_b_x4_rev1 parts until the panel lines up correctly.

## BOM
- Sources for all items can be found in the Annex [sourcing guide](https://docs.google.com/spreadsheets/d/1O3eyVuQ6M4F03MJSDs4Z71_XyNjXL5HFTZr1jsaAtRc/htmlview#) for the K3.

| Item                                                             | Qty Required  |
| ---                                                              | ---           |
| M5 x 8mm Dia x 7mm Length Heat Set Insert <br> M5 x 7.5mm Dia x 7mm Length (Fabreeko)                        | 8             |
| M5 x 20mm SHCS or BHCS                                           | 8             |
| M3 x 5mm Dia x 4mm Length Heat Set Insert                        | 12            |
| 6x3mm Magnet                                                     | 12            |

## Beta and Test Prints
This mod is currently in beta and has not been fully tested with different printer tolerances or material types. If you are curious how parts will fit but don't want to waste filament on the full parts, there are test parts you can print in the <i>STLs/test_prints/</i> folder to check fitment.

Feel free to tag @EveryColorYouAre on the Annex Engineering discord if you have questions or feedback.

## Assembly
- Insert M3 heat set inserts and magnets into the printed parts as for the stock tophat.
- Insert two M5 heat set inserts into the ends of each tophat corner (tophat_lid_structure_a_x4_rev1).
- Push two M5 x 20mm bolts into the slot and through the hole in each tophat center ([a]_tophat_lid_structure_b_x4_rev1) and screw into the heat set of the tophat corners using a ball end allen key.
- Two optional covers can be snapped into the bolt slots of each tophat center.

## Images
Cross-section of assembled tophat
![section](Images/top_lid_assembly_cross_section.png)

Test print parts assembled
![test_print](Images/test_prints.png)

