# Hotend
The hotend is the component of a extruder of the FDM 3D printer that melts the filament. Generally, a hot end consists of the following parts:
1. **Nozzle**: To melt filament and flow out，the size of its outlet determines the layer thickness can be built. It is usually made of materials with high thermal conductivity and high hardness, such as copper, carbon steel.  
2. **Heating block**: It is a device to fix the heater and nozzle together. It is usually made of materials with high thermal conductivity, such as aluminum and copper. In some designs, the nozzle and heating block may be integrated.
3. **Heat break**: It is a device used to isolate the heater from the printer, usually made of high temperature resistant but low thermal conductivity materials, such as stainless steel, PEEK, titanium, etc..  
4. **Heat sink**: In order to fix the hot end and keep the filaments cool in front of the hot end to conduct extrusion pressure, the heat break usually needs to be connected to a heat sink, and then install the heat sink to the 3d printer.    
5. **Cooling fan**: Speed up the heat dissipation efficiency of the heat sink, and there are also designs using water cooling methods.  
6. **Extruder fan**: It be used to cool the colloid flowed out from the nozzle so that the filaments can be formed and fixed ASAP.  
7. **Heater**: It be used to heat the nozzle, usually using a 40W~60W cartridge heater.
8. **Temperature sensor**: For measuring the temperature of the hot block (nozzle).
![](hotend.jpg)      
:link: **Referance document @ Reprap: [Hot End Design Theory](https://reprap.org/wiki/Hot_End_Design_Theory)**      

------
## 4 Channels Hotend
### :file_folder: [E4 (4-IN-1-OUT Non-Mix Color) Hotend](./E4/)
**E4 hotend** is a 4-IN-1-OUT non-mix color hotend, it has four input channels and one nozzle. One of the four filaments can be loaded into the heating block and extruded through the nozzle. When a new filament loaded in, it needs to unload the previous filament first.  
For details, please refer to [**here**](./E4/readme.md).  

### :file_folder: [M4 (4-IN-1-OUT Mix color) Hotend](./M4/)
**M4 hotend** is a 4-IN-1-OUT mix color hotend, it has four input channels and one nozzle. The filaments are mixed in the heating block and extruded through the nozzle.   
For details, please refer to [**here**](./M4/readme.md). 

### :file_folder: [FAQ for E4 and M4 Hotend](./FAQ_M4E4.md)
- [**What's different between E4 and M4 hotend?**](https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/FAQ_M4E4.md#pushpin-advantages-and-disadvantages-of-e4-and-m4-hot-end)
- [**Which type of hot end should I choose?**](https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/FAQ_M4E4.md#pushpin-which-type-of-hot-end-should-i-choose-m4-or-e4)
- [**How to switch between M4 Hotend and E4 Hotend?**](https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/FAQ_M4E4.md#pushpin-which-type-of-hot-end-should-i-choose-m4-or-e4)

------
## 3 Channels Hotend
### :file_folder: [M3 (3-IN-1-OUT Mix color) Hotend](./M3/)
**M3** hot end is a 3-IN-1-OUT mix color hotend, it has three input channels and one nozzle. Three filaments are mixed in the mixing chamber in the heating block and extruded through the nozzle.  
We have mass produced four versions of M3 hot end. For details, please refer to the documents in the "**M3 3-IN-1-OUT mixing color Hotend**" directory.  

### :file_folder: [M2P1 (3-IN-2-OUT Mix Color) Hotend](./M2P1/)
**M2P1** hot end is a 3-IN-2-OUT mix color hotend, it has three input channels and two nozzles. Two filaments are mixed in the heating block and extruded through one of the nozzle, another independent nozzle can be used to print the support filament.   
Simply put, it is a combination of an M2 hot end and a single color hot end. It has the advantages of M2, singel nozzle hot end and double nozzle hot end. It can meet the needs of printing singel color, mixed color and two-color, as well as singel color+ support (such as PLA + PVA).

### :file_folder: [R3 (3-IN-3-OUT Non-Mix color) Hotend](./R3/)
**R3** hot end is a 3-IN-3-OUT non-mix color hotend, it has three input channels and three nozzles, and all of the three nozzle share one heater and temperature sensor.  
For details, please refer to [**here**](./R3/readme.md).  

------
## 2 Channels Hotend
### :file_folder: [M2 (2-IN-1-OUT Mix color) Hotend](./M2/)
**M2** hot end is a 2-IN-1-OUT mix color hotend, it has two input channels and one nozzle. Two filaments are mixed in the heating block and extruded through the nozzle.   
For details, please refer to [**here**](./M2/readme.md).  

### :file_folder: [R2 (2-IN-2-OUT Non-Mix color) Hotend](./R2/)
**R2** hot end is a 2-IN-2-OUT hotend, it has two input channels and 2 nozzles. Two filaments can be loaded into the heating block and extruded through the nozzle.   
**R2S** is similar to **R2** hot end, but the two nozzles of R2S share the same heater and temperature sensor, so the temperatures of the two channels of R2S hot end cannot be set separately.     
For details, please refer to [**here**](./R2/). 

------
## One Color Hotend
### :file_folder: [Single color Hotend](./Single_color/)
[:book:Details](./Single_color/readme.md).
### :file_folder: [High Flow Hotend]()
[:book:Details]().

<!-- ------
## :file_folder: [Slicing Guide for ZONESTAR 3D Printer](https://github.com/ZONESTAR3D/Slicing-Guide)
[:book:Details](https://github.com/ZONESTAR3D/Slicing-Guide) -->

------
## :gift: How to buy
- **One color Hotend**   
  - **General Flowrate one color hotend** [**:gift: Buy (Aliexpress)**](https://www.aliexpress.com/item/1005001275334841.html)
  - **High Flowrate one color hotend** [**:gift: Buy (Official Store)**](https://bit.ly/3RF7ciR) [**:gift: Buy (Aliexpress)**](https://www.aliexpress.com/item/1005001275334841.html)
- **2 Channels Hotend (2-IN-1-OUT/2-IN-2-OUT)**
[**:gift: Buy (Aliexpress)**](https://www.aliexpress.com/item/1005001285955926.html)
- **3 Channels Hotend (3-IN-1-OUT/3-IN-2-OUT/3-IN-3-OUT)** [**:gift: Buy (Official Store)**](https://bit.ly/3z37ZUo)   [**:gift: Buy (Aliexpress)**](https://www.aliexpress.com/item/1005001275429959.html) 
- **4 Channels Hotend (M4 Hotend and E4 Hotend)**
  - **E4 (4-IN-1-OUT Non-mix Color) Hotend**
  [**:gift: Buy (Official Store)**](https://bit.ly/39qDtKp) [**:gift: Buy (Aliexpress)**](https://www.aliexpress.com/item/1005002951777699.html)
  - **M4V6 Hotend**
  [**:gift: Buy (Official Store)**](https://bit.ly/3QhWJtf)  [**:gift: Buy (Aliexpress)**](https://www.aliexpress.com/item/1005004547646195.html)
  - **M4V4 & M4V5 (Older Version 4-IN-1-OUTmix Color) Hotend**
  [**:gift: Buy (Aliexpress)**](https://www.aliexpress.com/item/1005001581641783.html)




