[E4_STARTGCODE]: https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/Custom_Gcode.md#start-g-code
[M4_MIXMULTICOLORPRINT]: https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/PrusaSlicerGuide_M4.md#how-to-print-more-than-4-colors-using-m4-hot-end
[E4_TOOLCHANGE]: https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/Custom_Gcode.md#tool-change-g-code
[FW_Z9V5]: https://github.com/ZONESTAR3D/Firmware/tree/master/Z9/Z9V5/bin
[FW_Z9M4]: https://github.com/ZONESTAR3D/Firmware/tree/master/Z9/Z9M4
[FW_Z8P]: https://github.com/ZONESTAR3D/Firmware/tree/master/Z8/Z8P

----
## <a id="choose-language">:globe_with_meridians: Choose language </a>
[![](../lanpic/EN.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4.md)
[![](../lanpic/ES.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-es.md)
[![](../lanpic/PT.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-pt.md)
[![](../lanpic/FR.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-fr.md)
[![](../lanpic/DE.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-de.md)
[![](../lanpic/IT.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-it.md)
[![](../lanpic/RU.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-ru.md)
[![](../lanpic/JP.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-jp.md)
[![](../lanpic/KR.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-kr.md)
<!-- [![](../lanpic/SA.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-ar.md) -->

----
# Preguntas frecuentes sobre hotend E4 y M4
- [**¿Cuál es la diferencia entre el hotend E4 y M4?**](#A1)
- [**¿Qué tipo de hotend debo elegir?**](#A2)
- [**¿Cómo cargar filamentos en el hotend correctamente?**](#A3)
- [**¿Cuál es la diferencia en la configuración de corte entre los hotends M4 y E4**](#A4)
- [**¿Cómo cambiar entre el hotend M4 y E4?**](#A5)


-----
## <a id="A1">¿Qué diferencia hay entre el hotend E4 y M4?</a>
![](./M4V6vsE4.jpg)   
- **M4 hotend** puede mezclar filamentos de diferentes colores para producir filamentos de nuevos colores. **El hotend E4** no tiene esta capacidad.
- **E4 hotend** es bueno para imprimir objetos 3D de un color o de varios colores (hasta 4 colores).
- **M4 hotend** es bueno para imprimir objetos 3D de color degradado, también puede imprimir objetos 3D de más de 4 colores (mezclando los filamentos).
### Principio de funcionamiento del hotend E4
![](./E4/User_guide/E4_principle.gif)
### Principio de funcionamiento del hotend M4
[](https://github.com/ZONESTAR3D/Document-and-User-Guide/assets/29502731/2b9f4d75-b6fd-486f-aaa7-7a1163383316)

### Ventajas del hotend E4
1. "Torre principal del interruptor del extrusor" más pequeña mientras se imprimen objetos 3D multicolores.
2. Mejor calidad al imprimir objetos 3D de un color.
3. Soporte para imprimir diferentes tipos de filamento en el mismo objeto 3D.
### Ventajas del hotend M4
1. Admite mezclar filamentos de diferentes colores con nuevos colores.
2. Admite impresión en color degradado.
3. Admite un mayor caudal.
![](M4VSE4.jpg)

-----
## <a id="A2"> ¿Qué hotend debo elegir, M4 o E4?</a>
- Si **no necesita** imprimir un modelo 3D de color degradado, le sugerimos que elija **E4 hotend**, puede obtener una mejor calidad en la impresión de impresiones 3D de un solo color y de varios colores.
- Si desea imprimir un modelo 3D de **color degradado**, o desea **mezclar filamentos de diferentes colores con otro color**, elija el hotend M4.

-----
## <a id="A3">Cómo cargar/descargar filamentos correctamente</a>
El extremo caliente M4 y el extremo caliente E4 tienen diferentes requisitos para cargar filamento.
- **Requisitos de cantidad para carga de filamentos:**
   - El hot end M4 requiere cargar cuatro filamentos al mismo tiempo, independientemente de si imprime en un solo color o en varios colores;
   - El hot end E4 puede elegir el número de filamentos a cargar según los colores impresos.
- **Requisitos de posición para carga de filamentos:**
   - El hot end M4 requiere que el filamento se instale en la parte inferior del hot end;
   - El hot end E4 requiere que el filamento se instale encima de la boca del embudo del hot end (extendiendo el tubo de PTFE unos 20 mm).
### Para hotend M4
#### Pasos para cargar filamentos en el hotend M4:
##### [![](https://img.youtube.com/vi/-47yB95uIxI/0.jpg)](https://www.youtube.com/watch?v=-47yB95uIxI)
Al cargar los filamentos en el hotend M4, independientemente de cuántos extrusores necesite usar durante la impresión, ***los cuatro filamentos deben cargarse en el hotend***, y es importante ***asegurarse de que todos los filamentos estén cargado en la parte inferior del hotend*** antes de comenzar a imprimir.     
:warning: ***Ya sea que imprima en un solo color o en varios colores, debe cargar los cuatro filamentos en el hotend M4V6.***
1. Corta la parte frontal del filamento con unos alicates diagonales antes de cargarlo en el extrusor y el hotend.
2. Cargue 4 filamentos en todos los extrusores uno por uno y luego gire el engranaje de los extrusores hasta que el filamento entre en el tubo interior de PTFE del hotend, gire más de 4 a 5 vueltas y luego deténgase.

#### Pasos para descargar el filamento del hotend M4:
1. Calentar la boquilla (200 ℃ para PLA / 230 ℃ para PETG/ABS) y esperar a que alcance la temperatura ***Menu: Prepare>>Filament>>Preheat: 200/230***.
2. Alimente los filamentos al menos 10 mm en los 4 canales simultáneamente ***Menu: Prepare>>Filament>>Extruder: All; Prepare>>Filament>>Slowly Load***.
3. Descargue los filamentos del hotend ***Menu: Prepare>>Filament>>Slowly unload***.
  
### Para hotend E4
#### <a id = "PRELOAD_FILAMENT">Pasos para cargar filamentos en el hotend E4:</a>
##### [![](https://img.youtube.com/vi/FyHrAMytlT8/0.jpg)](https://www.youtube.com/watch?v=FyHrAMytlT8)
Si comprende el principio de funcionamiento del hotend E4, ya debería saber que al imprimir en varios colores, la máquina primero debe descargar el filamento previamente cargado del hotend y luego cargar el siguiente filamento. Sin embargo, normalmente ***la máquina no tiene la capacidad de reconocer la distancia entre el extremo frontal del filamento y la boquilla antes de comenzar a imprimir***. Por lo tanto, necesitamos configurar un proceso llamado <u>***"filamentos de precarga"***</u>, cuyo objetivo es permitir que la máquina mueva los hilos finos a una posición adecuada conocida por la máquina antes. imprimiendo el objeto.
:warning: ***Solo los filamentos del extrusor que deben usarse en el archivo gcode deben cargarse en el hotend E4.***

### Pasos para descargar filamento del hotend E4:
1. Calentar la boquilla (200 ℃ para PLA / 230 ℃ para PETG/ABS). ***Menú: Preparar>>Filamento>>Precalentar: 200/230***
2. Alimente el filamento al menos 10 mm en el extrusor usado. ***Menú: Preparar>>Filamento>>Extruidor: 1/2/3/4; Preparar>>Filamento>>Cargar lentamente***
3. Descargue el filamento del fusor. ***Menú: Preparar>>Filamento>>Descargar lentamente***

-----
## <a id = "A4">¿Cuál es la diferencia en la configuración de corte entre el hotend M4 y E4?</a>
:pushpin: Estas configuraciones se han establecido en los perfiles del software PrusaSlicer que proporcionamos. Solo necesita elegir el **preajuste de impresora** correcto según su máquina y tipo de hotend.
### Configuración de corte para impresión multicolor
Para imprimir en varios colores, las configuraciones de corte para el hotend E4 y el hotend M4 difieren principalmente de la siguiente manera:
- **iniciar gcode**
   - **Para el hotend E4**, requiere "filamentos precargados" antes de comenzar a imprimir ([**Know Why**](#PRELOAD_FILAMENT)), para más detalles, consulte [**start gcode of the E4 hotend**][E4_STARTGCODE].
   - **Para el hotend M4**, al imprimir no más de 4 colores, no es necesario realizar cambios especiales en el gcode de inicio. Pero **si necesita imprimir más de 4 colores** (mezclando filamentos de diferentes colores en varios colores), puede configurar la proporción de mezcla de colores en el código de inicio. Para obtener más información, consulte [**Cómo imprimir más de 4 colores utilizando el extremo caliente M4**][M4_MIXMULTICOLORPRINT].
- **Configuración de retracción de los extrusores**
   - **Para el hotend E4**, la **Longitud de retracción** recomendada es de 6 ~ 8 mm (debe ser inferior a 10 mm).
   - **Para el hotend M4**, la **Longitud de retracción** recomendada es de 8 ~ 15 mm.
- **Torre de limpieza (Torre principal)**
:pushpin: El software de corte que admite múltiples impresoras extrusoras tiene una opción **"Wipe Tower(Prime Tower)"**. Porque cuando la impresora cambia de un extrusor a otro, a menudo necesita limpiar primero los hilos finos del color anterior en el extremo caliente. Después de activar la opción de borrado de la torre, el software de corte puede generar una impresión "adicional" en el archivo gcode para limpiar los filamentos restantes en el extremo caliente.
   - **Para el hotend E4**, el volumen requerido de la torre de cables es relativamente pequeño.
   - **Para el hotend M4**, el volumen requerido de la torre de cables es relativamente grande.
- **Código G de cambio de herramienta**
   - **Para el hotend E4**, al cambiar el extrusor, es necesario sacar el filamento del color anterior del hotend y luego cargar el filamento del siguiente color en el hotend. Por lo tanto, es necesario configurar Tool Change Gcode para lograr esta operación. Para obtener más información, consulte [**Código G de cambio de herramienta para hotend E4**][E4_TOOLCHANGE].
   - **Para el hotend M4**, no necesita **Código G de cambio de herramienta**.

-----
## <a id="A5">Cómo cambiar entre hotend M4 y hotend E4</a>
### 1. Afloje los tres tornillos de la carcasa del hotend y retire el hotend viejo de la máquina (x polea). Luego instale el nuevo hotend en la máquina (polea x) y bloquee los tornillos.
![](./E4/User_guide/E4-4.jpg)
### 2. Conecte los cables del nuevo hotend a la máquina.
![](./E4/User_guide/wiring1.jpg) ![](./E4/User_guide/wiring2.jpg)
### 3. Configure el tipo de hotend en el menú LCD: *Control>>Configurar>>Tipo de hotend*
![](./E4/User_guide/hotendtype-mix.jpg)![](./E4/User_guide/hotendtype-nonmix.jpg)
#### :pushpin: Los conectores del cabezal de impresión Z9V5 están ocultos dentro de la máquina, es necesario quitar el anillo de goma y sacar los conectores.
![](./Z9V5HotendWire.jpg)
### :warning: NOTA 1: Si no puede encontrar el menú "tipo de hotend" en la pantalla LCD, cargue el firmware más reciente en su impresora.
[**:point_right: Firmware para Z9V5**][FW_Z9V5] / [**:point_right: Firmware para Z8P**][FW_Z8P] / [**:point_right: Firmware para Z9M4**][FW_Z9M4]
### :warning: NOTA 2: El hotend de colores mezclados y el hotend de colores no mezclados deben usar configuraciones de corte diferentes; preste atención para distinguirlos. Usar una configuración de corte incorrecta puede bloquear el hotend.

-----
