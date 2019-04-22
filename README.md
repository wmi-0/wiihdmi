# wiihdmi
HDMI for your Wii powered by GCVideo

This PCB is based on the popular GCVideo project as well as the Shuriken V3 schematics and features HDMI output (240p, 480i, 480p) for the Wii.
Menu navigation is possible via IR-remote or Gamecube controller.  
One of the main goals for this project was to keep it as cheap as possible.
This means no flex-cable for an easier install, no replacement of analog output (RGB/Component) and most importantly a 2-layer PCB design for cheap manufacturing.

**Consider this project as a beta for now.**  
I've spent several hours testing it on my launch-model Wii, but I'd like to hear some second opinions calling it ready for general use.

## Compatibility
### main_pcb_6_layer
Confirmed to work on RVL-CPU-01 boards.  
The layout possibly fits RVL-CPU-20 as well, but this is currently untested. Won't (properly) fit RVL-CPU-30.  

### main_pcb_4_layer
The new PCB layout is designed for 4-layer Wiis (RVL-CPU-40/50/60) but it's untested as of now.

Both designs use a 2-layer PCB layout which can be manufactured on the cheap, 4/6-layer is just the number of layers used on the intended target Wii mainboard.

## Install
See [GCVideo documentation](https://github.com/ikorb/gcvideo/blob/master/HDL/gcvideo_dvi/README-Wii.md#digital-audio-and-video)

## BOM
### Main PCB
| Designator  | Component |
| ------------- | ------------- |
| U1  | XC3S200A-4VQG100C  |
| U2  | M25P40  |
| U3  | TPS74012DGKR  |
| U4  | IRM-V538/TR1  |
| SW1  | EVQ9P701P  |
| J3  | 15 pin FFC connector 0.5mm pin pitch  |
| C1, C2  | 1 uF, 0805  |
| C3  | 10 uF, 0805  |
| C4-C12  | 0.1 uF, 0805  |
| R1, R3  | 4.7K, 0805  |
| R2  | 330, 0805  |

Use 0603 components for main_pcb_4_layer.

### HDMI PCB
| Designator  | Component |
| ------------- | ------------- |
| J1  | 15 pin FFC connector 0.5mm pin pitch  |
| J2  | Mini-HDMI (Type C) socket  |
| R1  | 180, 0402  |
| R2, R3  | 10K, 0402  |
| U1-U3  | TPD4S010 DQA (optional)  |

Use 0.8mm PCB thickness for both PCBs.

## Todos and next steps
- ~~PCB for 4-layer, 65nm Wii consoles (RVL-CPU-40+)~~
- ~~Provide better install pictures showing the current version of the PCB~~
- Switch to a more common 16 pin FFC instead of 15 pin
- Possibly add half-cut vias as anchor points (the initial design already had some, but the PCB manufacturer charged extra so I removed them again)
- KiCad project cleanup

## Acknowledgements
[ikorb](https://github.com/ikorb): GCVideo project  
[Steven Taffs](http://www.retro-system.com/shuriken%20video.htm): Shuriken V3 schematic and incredibly useful M25P40 programming tool  
[citrus3000psi](https://github.com/citrus3000psi): Inspiration from GCHDMI designs

## License
This project is licensed under the GPL v3.0 License - see the LICENSE.md file for details