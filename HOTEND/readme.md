### :globe_with_meridians: Choose Language (Translated by google)
[![](../lanpic/ES.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=es)
[![](../lanpic/PT.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=pt)
[![](../lanpic/FR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=fr)
[![](../lanpic/DE.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=de)
[![](../lanpic/IT.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=it)
[![](../lanpic/SW.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=sv)
[![](../lanpic/PL.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=pl)
[![](../lanpic/DK.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=da)
[![](../lanpic/CZ.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=cs)
[![](../lanpic/HR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=hr)
[![](../lanpic/RO.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=ro)
[![](../lanpic/SK.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=sk)

[![](../lanpic/RU.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=ru)
[![](../lanpic/JP.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=ja)
[![](../lanpic/KR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=ko)
[![](../lanpic/ID.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=id)
[![](../lanpic/TH.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=th)
[![](../lanpic/VN.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=vi)
[![](../lanpic/IL.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=iw)
[![](../lanpic/SA.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=ar)
[![](../lanpic/TR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=tr)
[![](../lanpic/GR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=el)
[![](../lanpic/BR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=pt)
[![](../lanpic/CN.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND?_x_tr_sl=en&_x_tr_tl=zh-CN)

-----
# Hotend
The hotend is the component of a 3D printer that melts the filament for extrusion. Generally, the hot end consists of the following parts:

1. **Nozzle**: To melt filament and flow out，the size of its outlet determines the layer thickness can be built. It is usually made of materials with high thermal conductivity and high hardness, such as copper, carbon steel.  
2. **Heating block**: It is a device used to fix the heater and nozzle together. It is usually made of materials with high thermal conductivity, such as aluminum and copper. In some designs, the nozzle and heating block may be integrated.
3. **Heat break**: It is a device used to isolate the heater from the printer, usually made of high temperature resistant but low thermal conductivity materials, such as stainless steel, PEEK, PEI, etc..  
4. **Heat sink**: In order to fix the hot end to the printer and keep the filaments cool in front of the hot end to conduct extrusion pressure, the heat break usually needs to be connected to the heat sink, and then install the heat sink to the 3d printer.    
5. **Cooling fan**: Speed up the heat dissipation efficiency of the heat sink, and there are also designs using water cooling methods.  
6. **Extrusion fan**: It be used to cool the colloid flowed out from the nozzle so that the filaments can be formed and fixed ASAP.  
7. **Heater**: It be used to heat the nozzle, usually using a 40W~60W cartridge heater.
8. **temperature sensor**: The 100K NTC thermistor is usually used to measure the temperature of the hot end.
> **Referance document:**[***Hot End Design Theory***](https://reprap.org/wiki/Hot_End_Design_Theory)  
![](hotend.jpg)  

------
## 4 Extruders Hotend
### :file_folder: [E4 (4-IN-1-OUT Non-Mix Color) Hotend](./E4%204-IN-1-OUT%20Non-Mixing%20Color%20Hotend/)
**E4 hotend** is a 4-IN-1-OUT non-mix color hotend, it has four input channels and one nozzle. One of the four filaments can be loaded into the heating block and extruded through the nozzle. When a new filament loaded in, it needs to unload the previous filament first.  
For details, please refer to [**here**](./E4%204-IN-1-OUT%20Non-Mixing%20Color%20Hotend/readme.md).  

### :file_folder: [M4 (4-IN-1-OUT Mix color) Hotend](./M4%20%204-IN-1-OUT%20Mixing%20Color%20Hotend/)
**M4 hotend** is a 4-IN-1-OUT mix color hotend, it has four input channels and one nozzle. The filaments are mixed in the heating block and extruded through the nozzle.   
For details, please refer to [**here**](./M4%20%204-IN-1-OUT%20Mixing%20Color%20Hotend/readme.md). 

### :file_folder: [FAQ for E4 and M4 Hotend](./FAQ_M4E4.md)
- [**What's different between E4 and M4 hotend?**](https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/FAQ_M4E4.md#pushpin-advantages-and-disadvantages-of-e4-and-m4-hot-end)
- [**Which type of hot end should I choose?**](https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/FAQ_M4E4.md#pushpin-which-type-of-hot-end-should-i-choose-m4-or-e4)
- [**How to switch between M4 Hotend and E4 Hotend?**](https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/FAQ_M4E4.md#pushpin-which-type-of-hot-end-should-i-choose-m4-or-e4)

------
## 3 Extruders Hotend
### :file_folder: [M3 (3-IN-1-OUT Mix color) Hotend](./M3%20%203-IN-1-OUT%20Mixing%20Color%20Hotend/)
**M3** hot end is a 3-IN-1-OUT mix color hotend, it has three input channels and one nozzle. Three filaments are mixed in the mixing chamber in the heating block and extruded through the nozzle.  
We have mass produced four versions of M3 hot end. For details, please refer to the documents in the "**M3 3-IN-1-OUT mixing color Hotend**" directory.  

### :file_folder: [M2P1 (3-IN-2-OUT Mix Color) Hotend](./M2P1%20%203-IN-2-OUT%20Mixing%20Color%20Hotend/)
**M2P1** hot end is a 3-IN-2-OUT mix color hotend, it has three input channels and two nozzles. Two filaments are mixed in the heating block and extruded through one of the nozzle, another independent nozzle can be used to print the support filament.   
Simply put, it is a combination of an M2 hot end and a single color hot end. It has the advantages of M2, singel nozzle hot end and double nozzle hot end. It can meet the needs of printing singel color, mixed color and two-color, as well as singel color+ support (such as PLA + PVA).

### :file_folder: [R3 (3-IN-3-OUT Non-Mix color) Hotend](./R3%203-IN-3-OUT%20HOTEND/)
**R3** hot end is a 3-IN-3-OUT non-mix color hotend, it has three input channels and three nozzles, and all of the three nozzle share one heater and temperature sensor.  
For details, please refer to [**here**](./R3%203-IN-3-OUT%20HOTEND/readme.md).  

------
## 2 Extruders Hotend
### :file_folder: [M2 (2-IN-1-OUT Mix color) Hotend](./M2%202_IN-1-OUT%20Mixing%20Color%20Hotend/)
**M2** hot end is a 2-IN-1-OUT mix color hotend, it has two input channels and one nozzle. Two filaments are mixed in the heating block and extruded through the nozzle.   
For details, please refer to [**here**](./M2%202_IN-1-OUT%20Mixing%20Color%20Hotend/readme.md).  

### :file_folder: [R2S (2-IN-2-OUT Non-Mix color) Hotend]()
**R2S** hot end is a 2-IN-2-OUT hotend, it has two input channels and 2 nozzles. Two filaments can be loaded into the heating block and extruded through the nozzle.   
For details, please refer to [**here**](). 

------
## One Extruder /One Color Hotend
### :file_folder: [Single color Hotend](./Single%20color%20Hotend/)
[:book:Details](./Single%20color%20Hotend/readme.md).
### :file_folder: [High Flow Hotend]()
[:book:Details]().
<!-- ### :file_folder: [High Flow Hotend]()
[:book:Details](). -->

------
## :file_folder: [Slicing Guide for ZONESTAR 3D Printer](https://github.com/ZONESTAR3D/Slicing-Guide)
[:book:Details](https://github.com/ZONESTAR3D/Slicing-Guide)

------
## :gift: How to buy
### :one: One color Hotend 
#### Normal Flowrate hotend
[**Buy (Aliexpress)**](https://www.aliexpress.com/item/1005001275334841.html)
#### High Flowrate hotend
[**Buy (ZONESTAR Offical Store)**](https://bit.ly/3RF7ciR)    
[**Buy (Aliexpress)**](https://www.aliexpress.com/item/1005001275334841.html)
<!-- #### Ultra High Flowrate hotend -->
<!-- [**Buy (ZONESTAR Offical Store)**]() -->
<!-- [**Buy (Aliexpress)**] -->

### :two: 2 Extruders Hotend (2-IN-1-OUT/2-IN-2-OUT)
[**Buy (Aliexpress)**](https://www.aliexpress.com/item/1005001285955926.html)

### :three: 3 Extruders Hotend (3-IN-1-OUT/3-IN-2-OUT/3-IN-3-OUT)
[**Buy (ZONESTAR Offical Store)**](https://bit.ly/3z37ZUo)   
[**Buy (Aliexpress)**](https://www.aliexpress.com/item/1005001275429959.html)

### :four: 4 Extruders Hotend (4-IN-1-OUT Mix Color Hotend  and 4-IN-1-OUT Non-mix Color Hotend)
#### E4 (4-IN-1-OUT Non-mix Color) Hotend
[**Buy (ZONESTAR Offical Store)**](https://bit.ly/39qDtKp)    
[**Buy (Aliexpress)**](https://www.aliexpress.com/item/1005002951777699.html)
#### M4V6 (Newest Version 4-IN-1-OUTmix Color) Hotend
[**Buy (ZONESTAR Offical Store)**](https://bit.ly/3QhWJtf)   
[**Buy (Aliexpress)**](https://www.aliexpress.com/item/1005004547646195.html)
#### M4V4 & M4V5 (Older Version 4-IN-1-OUTmix Color) Hotend
[**Buy (Aliexpress)**](https://www.aliexpress.com/item/1005001581641783.html)




