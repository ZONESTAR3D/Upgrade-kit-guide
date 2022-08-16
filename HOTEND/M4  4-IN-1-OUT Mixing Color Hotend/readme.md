# ZONESTAR M4 (4-IN-1-OUT Mixing Color) Hotend



## M4V6 - The 6th version 4-IN-1-OUT mix color hotend
[:book: Introduction of the 6th M4 hotend](./M4_V6/readme.md)  
### Structure diagram
![](./M4_V6/M4V6_2.JPG)
### What's improved
The M4V6 has reformed the structure of the hot end, which is completely different from the previous version. It uses an inclined feed channel and canceled the flow channel inside the heater. Advantages compared with the previous version M4 hot ends:
1. Solved the leakage issue completely.
2. Reduced the volume of mixing room, the drawing/stings issue is greatly improved.


## M4V5 - The 5th version 4-IN-1-OUT mix color hotend
[:book: Introduction of the 5th version M4 hotend](./M4_V5/readme.md)
### Structure diagram
![](./M4_V5/M4V5.jpg)
### The different between **M4V5** with **M4V4**:  
1. Removed the inner PTEF pipes, Reduce the probability of clogged because the internal PTEF pipe be damaged.   
2. Upgraded the fittings, easier to load filament and replace the filament guide. 
### :warning: ATTETION PLEASE
Because M4V5 used different fittings which to fix the PTFE filament guides, its size is bigger than M4V3 and M4V4, so M4V5 can't be installed to the older housing.   


## M4V4 - The 4th version 4-IN-1-OUT mix color hotend
[:book: Introduction of the 4th M4 hotend](./M4_V3_V4/readme.md)      
[**Buy a M4 Hotend**](https://www.aliexpress.com/item/1005002124027691.html)  
[**Buy a M4 Hotend assembly**](https://www.aliexpress.com/item/1005001581641783.html) 

### Structure diagram
![](./M4_V3_V4/M4_V4.jpg)
### The different between  **M4V4** with **M4V3**:  
1. Upgraded the insulation block material from **PETF** to **PEEK**, so M4-V4 can work at maxius temperature to 260℃.  
![](./M4_V3_V4/PEEK_Insulation_block.jpg)
2. Upgraded the nozzle to a "Small store room nozzle" to improve the strings issue.
![](./M4_V3_V4/small_store_room_nozzle.jpg)  

### Get the upgrade parts
[**PEEK_Insulation_block**](https://www.aliexpress.com/item/1005002124027691.html)  
[**Small store room nozzle**](https://www.aliexpress.com/item/1005001447928770.html)

## M4V3 - The 3rd version 4-IN-1-OUT mix color hotend
[:book: Introduction of the 3rd M4 hotend](./M4_V3_V4/readme.md)
### Structure diagram
![](./M4_V3_V4/M4_V3.jpg)

## stl
Stl files of the fan duck
- :arrow_down: [Fan duck for M4V3 M4V4 & M4V5](./stl/fan_duck_m4_v3.rar)
- :arrow_down: [Fan duck for M4V6](./stl/fan_duck_m4_v6.rar)

## Example
gcode/stl files to print by using M4 hotend and slicing settings 
![4_Color_Dog](./Example/4_Color_Dog/M4_4C_Dog.jpg)  
![4_Color_owl](./Example/4_Color_owl/M4_4Color_owl.jpg)  
![6_Color_Patrick](./Example/6_Color_Patrick/M4_6Color_Patrick.jpg)  



## :bug: Issues of the mixing color hotend 
### 1. Clogged issue
#### :question: Reasons
1. The length of the extrusion channel is longer than that of the single color.   
![](Issue_mixing_1.jpg)       
2. Since the channels at the hot end of the color mixing are interconnected, the filaments in the feed channels are also under the action of the reverse extrusion force of the other channels at the same time.  
![](Issue_mixing_2.jpg)    
3. The longer of the filament between Tg(Glass Transition Temperature) and Tm(Melting Temperature), the greater its adhesion to the feed tube (refer to [***Hot End Design Theory***](https://reprap.org/wiki/Hot_End_Design_Theory)), and the final result will be that the extrusion feeder can't push the filament.  
![](Issue_mixing_3.jpg)   
4. Other reasons: Due to weight, processing and installation restrictions, the distance between the extruder feeder and the hot end needs to be longer, it also increases the resistance of the extruder.  
#### :pill: Solutions 
1. Increase extruder force, for exmple upgrade to [**Dual gear extruder**](https://www.aliexpress.com/item/1005003473360998.html) or [**Titan extruder**](https://www.aliexpress.com/item/1005001678239017.html) .  
2. Choose harder filaments, for example **PLA+** > **PLA** > **silk-PLA**.  
3. Reduce the heat transfer rate of **Insulation block** and keep the "Heat sink" cool, to short the filament distance between Tg and Tm.  
4. Minimize the length of the mixing chamber channels.   
5. Improve retraction settings.  
6. Do not leave the channel unused for a long time, filament in Tg state for a long time will be more firmly attached to the filament guide.
 
### 2. Strings issue
#### :question: Reasons
Because there is a mixing color chamber, so the stored filaments in the mixing color hotend is bigger than single color hotend, it will reduce the effect of retraction.  
![](Issue_mixing_4.jpg)   
#### :pill: Solutions  
##### 1. Reduce the size of mixing color chamber, for example, upgrade to [**small store room nozzle**](https://www.aliexpress.com/item/1005001447928770.html).  
##### 2. Add "wipe" on silcing settings.
###### Cura Slicer (Coasting)
![Cura](curawipe.png)
###### PrusaSlicer (Wipe while retracting)
![PrusaSlicer](prusawipe.png)
##### 3. Synchronous retract to use multiple extruders. It called "Auto Retraction" or "FW Retract" too, about detail, please refer to [Here](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/M4%20%204-IN-1-OUT%20Mixing%20Color%20Hotend/Example#use-auto-retraction-function-to-improve-stings-issue)
##### 4. If you are very concerned about strings issue, it is recommended that you buy a single color or 4-IN-1-OUT Non-mixing color Hotend.
- :package: [**Single color Hotend**](https://www.aliexpress.com/item/1005002829919346.html)
- :package: [**Direct Drive Extruder**](https://fr.aliexpress.com/item/1005002847644867.html)
- :package: [**4-IN-1-OUT Non-Mixing Color (E4) Hotend**](https://www.aliexpress.com/item/1005002951777699.html)



