# Hour Counter for Electronics Plate

![IMAGE](./Images/K3_Hour_Counter.jpg)

## WHY!?!

1. Will not lose data if your sd card is corrupted for any reason.
2. Physical representation of total hours printed (at least since this has been installed).
3. You get an audible "tick" whenever it is on.
4. Bragging rights?

## BOM

For this specific mod, you will need an hour counter similar to this one on [AliExpress](https://www.aliexpress.com/item/4000782513507.html?spm=a2g0s.9042311.0.0.27424c4dSkU6Cv)

You will also need 6 m3x8 screws and 4 m3x5x4 Heat Set Inserts.

## Install

Installation is fairly simple:

1. Install the 4 m3x5x4 Heat Set Inserts into the underside of the Hour Counter Plate. 
2. Fasten the Hour Counter to the Plate with 2 m3x8 screws (They are self tapping, but for this application it is fine.)
3. Fasten the Plate to your electronics box with the remaining 4 m3x8 screws into the Heat Set Inserts.

## Configuration
Configuration of this will differ depending on your specific needs and hardware. 

Keep in mind there are positive and negative terminals for this Hour Counter.

I have mine hooked up to a 24v heater pin on a Fysetc Spider board.
```
[output_pin hour_counter]
pin: PB3
```

You will need a macro to turn it on and off.
```
[gcode_macro hour_counter_on]
gcode:
    set_pin pin=hour_counter value=1

[gcode_macro hour_counter_off]
gcode:
    set_pin pin=hour_counter value=0
```

Then call on the "hour_counter_on" macro in my print_start and resume macros.
```
hour_counter_on
```


Also call for the "hour_counter_off" macro in your print_end, pause, and cancel macros.
```
hour_counter_off
```

## Contact
Please feel free to contact me (tayto #0001) on the Annex Engineering Discord with any issues.
