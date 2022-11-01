[:gift: **Buy (ZONESTAR Offical Store)**](https://bit.ly/39qDtKp)
[:gift: **Buy (Aliexpress)**](https://www.aliexpress.com/item/1005002951777699.html)

## E4 Hotend user guide
### 1. Specifications
There are 4 input channels and 1 nozzles on the E4 hotend, when switching color, we need to pull out the previous color filament first and then load the next color filament.
![](./E4-1.jpg)

### 2. Components
![](./E4-2.jpg)
>
    1. Cooling Fan        2. Housing        3. Bed leveling sensor(optional)  4. Mounted Screws   5. Extruder Fan
    6. Fan Duck           7. Heating block  8. Heat sink                      9. Nozzle           10. Cartridge heater 
    11.Temperature sensor 12. Throat        13. Silicone sleeve               14. Fittings        15. Cable

### 3. Wire and Terminals
![](./E4-3.jpg)   
If you choose "E4 hotend for Z9V5", it hasn't the extend cable.


### 4. Installation & wiring
#### :one: Installation
Simply remove the 3 screws behind the hot end assembly and install the E4 hotend assembly on the X carrier of the machine.
![](./E4-4.jpg)  
#### :two: Wiring
:loudspeaker: **Attention** 
- **Please watch for to distinguish terminals 3 and 4**, because their terminals  color are the same, but the wires color are different.    
PS: If the wires of 3 and 4 are connected reversely, you can see the nozzle temperature displayed on the LCD screen will be much higher than the room temperature after you powered on the machine.
- When pluging the terminal, **be careful not to push the metal terminal from the plastic case**.  
##### Wiring of Z9V5Pro
![](./E4_wiring_Z9V5.jpg)  
##### Wiring of Z8P (Extend cable is omitted in the below picture)
![](./E4_wiring_Z8P.jpg)  
#### :three: Set hot end type on LCD MENU: Control>>Configure>>Hotend Type
:warning: If you can't see the menu on the LCD screen of your printer, please upgrade to the newest version. [:link: **Firmware Download Link**](https://github.com/ZONESTAR3D/Firmware)    
![](./hotendtype-nonmix.jpg)  

### 5. Working principle
4-IN-1-OUT hot end is composed of fitting, heat-sink, heater, nozzle and other components, when printing, extrusion feeder insert one color filaments into the hot end, then the filament is melted and flowed from the nozzle, while need to chang to another color filament, the extruder pull the previous color filament out of the hot end, and then load another color filament.    
:movie_camera: [**Watch animation demonstration of E4 working principle**](./E4_rinciple.gif).   
Since the melted residual filament in the nozzle cannot be completely pulled out, after replacing the filament, a "wipe tower" needs to be added to remove the residual filament in the nozzle to make better color discrimination, refer to :point_right: [Slicing](#8-slicing)
![](./E4-5.jpg) 

###  6. Pre-load filaments
Before printing, please pre-load the filaments into the appropriate position of the hot end so that the extruder can load smoothly the filaments into and out of the hot end.
- **Step 1:** Load filaments from the extruder and let the filaments extend about 10mm out of PTFE tubes.
- **Step 2:** Plug the PTFE tubes (with filaments) into the HOTEND.  
:pushpin: :warning:**If there is a filament in the hot end, heating and noozle and then pull it out first.**    
:pushpin: Cutting the front of filaments into a sharp shape before loading filament. 
:pushpin: The filament of the extruder that is not used during printing does not need to be loaded.   
![](./E4-6.jpg) 
:pushpin: Add some gcodes in the **"Start gcode"** ([:point_right: View](https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/Custom_Gcode.md#start-gcode)) of slicing software to print. 
![](./Preload_line.jpg)   
:pushpin: Add some gcodes in the **"End gcode"** ([:point_right: View](https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/Custom_Gcode.md#end-g-code)) of slicing software to pull out the last printed filament from the hotend.      


### 7. Unload filaments
Please follow the steps below to unload the filament from the hotend:
- Step 1: Heating the nozzle (190 degree for PLA and 230 degree for ABS).
- Step 2: Rotate gear of the extruder to unload the filament.   
:star2: Some 3d printers (e.g. Z9V5Pro) has a “Filament” Menu on LCD screen, please operate the LCD screen and use menu of “Prepare>>Preheat/Extruder/Unload” etc. to preheat the nozzle, choose extruder and unload filaments.

### 8. Slicing
- For PrusaSlicer(recommended), please refer to :point_right: [**here**](https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer#6-slicing-muti-color-for-e4-hotend)
- For Cura slicer, please refer to :point_right: [**here**](https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/cura)
- For Simplify3d Slicer, please refer to :point_right: [**here**](https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/Simplify3D#slicing-video-toturial-for-z9v5-with-e4-hotend)

### 9. Maintain
For some reason, it may happen that the filament is clogged inside the hot end and cannot be pulled out 
and pushed in, in this case, you may need to remove the heating block from the hot end and clean the 
hot end, the reasons included:
1. The filament breaks inside the hot end, usually because the filament is damaged by moisture or 
poor quality. 
2. When the filament is pulled out, the melted front end will be pulled out a long filament, and when 
a new filament enters, the filament may be glued together and cannot be inserted. The cause is 
usually an excess of toughening agent added to the filament. [Refer to here to set the length when switching filament](https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/Custom_Gcode.md)
3. The filament is not completely melted due to the printing temperature setting problem, and may 
be stuck in the PTFE tube when pulled out. 
4. Incorrect "Retract length" or “switch extruder" settings on slicing software. :point_right:[For Detail.](https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/PrusaSlicerGuide_E4.md#step-6-set-the-print-settings)


#### Unassemble the E4 hotend
If the filament clogged in the hotend, please unassemble the hotend and then remove the filament from the "throat", steps as follows:
:warning: Wait for the hot end to cool down before operation.:warning:   
![](E4-8.jpg) 
1. Remove the hotend assembly from the X carrier of 3d printer, and take down the silicone insulation sleeve.
2. Remove the cable from the hotend housing.
3. Loosen the 2 screws fixing the hot end.
4. Pull the hot end out of the heats-sink.

#### Replace the inner PTFE pipe
If the blockage is easy to occur, it is recommended that you replace the built-in PTFE pipe too, steps as follows:
![](E4-9.jpg) 
1. Remove the scews which fixed the temperature sensor and heater and take down the temperature sensor and heater.
2. Use a wrench to remove the nozzle.
3. Remove the built-in PTFE pipe to be replaced.
4. Install a new PTFE pipe, and use a paper cutter to cut off.
5. the PTFE pipe should be about 0.5mm longer than the throat, or it can be directly flush.
6. Use a small metal thin rod to turn it inside, because when cutting the PTFE pipe, its inner diameter may become thinner.
7. Reinstall the hot end in reverse order.


### 10. Testing gcode
We have uploaded some test files to our website, you can download them from [**here**](../example/readme.md)

### Video toturial
- :movie_camera: [**How to load Filament - for one color printing**](https://youtu.be/6aTF5QnFhi4)
- :movie_camera: [**How to load Filament - for multi colors printing**](https://youtu.be/FyHrAMytlT8)
- :movie_camera: [**Download and install slicing software**](https://youtu.be/SgyXD-kQIeo)  
- :movie_camera: [**Slicing guide - for one color printing**](https://youtu.be/SgyXD-kQIeo4)  
- :movie_camera: [**Slicing guide - for multi colors printing**](https://youtu.be/AIKrszmxvE4)    
- :movie_camera: [**Slicing guide - Convert one color 3d file to multi colors**](https://youtu.be/2LJu4G0T4Zg)    

  