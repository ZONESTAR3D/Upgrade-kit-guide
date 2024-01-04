### :globe_with_meridians: Choose Language (Translated by google)
[![](../lanpic/ES.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=es)
[![](../lanpic/PT.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=pt)
[![](../lanpic/FR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=fr)
[![](../lanpic/DE.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=de)
[![](../lanpic/IT.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=it)
[![](../lanpic/SW.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=sv)
[![](../lanpic/PL.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=pl)
[![](../lanpic/DK.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=da)
[![](../lanpic/CZ.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=cs)
[![](../lanpic/HR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=hr)
[![](../lanpic/RO.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=ro)
[![](../lanpic/SK.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=sk)

[![](../lanpic/RU.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=ru)
[![](../lanpic/JP.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=ja)
[![](../lanpic/KR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=ko)
[![](../lanpic/ID.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=id)
[![](../lanpic/TH.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=th)
[![](../lanpic/VN.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=vi)
[![](../lanpic/IL.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=iw)
[![](../lanpic/SA.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=ar)
[![](../lanpic/TR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=tr)
[![](../lanpic/GR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=el)
[![](../lanpic/BR.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=pt)
[![](../lanpic/CN.png)](https://github-com.translate.goog/ZONESTAR3D/Upgrade-kit-guide?_x_tr_sl=en&_x_tr_tl=zh-CN)

-----
## :warning: ATTENTION PLEASE
- **Power off the control board before replacing/plugin the drive module.**
- **Pay attention to the direction when plugin, incorrect direction may burn the drivers and control board.**
- **Usually we have already set the motor drive current before shipping out, please don't tune the potentiometer if you are not sure how to adjust it.**
![](1.jpg)
### How to change working direction by exchange motor wiring 
You may need to change the stepper motor working direction after replaced the motor drivers, such as replaced A4988 to TMC2208, you can upgrade the appropriate firmware to the control board or adjust the motor wiring to reserved the motor working direction.
- Simply exchange PIN1 and PIN3 of the motor cable, the stepping motor working direction will be reversed.
![](2.jpg)
- TIPS: Use a knife to turn up the clip of the terminal and then pull out the wiring
![](3.jpg)

### How to adjust drive current
If you want to adjust the current of the motor driver module, please measure the voltage (Vref) on the potentiometer with a multimeter.
:warning:NOTE:warning:  
- **Diconnected the motor wire and then supply power to the control board.**
- **For A4988 drive module, you can supply power to the control board from USB, but for TMC drive module, it must supply power to the control board from DC terminal.**
![](4.jpg)


