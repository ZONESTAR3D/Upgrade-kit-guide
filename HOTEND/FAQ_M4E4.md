## FAQ for E4 and M4 hot end
- [**What's different between E4 and M4 hotend?**](#whats-different-between-e4-and-m4-hotend)
- [**Which type of hot end should I choose?**](#which-type-of-hot-end-should-i-choose-m4-or-e4)
- [**How to switch between M4 Hotend and E4 Hotend?**](#how-to-switch-between-m4-hotend-and-e4-hotend)

----
### What's different between E4 and M4 hotend?
- **M4 hotend** has a mix color room, it can mix different color filament to another colors. **E4 hotend** hasn't mix color room, it only print only one filament color at once.  
- **E4 hotend** is good at printing one color 3d prints or multi colos 3d prints (up to 4 colors).
- **M4 hotend** is good at printing gradient color 3d prints, it can print one color and over 4 colos 3d object too.
#### Advantages of E4 hotend
1. No strings/drawing issue.
2. Less clogging issue.
3. Smaller "extruder switch prime tower" inneed while printing multi colors.
#### Advantages of M4 hotend
1. Get more colors than extruders.
2. Support gradient color printing feature.
![](M4VSE4.jpg)

----
### Which type of hot end should I choose, M4 or E4?
- If you **do not need** to print gradient color 3d model, we suggest you choose **E4 hotend**, it can get better quality on printing single color and multi colors 3d prints.
- If you want to print **gradient color** 3d model, or you want to **mix different color filaments to another color**, choose M4 hotend.

----
### How to switch between M4 Hotend and E4 Hotend
#### 1. Loosen the three screws on the hot end housing and remove the old hot end from the machine (x pulley). Then install the new hot end on the machine (x pulley) and lock the screws.
![](./E4%204-IN-1-OUT%20Non-Mixing%20Color%20Hotend/User_guide/E4-4.jpg)
#### 2. Connect the wires of the new hot end to the machine.
![](./E4%204-IN-1-OUT%20Non-Mixing%20Color%20Hotend/User_guide/E4_wiring.jpg)
#### 3. Set the hot end type on the LCD menu: *Control>>Configure>>Hotend Type*
![](./E4%204-IN-1-OUT%20Non-Mixing%20Color%20Hotend/User_guide/hotendtype-mix.jpg)![](./E4%204-IN-1-OUT%20Non-Mixing%20Color%20Hotend/User_guide/hotendtype-nonmix.jpg)
#### :warning: NOTE 1: If you can't find the hotend type menu on LCD screen, please upload the newest firmware to your printer 
:point_right: Firmware for [**[Z9V5]**](https://github.com/ZONESTAR3D/Firmware/tree/master/Z9/Z9V5/bin)  [**[Z8P]**](https://github.com/ZONESTAR3D/Firmware/tree/master/Z8/Z8P/ZM3E4/released)  [**[Z9M4]**](https://github.com/ZONESTAR3D/Firmware/tree/master/Z9/Z9M4)
#### :warning: NOTE 2: The mix color Hotend and non-mix color hotend must use different slice settings, please pay attention to distinguish. Using the wrong slice setting may cause the hotend to be blocked.


