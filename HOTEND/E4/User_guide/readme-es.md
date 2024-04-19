[PRUSA]: https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer#6-slicing-muti-color-for-e4-hotend
[CURA]: https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/cura
[S3D]: https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/Simplify3D#slicing-video-toturial-for-z9v5-with-e4-hotend
[ENDGCODE]: https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/Custom_Gcode.md#end-g-code
[STARTGCODE]: https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/Custom_Gcode.md#start-gcode
[FIRMWARE]: https://github.com/ZONESTAR3D/Firmware

----
## <a id="choose-language">:globe_with_meridians: Choose language </a>
[![](../../../lanpic/EN.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/User_guide/readme.md)
[![](../../../lanpic/ES.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/User_guide/readme-es.md)
[![](../../../lanpic/PT.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/User_guide/readme-pt.md)
[![](../../../lanpic/FR.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/User_guide/readme-fr.md)
[![](../../../lanpic/DE.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/User_guide/readme-de.md)
[![](../../../lanpic/IT.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/User_guide/readme-it.md)
[![](../../../lanpic/RU.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/User_guide/readme-ru.md)
[![](../../../lanpic/JP.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/User_guide/readme-jp.md)
[![](../../../lanpic/KR.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/User_guide/readme-kr.md)
<!-- [![](../../../lanpic/SA.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/User_guide/readme-ar.md) -->

----
## Manual de usuario del hotend E4
ZONESTAR 4-IN-1-OUT **No mezclar colores** hot end (conocido como **E4 Hot end**) tiene 4 canales de entrada y 1 boquilla, al cambiar de color, es necesario descargar el filamento del color anterior ( sacado) del extremo caliente y luego cargue el siguiente filamento de color.

### <a id="A1"> 1. Especificaciones </a>
| Artículo | Parámetros | Artículo | Parámetros |
|:--------------------------:|:-------------------------:|:--------------------------:|:--------------------------:|
| Tensión nominal | CC 24 V/60 W máx. | Diámetro de la boquilla | Predeterminado 0,4 mm<sup>1</sup> |
| Canal de entrada | 4 | Modelo de boquilla | E3D V6 |
| Número de boquillas | 1 | Diámetro del filamento | 1,75 mm |
| Calentador | 24V/60W ⌀6x25mm | Sensor de temperatura | Termistor NTC 100K B3950 |
| Ventilador de refrigeración | 4010/5000 RPM/24 V 0,15 A | Ventilador extrusor | 4010/5000 RPM/24 V 0,15 A |
| Filamentos de soporte | PLA/PLA+/PETG/ABS/ASA etc. | Temperatura de trabajo | 260 ℃ máximo |
| Longitud del cable | 1 metro | Dimensiones exteriores | 50x60x75mm |
| Peso neto | 220 g | Peso bruto | 350g |

### <a id="A2"> 2. Componentes </a>
El conjunto del hot end E4 incluye las siguientes piezas/accesorios:
![](./E4-2.jpg)
>
     1. Ventilador de refrigeración 2. Carcasa 3. Orificio de instalación del sensor de nivelación de la cama 4. Tornillos montados
     5. Ventilador extrusor 6. Impresiones de "pato" del ventilador 7. Bloque calefactor 8. Disipador de calor
     9. Boquilla 10. Calentador de cartucho 11. Sensor de temperatura 12. Garganta
     13. Funda de silicona 14. Accesorios (conectores neumáticos) 15. Cable

### <a id="A3"> 3. Cable </a>
![](./E4-3.jpg)

### <a id="A4"> 4. Instalación y cableado </a>
La posición de montaje del hot end E4 se ajusta al "estándar de montaje del hot end ZONESTAR", que se puede instalar en casi todas las impresoras 3D ZONESTAR, incluidas las series de productos P802, M8, D805S, Z8, Z9, Z10, etc.
#### 4.1 Instalación
Simplemente retire los 3 tornillos detrás del conjunto del hotend e instale el conjunto del hotend E4 en el soporte X de la máquina.
![](./E4-4.jpg)
#### 4.2 Cableado
##### :loudspeaker: **Atención**
- **Por favor tenga cuidado para distinguir los terminales 3 y 4**, porque el color de sus terminales es el mismo, pero el color de los cables es diferente.
Si los cables de 3 y 4 están conectados al revés, podrá ver que la temperatura de la boquilla que se muestra en la pantalla LCD será mucho más alta que la temperatura ambiente después de encender la máquina.
- Al enchufar el terminal, **tenga cuidado de no empujar el terminal metálico fuera de la caja de plástico**.
##### :loudspeaker: **Tenga en cuenta**
- **El ventilador de refrigeración debe estar encendido** (cuando la temperatura del hot end es superior a 60 °C), de lo contrario el hot end podría bloquearse o incluso dañarse.
  - De forma predeterminada, el **voltaje de trabajo** del ventilador y el calentador en el extremo caliente es **DC 24V**.
#### Siga la definición de terminales para conectar el hotend a su tablero de control.
- **Sin cable de extensión**
![](./cableado1.jpg)
- **Con cable extendido**
![](./cableado2.jpg)
#### 4.3 Establecer el tipo de hotend en el MENÚ LCD: Control>>Configurar>>Tipo de hotend: sin mezcla
- :warning: Si su impresora no tiene una pantalla TFT-LCD de 4,3", ignore este paso.
- :warning: Si no puede ver el menú en la pantalla LCD de su impresora, actualice a la versión más reciente. [:link: **Enlace de descarga de firmware**][FIRMWARE]
##### ![](./hotendtype-nonmix.jpg)

### <a id="A5"> 5. Principio de funcionamiento </a>
El extremo caliente E4 (4-EN-1-SALIDA sin mezcla de colores) está compuesto por un disipador de calor, un colector de embudo, un bloque calefactor, una boquilla, etc. Durante la impresión, solo se permite cargar un filamento en el extremo caliente. Mientras cambia a otro filamento de color, el extrusor extrae el filamento de color anterior del extremo caliente E4 y luego carga otro filamento en el extremo caliente E4. La siguiente imagen (de izquierda a derecha) demuestra brevemente este proceso.
##### ![](./E4-5.jpg)
#### También puede consultar una animación para comprender bien el principio de funcionamiento del hot end E4.
![](./E4_principle.gif).
##### :book: Acerca de "Torre de limpieza"
Debido a que todavía quedan filamentos derretidos del color anterior en la boquilla después de cargar un filamento de nuevo color, debemos "limpiar" la boquilla antes de comenzar a imprimir el filamento de nuevo color. De lo contrario, la parte inicial impresa será del color anterior pero no del nuevo color como esperábamos. La solución es agregar **"torre de limpieza"** después de cambiar a una nueva extrusora en el software de corte.
Para obtener más información, consulte [**:point_right: Slicing**](#A9).
:bulb: la torre de limpieza se llama "torre Prime" en Cura Slicer y "Prime Pillar" en Simplify3d Slicer.

### <a id="A6"> 6. Dimensiones </a>
![](./E4_size.jpg)

### <a id="A7"> 7. Precarga los filamentos </a>
#### 7.1 Para impresión a un color
[![](https://img.youtube.com/vi/6aTF5QnFhi4/0.jpg)](https://www.youtube.com/watch?v=6aTF5QnFhi4)
#### 7.2 Para impresión multicolor
[![](https://img.youtube.com/vi/FyHrAMytlT8/0.jpg)](https://www.youtube.com/watch?v=FyHrAMytlT8)    
Antes de imprimir, cargue previamente los filamentos en la posición adecuada del extremo caliente para que el extrusor pueda cargar suavemente los filamentos dentro y fuera del extremo caliente.
- **Paso 1:** Cargue los filamentos del extrusor y deje que se extiendan unos 10 mm fuera de los tubos de PTFE.
- **Paso 2:** Conecta los tubos de PTFE (con filamentos) al HOTEND.
     - :pushpin: **Si hay un filamento en el extremo caliente, caliéntalo y sácalo primero. Consulte [Descargar filamentos](#A8) para hacerlo.**
     - :pushpin: Cortar la parte frontal de los filamentos en una forma afilada antes de cargar el filamento.
     - :pushpin: Si no se utilizó el extrusor durante la impresión, no es necesario cargar el filamento en el extremo caliente.
     ![](./E4-6.jpg)
     - :pushpin: agregue algunos gcodes en **"Iniciar gcode"** ([:point_right: View][STARTGCODE]) del software de corte para imprimir.
     ![](./Preload_line.jpg)
     - :pushpin: agregue algunos gcodes en **"End gcode"** ([:point_right: View][ENDGCODE]) del software de corte para extraer el último filamento impreso del hotend.

### <a id="A8"> 8. Descargar filamentos </a>
Siga los pasos a continuación para descargar el filamento del hotend:
- **Paso 1:** Calentar la boquilla (190 grados para PLA y 230 grados para ABS).
- **Paso 2:** Gire el engranaje del extrusor para descargar el filamento.
:star2: Algunas impresoras 3D (por ejemplo, Z9V5Pro) tienen un menú "Filamento" en la pantalla LCD, opere la pantalla LCD y use el menú ***"Preparar>>Filamento"*** para precalentar la boquilla, elija la extrusora y descargue filamentos.

### <a id="A9"> 9. Cortar </a>
Guía del usuario (vídeo tutorial) para el software de corte PrusaSlicer/Cura/Simplify3d.
- **:+1: PrusaSlicer**, consulte :point_right: [**aquí**][PRUSA].
- **Cura slicer**, consulte :point_right: [**aquí**][CURA].
- **Simplify3d Slicer**, consulte :point_right: [**aquí**][S3D].

### <a id="A10"> 10. Probando gcode </a>
Hemos subido algunos archivos de prueba a nuestra página de Github, puede descargarlos desde [**aquí**](../example/readme.md).

### <a id="A11"> 11. Solución de problemas </a>
Si tiene problemas al utilizar el hot-end E4, consulte primero la [**guía de solución de problemas**](../FAQ/readme.md) para encontrar una solución. Si el problema aún no se puede resolver, comuníquese con nuestro ingeniero de soporte técnico por correo electrónico: correo electrónico: support@zonestar3d.com.

----
### Vender enlace
[:gift: **ZONESTAR Offical Store**](https://bit.ly/39qDtKp)     
[:gift: **Aliexpress**](https://www.aliexpress.com/item/1005002951777699.html)

----

