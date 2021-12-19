# K3 Outside Camera

This mod allows you to mount a webcam to the Annex K3 printer behind the rear panel. It is compatible with both full height and standard versions of the backpack.

![CAD Model](Images/cad_model.png?raw=true)

![Camera View](Images/camera_view.png?raw=true)

## Goals
- Keep the camera out of the chamber to protect it from heat
- Provide a view of the full print area at nozzle height

## BOM
- Sources for all items except the webcam can be found in our [sourcing guide](https://docs.google.com/spreadsheets/d/1O3eyVuQ6M4F03MJSDs4Z71_XyNjXL5HFTZr1jsaAtRc/htmlview#) in the K3 sheet.
- [example source for the webcam (Amazon)](https://www.amazon.com/Microphone-Wansview-Correction-Streaming-Conference/dp/B088D3VXC6)

| Item                                                          | Qty Required  |
| ---                                                           | ---           |
| M3 x 8mm Button Head Cap Screw                                | 4             |
| M3 x 8mm Socket Head Cap Screw                                | 9             |
| M3 Brass Heat Stake Threaded Insert - Short (5.0mm x 4.0mm)   | 12            | 
| Wansview 1080P Webcam                                         | 1             |
| Foam Panel Tape (5mm Wide x 3mm Thick)                        | about 65mm    |

## Notes
- I recommend following the eDrawing (located in the CAD folder) for assembly.
- The window is meant to be cut from 3mm acrylic, but thicker material may work. The dimensions aren't critical, as long as it fits in the plastic part and fills up the hole in the front casing. Rounded corners are needed for clearance but don't need to be precise.
- There are currently 2 versions of the `camera_mount` stl: a generic version, and a version specifically for the Wansview camera. The Wansview version uses foam tape to make sure light doesn't strike the window from the back and cause glare:
  - ![Camera Mounts](Images/camera_mounts.jpg?raw=true)
- This mod is meant to give a full view of the print area of K3 at nozzle height. It may work with other printers that have a 38mm diameter hole in the rear panel, but the webcam might not be aimed correctly.
  - ![Camera Angle](Images/camera_angle.png?raw=true)
- Using other cameras:
  - This mod was designed for the Wansview webcam. I cannot guarantee that you will get the full field of view if using a different camera.
  - Depending on how your camera attaches, you will likely have to modify the `webcam_arm_left` and `webcam_arm_right` pieces.
  - I recommend either modifying the `camera_mount` piece to fit around your camera's lens to block off light, or using the generic version of the mount and adding separate material for blocking light.
  - The CAD model includes a "Camera FOV" component for visualizing the intended field of view of the camera. This may be helpful for positioning your camera if creating a custom camera mount.

## Other Images
![Front View](Images/front_view.jpg?raw=true)