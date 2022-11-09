[:gift: **Sell link (ZONESTAR Offical Store)**](https://bit.ly/39qDtKp)     
[:gift: **Sell link (Aliexpress)**](https://www.aliexpress.com/item/1005002951777699.html)

## :book: E4 Hotend user guide
ZONESTAR 4-IN-1-OUT Non-mix color hotend (we called E4 Hotend) has 4 input channels and 1 nozzle, when switching color, the previous color filament need to be unloaded (pulled out) from the hot end, and then load the next color filament.

----
### 1. Specifications
![](./E4-1.jpg)

----
### 2. Components
The E4 hot end assembly includes the following parts/accessories:    
![](./E4-2.jpg)
>
    1. Cooling Fan          2. Housing              3. Bed leveling sensor install hole     4. Mounted Screws                         
    5. Extruder Fan         6. fan "duck" prints    7. Heating block                        8. Heat sink                         
    9. Nozzle               10. Cartridge heater   11.Temperature sensor                    12. Throat        
    13. Silicone sleeve     14. Fittings(Pneumatic Connectors)                              15. Cable

----
### 3. Wire and Terminals
![](./E4-3.jpg)   
:warning: **"E4 hotend for Z9V5"** hasn't the extend cable.

----
### 4. Installation & wiring
The mounting position of E4 hot end conform to the "ZONESTAR hot end mounting standard" , which can be installed on almost all ZONESTAR 3d printers, including P802, M8, D805S, Z8, Z9, Z10 etc. series of products.   
![](./E4_size.jpg)   

#### :one: Installation
Simply remove the 3 screws behind the hot end assembly and install the E4 hotend assembly on the X carrier of the machine.
![](./E4-4.jpg)  

#### :two: Wiring
##### :loudspeaker: **Attention** 
- **Please watch for to distinguish terminals 3 and 4**, because their terminals  color are the same, but the wires color are different.    
If the wires of 3 and 4 are connected reversely, you can see the nozzle temperature displayed on the LCD screen will be much higher than the room temperature after you powered on the machine.
- When pluging the terminal, **be careful not to push the metal terminal from the plastic case**.     
#### :loudspeaker: **Please note**    
- **The cooling fan must be turned on** (when the temperature of the hot end is higher than 60°C), otherwise the hot end may be blocked or even damaged.  
 - By default, the **working voltage** of the fan and heater at the hot end is **DC 24V**. 
#### Please following the define of terminals to connect the hotend to your control board.
- Wiring of Z8P (Extend cable is omitted in the below picture)     
![](./E4_wiring_Z8P.jpg)  
- Wiring of Z9V5Pro     
![](./E4_wiring_Z9V5.jpg)  

#### :three: Set hot end type on LCD MENU: Control>>Configure>>Hotend Type
:warning: If your printer hasn't a 4.3" TFT-LCD screen, ignore this step.   
:warning: If you can't see the menu on the LCD screen of your printer, please upgrade to the newest version. [:link: **Firmware Download Link**](https://github.com/ZONESTAR3D/Firmware)    
![](./hotendtype-nonmix.jpg)  

----
### 5. Working principle
4-IN-1-OUT hot end is composed of fitting, heat-sink, heater, nozzle and other components, when printing, extrusion feeder insert one color filaments into the hot end, then the filament is melted and flowed from the nozzle, while need to chang to another color filament, the extruder pull the previous color filament out of the hot end, and then load another color filament. 
![](./E4-5.jpg)   
:movie_camera: [**Watch animation demonstration of E4 working principle**](./E4_principle.gif).   
#### :book: About "Wipe tower"  
Because there are still melted filaments of the previous color in the nozzle after a new color filament loaded, so we need to "clean" the nozzle before starting to print the new color filament. Otherwise, the printed initial part will be the previous color but not the new color as we expect. The solution is that to add **"wipe tower"** after switched to a new extruder in slicing software.    
About details, please refer to [**:point_right: Slicing**](#8-slicing).    
:bulb: Wipe tower is called "Prime tower" in Cura Slicer and "Prime Pillar" in Simplify3d Slicer. 

----
###  6. Pre-load filaments
#### 6.1 For one color printing
:movie_camera: [**How to load Filament - for one color printing**](https://youtu.be/6aTF5QnFhi4)
#### 6.2 For multi colors printing
:movie_camera: [**How to load Filament - for multi colors printing**](https://youtu.be/FyHrAMytlT8)      
Before printing, please pre-load the filaments into the appropriate position of the hot end so that the extruder can load smoothly the filaments into and out of the hot end.
- **Step 1:** Load filaments from the extruder and let the filaments extend about 10mm out of PTFE tubes.
- **Step 2:** Plug the PTFE tubes (with filaments) into the HOTEND.  
:pushpin: **If there is a filament in the hot end, heating and noozle and then pull it out first. Refer to [Unload filaments](#7-unload-filaments) to do it.**    
:pushpin: Cutting the front of filaments into a sharp shape before loading filament.     
:pushpin: If the extruder was not used during printing, donot need to load the filament to the hot end.   
![](./E4-6.jpg) 
:pushpin: Add some gcodes in the **"Start gcode"** ([:point_right: View](https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/Custom_Gcode.md#start-gcode)) of slicing software to print. 
![](./Preload_line.jpg)   
:pushpin: Add some gcodes in the **"End gcode"** ([:point_right: View](https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/Custom_Gcode.md#end-g-code)) of slicing software to pull out the last printed filament from the hotend.      

----
### 7. Unload filaments
Please follow the steps below to unload the filament from the hotend:
- **Step 1:** Heating the nozzle (190 degree for PLA and 230 degree for ABS).
- **Step 2:** Rotate gear of the extruder to unload the filament.   
:star2: Some 3d printers (e.g. Z9V5Pro) has a “Filament” Menu on LCD screen, please operate the LCD screen and use menu of ***“Prepare>>Filament”***  to preheat the nozzle, choose extruder and unload filaments.

----
### 8. Slicing
We have made user guide and video tutorial for PrusaSlicer/Cura/Simplify3d slicing software (PrusaSlicer is our recommended slicing software right now). For details, please refer to:   
- **PrusaSlicer(:+1:)**, please refer to :point_right: [**here**](https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer#6-slicing-muti-color-for-e4-hotend).
- **Cura slicer**, please refer to :point_right: [**here**](https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/cura).
- **Simplify3d Slicer**, please refer to :point_right: [**here**](https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/Simplify3D#slicing-video-toturial-for-z9v5-with-e4-hotend).

----
### 9. Testing gcode
We have uploaded some test files to our Github page, you can download them from [**here**](../example/readme.md).

----
### 10. Troubleshootings
If you encounter problems when using the E4 hot end, please refer to the [**troubleshootings guide**](../FAQ/readme.md) first to find a solutions. If the problem still can't be solved, please contact our technical support engineer by email: :email: support@zonestar3d.com.

  