### :globe_with_meridians: Choose Language (Translated by google)
[![](../lanpic/ES.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=es)
[![](../lanpic/PT.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=pt)
[![](../lanpic/FR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=fr)
[![](../lanpic/RU.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=ru)
[![](../lanpic/IT.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=it)
[![](../lanpic/DE.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=de)
[![](../lanpic/PL.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=pl)
[![](../lanpic/KR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=ko)
[![](../lanpic/JP.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=ja)
[![](../lanpic/SA.png)](https://github-com.translate.goog/ZZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=ar)

# Hotend
The hotend is the component of a 3D printer that melts the filament for extrusion. Generally, the hot end consists of the following parts:

1. **Nozzle**: To melt filament and flow out， the size of its outlet determines the layer thickness can be built. It is usually made of materials with high thermal conductivity and high hardness, such as copper and carbon steel.  
2. **Heating block**: It is a device used to fix the heating rod and nozzle together. It is usually made of materials with high thermal conductivity, such as aluminum and copper.  
3. **Insulation block**: It is a device used to isolate the heater from the Heat sink, usually made of high temperature resistant but low thermal conductivity materials, such as stainless steel, PTFE, PEEK, etc..  
4. **Heat sink**: In order to fix the hot end to the printer and keep the consumables cool in front of the hot end to conduct extrusion pressure, the heat insulation block usually needs to be connected to the Heat sink, and then install the heat sink to the 3d printer.    
5. **Cooling fan**: Speed up the heat dissipation efficiency of the radiator, and there are also designs using water cooling methods.  
6. **Extrusion fan**: It be used to cool the colloid extruded from the nozzle so that the filaments can be formed and fixed as soon as possible.  
7. **Heater and temperature sensor**:  
> **Referance document:**[***Hot End Design Theory***](https://reprap.org/wiki/Hot_End_Design_Theory)  
![](hotend.jpg)  

------
## [Single color Hotend](./Single%20color%20Hotend/)
Included documents about ZONESTAR single color hot end

------
## [M2 (2-IN-1-OUT)  Mixing color hotend](./M2%202_IN-1-OUT%20Mixing%20Color%20Hotend/)
**M2** hot end is a 2-IN-1-OUT hotend, it has two feeding channels and one nozzle. Two filaments are mixed in the mixing chamber in the heating block and extruded through the nozzle.  
We have mass produced four versions of M2 hot end. For details, please refer to the documents in the "**M2 2-IN-1-OUT mixing color Hotend**" directory.  

------
## [M3 (3-IN-1-OUT) Mixing color hotend](./M3%20%203-IN-1-OUT%20Mixing%20Color%20Hotend/)
**M3** hot end is a 3-IN-1-OUT hotend, it has three feeding channels and one nozzle. Three filaments are mixed in the mixing chamber in the heating block and extruded through the nozzle.  
We have mass produced four versions of M3 hot end. For details, please refer to the documents in the "**M3 3-IN-1-OUT mixing color Hotend**" directory.  

## [M2P1 3-IN-2-OUT Mixing Color Hotend](./M2P1%20%203-IN-2-OUT%20Mixing%20Color%20Hotend/)
**M2P1** hot end is a 3-IN-2-OUT hotend, it has three feeding channels and two nozzle. Two filaments are mixed in the mixing chamber in the heating block and extruded through one of the nozzle, another independent nozzle can be used to print the support filament.   
Simply put, it is a combination of an M2 hot end and a single color hot end. It has the advantages of M2, singel nozzle hot end and double nozzle hot end. It can meet the needs of printing singel color, mixed color and two-color, as well as singel color+ support (such as PLA + PVA).

## [R3 3-IN-3-OUT HOTEND](./R3%203-IN-3-OUT%20HOTEND/)
**R3** hot end is a 3-IN-3-OUT hotend, it has three feeding channels and three nozzles, and all of the three nozzle share one heater and temperature sensor.  
We have mass produced 2 versions of R3 hot end. For details, please refer to the documents in the "**R3 3-IN-3-OUT HOTEND**" directory.  

------
## [M4(4-IN-1-OUT Mixing color) hotend](./M4%20%204-IN-1-OUT%20Mixing%20Color%20Hotend/)
**M4** hot end is a 4-IN-1-OUT hotend, it has four feeding channels and one nozzle. Four filaments are mixed in the mixing room in the heating block and extruded through the nozzle. For details, please refer to [**here**](./M4%20%204-IN-1-OUT%20Mixing%20Color%20Hotend/readme.md).  

## [E4 (4-IN-1-OUT Non-Mix Color) Hotend](./E4%204-IN-1-OUT%20Non-Mixing%20Color%20Hotend/)
**E4** hot end is a 4-IN-1-OUT hotend, it has four feeding channels and one nozzle. One of the four filaments can be pushed in the heating block and extruded through the nozzle, When a new filament push in, it needs to pull out the previous filament first.
For details, please refer to [**here**](./E4%204-IN-1-OUT%20Non-Mixing%20Color%20Hotend/readme.md).  

### Advantages and disadvantages of E4 and M4 hot end
- M4 hotend has a mix color room, it can mix different color filament to another colors. E4 hotend hasn't mix color room, it only print only one filament color at once.  
- E4 hotend is good at printing one color 3d prints or multi colos 3d prints (up to 4 colors).
- M4 hotend is good at printing gradient color 3d prints, it can print one color and over 4 colos 3d object too.
#### Advantages of E4 hotend
1. No strings/drawing issue.
2. Less clogging issue.
3. Smaller "extruder switch prime tower" inneed while printing multi colors.
#### Advantages of M4 hotend
1. Get more colors than extruders.
2. Support gradient color printing feature.
![](M4VSE4.jpg)

### Which type of hot end should I choose, M4 or E4?
- If you do not need to print gradient color 3d model, we suggest you choose E4 hotend, it can get better quality on printing one color and multi colors 3d prints.
- If you want to print gradient color 3d model, or you want to mix different color filaments to another color, you need to choose M4 hotend.

### How to switch between mix color Hotend and non-mix color Hotend
#### 1. Loosen the three screws on the hot end housing and remove the old hot end from the machine (x pulley). Then install the new hot end on the machine (x pulley) and lock the screws.
![](./E4%204-IN-1-OUT%20Non-Mixing%20Color%20Hotend/User_guide/E4-4.jpg)
#### 2. Connect the wires of the new hot end to the machine.
![](./E4%204-IN-1-OUT%20Non-Mixing%20Color%20Hotend/User_guide/E4_wiring.jpg)
#### 3. Set the hot end type on the LCD menu: *Control>>Configure>>Hotend Type*
![](./E4%204-IN-1-OUT%20Non-Mixing%20Color%20Hotend/User_guide/hotendtype-mix.jpg)![](./E4%204-IN-1-OUT%20Non-Mixing%20Color%20Hotend/User_guide/hotendtype-nonmix.jpg)
#### :warning: NOTE 1: If you can't find the hotend type menu on LCD screen, please upload the newest firmware to your printer 
:point_right: Firmware for [**[Z9V5]**](https://github.com/ZONESTAR3D/Firmware/tree/master/Z9/Z9V5/bin)  [**[Z8P]**](https://github.com/ZONESTAR3D/Firmware/tree/master/Z8/Z8P/ZM3E4/released)  [**[Z9M4]**](https://github.com/ZONESTAR3D/Firmware/tree/master/Z9/Z9M4)
#### :warning: NOTE 2: The mix color Hotend and non-mix color hotend must use different slice settings, please pay attention to distinguish. Using the wrong slice setting may cause the hotend to be blocked.

------
# [Slicing Guide](https://github.com/ZONESTAR3D/Slicing-Guide)
Please refer to the [:point_right: guide](https://github.com/ZONESTAR3D/Slicing-Guide)



