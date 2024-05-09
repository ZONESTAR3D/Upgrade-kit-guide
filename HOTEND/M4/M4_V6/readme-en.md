[M4V6_CAUTION]: https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/M4/M4_V6/M4V6_Precaution.md
[MIXING_COLOE]: https://github.com/ZONESTAR3D/Document-and-User-Guide/tree/master/Mixing_Color
[SLICING_0]: https://github.com/ZONESTAR3D/Slicing-Guide
[SLICING_1]: https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer
[SLICING_2]: https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer#4-slicing-one-color
[SLICING_M4]: https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/PrusaSlicerGuide_M4.md
[FAQ_M4E4]: https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/FAQ_M4E4.md

----
## <a id="choose-language">:globe_with_meridians: Choose language </a>
[![](./lanpic/EN.png)](./readme.md)
[![](./lanpic/ES.png)](./readme-es.md)
[![](./lanpic/PT.png)](./readme-pt.md)
[![](./lanpic/FR.png)](./readme-fr.md)
[![](./lanpic/DE.png)](./readme-de.md)
[![](./lanpic/IT.png)](./readme-it.md)
[![](./lanpic/RU.png)](./readme-ru.md)
[![](./lanpic/JP.png)](./readme-jp.md)
[![](./lanpic/KR.png)](./readme-kr.md)
<!-- [![](./lanpic/SA.png)](./readme-ar.md) -->

----
## :book: M4V6 Hotend User Guide
ZONESTAR 4-IN-1-OUT mix color hot end has 4 input channels and 1 nozzle, four filaments are mixed in the hot end and then extruded through one nozzle, so it not only allows the printer to print the filaments original color, but also allows for printing more colors by adjusting the filament mixing ratio.

### Contents
- **[Attention](#A0)**
- **[Working principle](#A1)**
- **[Specifications](#A2)**
- **[Components of M4V6](#A3)**
- **[Wiring](#A4)**
- **[Structure](#A5)**
- **[Dimensions](#A6)**
- **[Installation & wiring](#A7)**
- **[Load/unload filaments](#A8)**
- **[Steps to print by using M4V6 hotend](#A9)**
- **[Slicing guide](#A10)**
- **[Troubleshooting](#A11)**
- **[Appendix](#A12)**

## <a id="A0">:warning: ATTENTION PLEASE</a>
### :loudspeaker: Before using the M4V6 hot end, please read [:book:Precautions for using M4V6][M4V6_CAUTION] carefully.
### :loudspeaker: Must load 4 filaments onto the M4V6 hotend simultaneously, incorrect operationa may block the mix color hotend. If the hot end blockage caused by incorrect operation, it is not covered by the warranty. 
### :loudspeaker: DON'T pull the "inner PTFE tubes" out of the M4V6 hotend. 
### :loudspeaker: Once the filaments has already entered the M4V6 hotend, DONOT use "Quickly Load" menu to load filaments.

### <a id="A1">Working principle</a>
**:warning: Before using the M4V6, please read [:book: Introduction of Color Mixing Extruder][MIXING_COLOE] to understand the working principles of mixing color extruder.**
###### 
[](https://github.com/ZONESTAR3D/Document-and-User-Guide/assets/29502731/2b9f4d75-b6fd-486f-aaa7-7a1163383316)

### <a id="A2">Specifications</a>
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

### <a id="A3">Components</a>
![](./2.jpg) ![](./1.jpg)

### <a id="A4">Wiring Terminal</a>
![](./wire.jpg)    
:pushpin: Extend cable is optional.

### <a id="A5">Structure</a>
![](./3.jpg)

### <a id="A6">Dimensions</a>
![](./size.jpg)

### <a id="A7">Installation & wiring</a>
The mounting position of M4 hot end conform to the "ZONESTAR hot end mounting standard", which can be installed on almost all ZONESTAR 3d printers, including P802, M8, D805S, Z8, Z9, Z10 etc. series of products etc.   
#### Installation
Simply remove the 3 screws behind the hot end assembly and install the M4 hotend assembly on the X carrier of the machine.
![](./M4_installation.jpg)  
#### Wiring
##### :loudspeaker: ATTENTION
- **Please watch for to distinguish terminals 3 and 4**, because their terminals color are the same, but the wires color are different.    
If the wires of 3 and 4 are connected reversely, you can see the nozzle temperature displayed on the LCD screen will be much higher than the room temperature after you powered on the machine.
- When pluging the terminal, **be careful not to push the metal terminal from the plastic case**.     
##### :loudspeaker: Please note  
- **The cooling fan must be turned on** (when the temperature of the hot end is higher than 60°C), otherwise the hot end may be blocked or even damaged.  
 - By default, the **working voltage** of the fan and heater at the hot end is **DC 24V**. 
#### Please following the define of terminals to connect the hotend to your control board.  
- **Without extend cable**     
![](./wiring1.jpg)  
- **With extend cable**     
![](./wiring2.jpg)  
#### Set hot end type on LCD MENU: Control>>Configure>>Hotend Type: Mixing
![](./hotendtype-mix.jpg)  

### <a id="A8">Load/Unload filaments</a>
#### :warning: ATTENTION PLEASE! You need load 4 filament to the hot end even you print one color 3d model, DONOT leave any channel empty before printing.
#### :warning: ATTENTION PLEASE! "Quickly Load" menu only can be used when loading the filament from extruder to hot end, once the filament entered the hot end, use "Slowly Load" menu but not "Quickly Load".
- **Load filament to the hotend:**     
[![](https://img.youtube.com/vi/-47yB95uIxI/0.jpg)](https://www.youtube.com/watch?v=-47yB95uIxI)
  - Cut the front of the filament with diagonal pliers before loading it to the extruder and hot end.
  - Load 4 filaments to all extruders one by one.
  - Rotate the gear of extruders to load filament one by one, do not rotate each extruder more than 2 turns at a time, until all the filaments enter to the inner PTFE tube of hot end, extrdue more 4 ~ 5 turn for each extruder and then stop.      
  :warning: Don't feed filaments to the hotend when any channel of the hot end are empty.     
  :warning: Ensure that the filaments for each channel reach the bottom of the hot end before feeding the filament.    
- **Unload filament from the hotend:**
  - Heating the nozzle (200℃ for PLA / 230℃ for PETG/ABS).
  - Simultaneously feed filament at least 10mm on all 4 channels.
  - Operature on the LCD menu or rotate the extruder gear to unload filaments.

### <a id="A9">Steps to print by using M4V6 hotend</a>
#### Print one color 3D model
- **Prepare gcode file**. Slicing the 3d modle by using one color 3d printer settings, please refer to [**here**][SLICING_2].   
- **Load filaments**. Load **all 4 filaments** to the extruders and then feed the filaments into the bottom of the M4V6 hot end.     
- **Print from SD card**. Move item to **Print** item on LCD screen and click the knob and choose the gcode file, click knob to start print.
- **Fine tune nozzle height**. Wait the nozzle and hotbed heating, and when the printer starting to print the first layer, double click the knob of LCD screen to fine tune the distance from the nozzle to the bed, and then wait it to finish.
#### Print multi color 3D model
- **Prepare gcode file**. Slicing the 3d modle by using M4 multi color 3d printer settings, please refer to [**here**][SLICING_M4].   
- **Load filaments**. Load **all 4 filaments** to the extruders and then feed the filaments into the bottom of the M4V6 hot end. 
- **Print from SD card**. Move item to **Print** item on LCD screen and click the knob and choose the gcode file, click knob to start print.
- **Fine tune nozzle height**. Wait the nozzle and hotbed heating, and when the printer starting to print the first layer, double click the knob of LCD screen to fine tune the distance from the nozzle to the bed, and then wait it to finish.

### <a id="A10">Slicing</a>
We recommend using PrusaSlicer for slicing. For installation and usage tutorials, please refer to the following link:
- **[Install Prusaslicer software][SLICING_1]**    
- **[Slicing guide for M4 hotend][SLICING_M4]**     
For more tutorials on using other slicing software, please refer to [:book:this guide][SLICING_0].

### <a id="A11">Troubleshootings</a>
If there is any problems while using the M4V6 hot end, please refer to [**:book: this troubleshooting manual**](./M4V6_FAQ/readme.md) to find a solution first.

### <a id="A12">:paperclip: Appendix</a>
#### :paperclip: Appendix I: Achieve speedy printing by using M4V6 hot end
When printing a single color 3d model, M4V6 can support higher flow rates. About the details, please refer to [:book: this guide](./HighFlow/readme.md).

#### :paperclip: Appendix II: [How to switch between E4 hotend and M4 hotend][FAQ_M4E4]
