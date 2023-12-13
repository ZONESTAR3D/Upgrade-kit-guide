## :book: M4V6 hot end use manual
ZONESTAR 4-IN-1-OUT **mix color** hot end (referred to as **M4 Hot end**) has 4 input channels and 1 nozzle, four filaments are mixed in the hot end and then extruded through a nozzle.Therefore, the M4 hot end not only allows the printer to print the original color of the filaments, but also allows for printing more colors by adjusting the filament mixing ratio.

-----
## :warning: ATTENTION PLEASE 
## Before using the M4V6 hot end, please read [:book:Precautions for using M4V6](https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/M4/M4_V6/M4V6_Precaution.md) carefully.
### :loudspeaker: Must load 4 filaments onto the M4V6 hotend simultaneously, incorrect operationa may block the mix color hotend. If the hot end blockage caused by incorrect operation, it is not covered by the warranty. For how to load filaments, please refer to [this guide](#7-how-to-load-and-unload-filaments).
### :loudspeaker: DON'T pull the "inner PTFE tubes" out of the M4V6 hotend.

-----
### 1.Specifications
|            Item            |      Parameters            |            Item            |      Parameters            |
|:--------------------------:|:--------------------------:|:--------------------------:|:--------------------------:|
|    Rated Voltage           |      DC24V/60W Max         |     Nozzle Diameter        | Default 0.4mm<sup>1</sup>  |
|    Input Channel           |      4                     |     Nozzle model           |      E3D V6                |
|    Nozzles Number          |      1                     |     Filament Diameter      |      1.75mm                |
|    Heater                  |      24V/60W ⌀6x25mm       |     Temperature Sensor     | NTC Thermistor 100K B3950  |
|    Cooling Fan             |   4010/5000RPM/24V 0.15A   |    Extruder Fan            | 4010/5000RPM/24V 0.15A     |
|    Support Filaments       | PLA/PLA+/PETG/ABS/ASA etc. |    Working Temperature     | 260℃ Maximus              |
|    Wire length             |      1 meter               |    Outer Dimensions        |      50x60x75mm            |
|    Net weight              |      220g                  |    Gross weight            |      350g                  |

-----
### 2.Components
![](./1.jpg) ![](./2.jpg)

-----
### 3.Wire and Terminals
![](./wire.jpg)

-----
### 4.Structure
![](./3.jpg)

-----
### 5.Dimensions
![](./size.jpg)

-----
### 6.Installation & wiring
The mounting position of M4 hot end conform to the "ZONESTAR hot end mounting standard", which can be installed on almost all ZONESTAR 3d printers, including P802, M8, D805S, Z8, Z9, Z10 etc. series of products.   
#### 6.1 Installation
Simply remove the 3 screws behind the hot end assembly and install the M4 hotend assembly on the X carrier of the machine.
![](./M4_installation.jpg)  
#### 6.2 Wiring
##### :loudspeaker: **Attention** 
- **Please watch for to distinguish terminals 3 and 4**, because their terminals  color are the same, but the wires color are different.    
If the wires of 3 and 4 are connected reversely, you can see the nozzle temperature displayed on the LCD screen will be much higher than the room temperature after you powered on the machine.
- When pluging the terminal, **be careful not to push the metal terminal from the plastic case**.     
#### :loudspeaker: **Please note**    
- **The cooling fan must be turned on** (when the temperature of the hot end is higher than 60°C), otherwise the hot end may be blocked or even damaged.  
 - By default, the **working voltage** of the fan and heater at the hot end is **DC 24V**. 
#### Please following the define of terminals to connect the hotend to your control board.  
- **Without extend cable**     
![](./wiring1.jpg)  
- **With extend cable**     
![](./wiring2.jpg)  
#### 6.3 Set hot end type on LCD MENU: Control>>Configure>>Hotend Type: Mixing
:warning: If your printer hasn't a 4.3" TFT-LCD screen, ignore this step.   
:warning: If you can't see the menu on the LCD screen of your printer, please upgrade to the newest version. [:link: **Firmware Download Link**](https://github.com/ZONESTAR3D/Firmware)    
![](./hotendtype-nonmix.jpg)  

-----
### 7. How to load and unload filaments
### :warning: ATTENTION PLEASE
For M4V6 hotend, you need to load 4 filament to the hotend even you print one color 3d model, DONOT leave any channel empty before printing.
- **Load filament to the hotend:**     
[:clapper:video tutorial](https://youtu.be/-47yB95uIxI).
  - Cut the front of the filament with diagonal pliers before loading it to the extruder and hot end.
  - Load 4 filaments to all extruders one by one.
  - Rotate the gear of extruders to load filament one by one, do not rotate each extruder more than 2 turns at a time, until all the filaments enter to the inner PTFE tube of hot end, extrdue more 4 ~ 5 turn for each extruder and then stop.      
  :warning:It is recommened to use the ***Prepare>>Filament>>Extruer: All*** and ***Prepare>>Filament>>Load quickly*** menu to load filamets if your printer has a "filament" Menu.     
  :warning: Don't extrude filament when any one of the channel is empty.     
- **Unload filament from the hotend:**
  - Heating the nozzle (200℃ for PLA / 230℃ for PETG/ABS).
  - Operature on the LCD menu or rotate the extruder gear to unload filaments.

-----
### 8. Steps to use M4V6 hotend
#### Print one color 3D model by M4V6 ho tend
- **Prepare gcode file**. Slicing the 3d modle by using one color 3d printer settings, please refer to [**here**](https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer#4-slicing-one-color).   
**Here is a test gcode file for your reference: [:arrow_down: download xyz_cube zip file](./xyz_cube.zip)** and unzip it on PC, and then copy the **xyz_cube.gcode** to SD card. Plug the SD card to the SD socket of machine.
- **Load filaments**. Refer to [:point_up: **"How to load and unload filament"**](#load-and-unload-filament) to load all 4 color filaments to the extruders and hotend.     
- **Print from SD card**. Move item to **Print** item on LCD screen and click the knob and choose the gcode file, click knob to start print.
- **Fine tune nozzle height**. Wait the nozzle and hotbed heating, and when the printer starting to print the first layer, double click the knob of LCD screen to fine tune the distance from the nozzle to the bed, and then wait it to finish.
#### Print multi color 3D model
- **Prepare gcode file**. Slicing the 3d modle by using M4 multi color 3d printer settings, please refer to [**here**](https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/PrusaSlicerGuide_M4.md).   
**Here is a test gcode file for your reference: [:arrow_down: **download M4_4CTest zip file](./M4_4CTest.zip)** and unzip it on PC, and then copy the **M4_4CTest.gcode** to SD card. Plug the SD card to the SD socket of machine.
- **Load filaments**. Refer to [:point_up: **"How to load and unload filament"**](#load-and-unload-filament) to load all 4 color filaments to the extruders and hotend.
- **Print from SD card**. Move item to **Print** item on LCD screen and click the knob and choose the gcode file, click knob to start print.
- **Fine tune nozzle height**. Wait the nozzle and hotbed heating, and when the printer starting to print the first layer, double click the knob of LCD screen to fine tune the distance from the nozzle to the bed, and then wait it to finish.

-----
### 9. Slicing
- **[Install Prusaslicer software](https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer)**
- **[Multi Color Slicing](https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/PrusaSlicerGuide_M4.md)**

-----
### :paperclip: Appendix I: Achieve speedy printing by using M4V6 hot end
When printing a single color 3d model, M4V6 can support higher flow rates. About the details, please refer to [:book: this guide](./HighFlow/readme.md).

-----
### :paperclip: Appendix II: How to clean the blocked M4V6 hotend
About how to clean the blocked M4V6 hotend, please refer to [:book: this guide](./cleanM4V6.md).

-----
### :paperclip: Appendix III: How to replace of the inner PTFE tubes
About how to replace the inner PTFE tubes of the M4V6 hotend, please refer to [:book: this guide](./ReplaceM4V6InnerPTFE.md).

-----
### [:book: How to switch hotend between E4 hotend and M4 hotend](https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/FAQ_M4E4.md#how-to-switch-between-m4-hotend-and-e4-hotend)
