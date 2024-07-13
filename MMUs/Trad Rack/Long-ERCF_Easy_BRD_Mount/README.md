
**Pi Camera V3 (wide) Mount**
============
<table width=100%>
<TR>
<TD width=50% align="center"><img src="Images/left.jpg"></TD>
<TD width=50% align="center"><img src="Images/right.png"></TD>
<TR>
<TD width=50% align="center"><img src="Images/open.jpg"></TD>
<TD width=50% align="center"><img src="Images/top.jpg"></TD>
</TR>
</TABLE>

**Notes**
   - This is a mod of the official Nebula mount for TradRack that allows mounting of the ERCF Easy BRD Can board.  Credit to Ryan G for this original part as it is super cool and very nicely designed.
   - Since the BRD board is much narrower and slightly longer, this version increases the width slightly and makes it much less deep.  

**BOM**
   - (4) 6mm x 3mm magnets
   - (8) m3 x 8mm screws (preferably BHCS, although SHCS should also work)
   - (2) m3 x 16mm bolts
   - (6) m3 x 5mm x 4mm heat sets
   - (1) 4010 fan
     -  I used a Sunon 4010v2 12v fan and I further downvolted it to 8v using a buck converter (because I already had it).  
     - Alternatively you could probably use a Sunon 4010 5v fan (on the Tradrack BOM) and run it at 3.3v using the GPIO pins?

**Build Instructions**
   - Print the STLs in the provided orientation
   - Glue the two tray pieces together.  The pegs should be keyed to prevent gluing in the incorrect direction.
     - note there are several ziptie cutouts in the Tray Face.
   - Figure out how you will power the fan.  
     - Buck converter
       - https://www.aliexpress.us/item/3256805684077964.html
       - To power the buck, I solder wires to the 24v power input legs on the back of the power connector.
   - Attach the board with (3) m3 x 8 mm bolts going up through the bottom of the board.
   - Glue in the magnets to the tray and the Pocket
   - Melt in the (6) heat sets and attach the mount bracket with (4) m3 x 8 mm screws.




