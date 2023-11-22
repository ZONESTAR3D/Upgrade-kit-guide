# Dual Gear Extruder
### BMG Extruder
The BMG utilizes an internal gearing ratio of 3:1 together with precision CNC-machined hardened steel drive gears to give you a compact powerhouse for all your applications.
Whether you require high resolution prints with small nozzles or high-flow prints with big nozzles the optimized gearing ratio combined with our industry leading drive gears provides unparalleled pushing power and lightning fast retractions in a lightweight and compact package.
The extruder is sold without motor.
BMG is available in both left hand and right hand. 
### Technical Specification
- **Net weight:** 75g
- **Gross weight:** 139g
- **Package dimension:** 137×94×65mm
- **Gearing ratio:** 3:1
- **Filament diameter:** 1.75mm, Capable of supporting 2.85mm after simple modifications
- **Operating temperature:** 0–80°C
- **E-steps value:** 415
### Dimensions
![](BMG-Size.jpg)

### More information about BMG Extruder
- **[:clapper:Install BMG Extruder ](https://youtu.be/87OYybHhPFA)**
- **[:clapper:How a BMG extruder works and why it's so good](https://youtu.be/f2KTWnF3r1k)**

-----
## P802Q upgrade to Dual Gear Extruder
![](./P802Q/QR2_BMG.jpg)
### STEP:one: Print a bracket and install the Dual Gear Extruder
#### [:arrow_down:Download the stl file of bracket- left](./P802Q/BMG_BR_L.zip)
![](./P802Q/L1.jpg)
![](./P802Q/L2.jpg)
![](./P802Q/L3.jpg)
![](./P802Q/L4.jpg)
#### [:arrow_down:Download the stl file of bracket - right](./P802Q/BMG_BR_R.zip)
![](./P802Q/R1.jpg)
![](./P802Q/R2.jpg)
![](./P802Q/R3.jpg)
![](./P802Q/R4.jpg)
### STEP:two: Modify the motor wire to change the motor working direction
You may need to exchange the extruder stepping motor working direction after upgraded the dual gear extruder, you can simply modify the stepping motor wires to change it, for details, please refer to [:book:**this guide**](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/Motor_Driver#how-to-change-working-direction-by-exchange-motor-wiring).
### STEP:three: Change Esteps/mm settings on LCD screen
Because the double gear extruder build in a reduction gear, you need to modify the steps/mm parameter of the control board. You can use the following methods to modify the steps/mm parameter:    
1. **[Only valid for Marlin firmware]** -If your machine is using the latest Marlin firmware, you can modify the E Steps/mm parameter on the LCD menu (***Configuration>>Advance Settings>>Steps/mm>>E Steps/mm:***), usually you can change the parameter to 400. Then execute (***Configuration>>Store Settings***) to save the parameters to the NVRAM on the control board.
2. **[Valid for both Marlin and Repeater firmware]** - You can also add a "M92 E400" command in the Start G-code of the slicing software to set the steps/mm parameter. If you need to save the parameters to the NVRAM of the control board, you need to add a "M500" command following the M92 command.

<!-- -----
## Z9V5Pro upgrade to Dual Gear Extruder
**[:clapper: Video turorial]()** -->


