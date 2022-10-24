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
[![](../lanpic/SA.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=ar)
[![](../lanpic/CN.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=zh-CN)

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
## [4-IN-1-OUT Non-Mix Color (E4) Hotend](./E4%204-IN-1-OUT%20Non-Mixing%20Color%20Hotend/)
**E4 hotend** is a 4-IN-1-OUT non-mix color hotend, it has four input channels and one nozzle. One of the four filaments can be loaded into the heating block and extruded through the nozzle. When a new filament loaded in, it needs to unload the previous filament first.  
For details, please refer to [**here**](./E4%204-IN-1-OUT%20Non-Mixing%20Color%20Hotend/readme.md).  

## [4-IN-1-OUT Mix color (M4) Hotend](./M4%20%204-IN-1-OUT%20Mixing%20Color%20Hotend/)
**M4 hotend** is a 4-IN-1-OUT mix color hotend, it has four input channels and one nozzle. The filaments are mixed in the heating block and extruded through the nozzle.   
For details, please refer to [**here**](./M4%20%204-IN-1-OUT%20Mixing%20Color%20Hotend/readme.md). 

## [FAQ for E4 and M4 Hotend](./FAQ_M4E4.md)
- [**What's different between E4 and M4 hotend?**](https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/FAQ_M4E4.md#pushpin-advantages-and-disadvantages-of-e4-and-m4-hot-end)
- [**Which type of hot end should I choose?**](https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/FAQ_M4E4.md#pushpin-which-type-of-hot-end-should-i-choose-m4-or-e4)
- [**How to switch between M4 Hotend and E4 Hotend?**](https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/FAQ_M4E4.md#pushpin-which-type-of-hot-end-should-i-choose-m4-or-e4)

------
## [M3 (3-IN-1-OUT) Mix color Hotend](./M3%20%203-IN-1-OUT%20Mixing%20Color%20Hotend/)
**M3** hot end is a 3-IN-1-OUT mix color hotend, it has three input channels and one nozzle. Three filaments are mixed in the mixing chamber in the heating block and extruded through the nozzle.  
We have mass produced four versions of M3 hot end. For details, please refer to the documents in the "**M3 3-IN-1-OUT mixing color Hotend**" directory.  

## [M2P1 3-IN-2-OUT Mix Color Hotend](./M2P1%20%203-IN-2-OUT%20Mixing%20Color%20Hotend/)
**M2P1** hot end is a 3-IN-2-OUT mix color hotend, it has three input channels and two nozzles. Two filaments are mixed in the heating block and extruded through one of the nozzle, another independent nozzle can be used to print the support filament.   
Simply put, it is a combination of an M2 hot end and a single color hot end. It has the advantages of M2, singel nozzle hot end and double nozzle hot end. It can meet the needs of printing singel color, mixed color and two-color, as well as singel color+ support (such as PLA + PVA).

## [R3 3-IN-3-OUT Hotend](./R3%203-IN-3-OUT%20HOTEND/)
**R3** hot end is a 3-IN-3-OUT non-mix color hotend, it has three input channels and three nozzles, and all of the three nozzle share one heater and temperature sensor.  
For details, please refer to [here](./R3%203-IN-3-OUT%20HOTEND/readme.md).  

------
## [M2 (2-IN-1-OUT) Mix color Hotend](./M2%202_IN-1-OUT%20Mixing%20Color%20Hotend/)
**M2** hot end is a 2-IN-1-OUT mix color hotend, it has two input channels and one nozzle. Two filaments are mixed in the heating block and extruded through the nozzle.   
For details, please refer to [here](./M2%202_IN-1-OUT%20Mixing%20Color%20Hotend/readme.md).  

------
## [Single color Hotend](./Single%20color%20Hotend/)
[:book:Details](./Single%20color%20Hotend/readme.md).

------
## How to buy
### :one: One color Hotend 
#### Normal Flowrate hotend
[**Buy (Aliexpress)**](https://www.aliexpress.com/item/1005001275334841.html)
#### High Flowrate hotend
[**Buy (ZONESTAR Offical Store)**](https://bit.ly/3RF7ciR)    
[**Buy (Aliexpress)**](https://www.aliexpress.com/item/1005001275334841.html)
<!-- #### Ultra High Flowrate hotend -->
<!-- [**Buy (ZONESTAR Offical Store)**]() -->
<!-- [**Buy (Aliexpress)**] -->

### :two: 2 Colors Hot end (2-IN-1-OUT/2-IN-2-OUT)
[**Buy (Aliexpress)**](https://www.aliexpress.com/item/1005001285955926.html)

### :three: 3 Colors Hotend (3-IN-1-OUT/3-IN-2-OUT/3-IN-3-OUT)
[**Buy (ZONESTAR Offical Store)**](https://bit.ly/3z37ZUo)   
[**Buy (Aliexpress)**](https://www.aliexpress.com/item/1005001275429959.html)

### :four: 4 Colors Hot end
#### E4 Hot end
[**Buy (ZONESTAR Offical Store)**](https://bit.ly/39qDtKp)    
[**Buy (Aliexpress)**](https://www.aliexpress.com/item/1005002951777699.html)
#### M4V6 Hot end
[**Buy (ZONESTAR Offical Store)**](https://bit.ly/3QhWJtf)   
[**Buy (Aliexpress)**](https://www.aliexpress.com/item/1005004547646195.html)
#### M4V4 & M4V5 Hot end
[**Buy (Aliexpress)**](https://www.aliexpress.com/item/1005001581641783.html)

------
## [Slicing Guide for ZONESTAR 3D Printer](https://github.com/ZONESTAR3D/Slicing-Guide)
[:book:Details](https://github.com/ZONESTAR3D/Slicing-Guide)


