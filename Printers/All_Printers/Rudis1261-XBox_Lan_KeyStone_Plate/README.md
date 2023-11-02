## Waveshare 4.3" DSI screen mount [like this one](https://www.diyelectronics.co.za/store/displays/3833-3inch-wide-angle-touch-lcd-display-for-raspberry-pi.html?search_query=waveshare&results=183)

This is to mount your DSI waveshare screen to your Ebox. I like this screen as it's not too small/big and is fairly affordable. 

![image](./Images/IRL.jpeg)

### Print settings
- Perimeters 4
- Infil > 50% infill
- Infil type rectilinear
- Solid Top/bottom layers (4+)
- Layer height .20mm 

### Getting the screen and touch to rotate

Edit `/boot/config.txt` with your favourite text editor and add this section to it:
```
[all]
display_rotate=3
display_lcd_rotate=3
display_auto_detect=1
dtoverlay=disable-bt
```

Edit this file `/usr/share/X11/xorg.conf.d/40-libinput.conf` with your favourite text editor, and update the `libinput touchscreen catchall` section to this:
```
Section "InputClass"
        Identifier "libinput touchscreen catchall"
        MatchIsTouchscreen "on"
        MatchDevicePath "/dev/input/event*"
        Option "TransformationMatrix" "0 -1 1 1 0 0 0 0 1"
        Driver "libinput"
EndSection
```

![image](./Images/Waveshare_4_3_Screen1.png)
![image](./Images/Waveshare_4_3_Screen2.png)
![image](./Images/IRL2.jpeg)
