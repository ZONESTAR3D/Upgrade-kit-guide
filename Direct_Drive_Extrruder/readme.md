### :globe_with_meridians: Choose Language (Translated by google)
[![](../lanpic/ES.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder?_x_tr_sl=en&_x_tr_tl=es)
[![](../lanpic/FR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder?_x_tr_sl=en&_x_tr_tl=fr)
[![](../lanpic/PT.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder？_x_tr_sl=en&_x_tr_tl=pt)
[![](../lanpic/DE.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder？_x_tr_sl=en&_x_tr_tl=de)
[![](../lanpic/IT.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder？_x_tr_sl=en&_x_tr_tl=it)
[![](../lanpic/PL.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder？_x_tr_sl=en&_x_tr_tl=pl)
[![](../lanpic/RU.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder？_x_tr_sl=en&_x_tr_tl=ru)
[![](../lanpic/GR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder？_x_tr_sl=en&_x_tr_tl=el)
[![](../lanpic/JP.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder？_x_tr_sl=en&_x_tr_tl=ja)
[![](../lanpic/KR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder？_x_tr_sl=en&_x_tr_tl=ko)
[![](../lanpic/ID.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder？_x_tr_sl=en&_x_tr_tl=id)
[![](../lanpic/TH.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder？_x_tr_sl=en&_x_tr_tl=th)
[![](../lanpic/VN.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder？_x_tr_sl=en&_x_tr_tl=vi)
[![](../lanpic/IL.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder？_x_tr_sl=en&_x_tr_tl=iw)
[![](../lanpic/SA.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder？_x_tr_sl=en&_x_tr_tl=ar)
[![](../lanpic/TR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder？_x_tr_sl=en&_x_tr_tl=tr)
[![](../lanpic/CN.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide/Direct_Drive_Extrruder？_x_tr_sl=en&_x_tr_tl=zh-CN)

-----
## 1. Installation
:movie_camera:[**Video tutorial**](https://youtu.be/_s9Yc3zy6vw)
+ **Step 1**. Take down the orignal hotend from the x carrier.  
+ **Step 2**. Install the direct drive extruder (DDE ) to the same position of the carrier.  
![DDE_Installation](DDE_Installation.jpg)
## 2. Wiring
![Wiring](DDE_Wiring.jpg)
**if the stepper motor working direction is reserved, you can change change the stepping motor direction by modified the wire**  
![DDE_Installation](Change_motor_working_direction.jpg)  
## 3. Set the steps/mm parameter
**You may need to change the steps/mm parameter of the extruder, there are two method to set the steps/mm parameter**  
![](Set_steps_per_mm.jpg)
## 4. Reference
### How to install bed leveling sensor
![](Install_Bed_leveling_Sensor.jpg)
### To fix HOME X issue for Z9V5-MK1 and Z9V5-MK2
![](Install_Z9V5.jpg)
### How to open the control box
Lossen the four screws to open the upper control box and then you can find the wire for extrude motors, connect the wire to E1 motor connecotor.  
![](OpenZ9V5Box.jpg)
## 5. :point_right: [Print parts stl file](./stl/readme.md)  [:arrow_down:](./stl/stl.zip)

## 6. Correct X&Y offset
The hot bed center moves after replacing the extruder, you can set it on LCD screen if you care about it, please upload the newest firmware to your printer. Firmware Download link:    
- [**Z9V5**](https://github.com/ZONESTAR3D/Firmware/tree/master/Z9/Z9V5/bin)  
- [**Z8P**](https://github.com/ZONESTAR3D/Firmware/tree/master/Z8/Z8P/ZM3E4)  
