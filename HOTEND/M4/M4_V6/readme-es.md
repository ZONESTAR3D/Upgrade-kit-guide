[M4V6_CAUTION]: https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/M4/M4_V6/M4V6_Precaution.md
[MIXING_COLOE]: https://github.com/ZONESTAR3D/Document-and-User-Guide/tree/master/Mixing_Color
[SLICING_0]: https://github.com/ZONESTAR3D/Slicing-Guide
[SLICING_1]: https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer
[SLICING_2]: https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer#4-slicing-one-color
[SLICING_M4]: https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/PrusaSlicerGuide_M4.md
[FAQ_M4E4]: https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/FAQ_M4E4.md

----
## <a id="choose-language">:globe_with_meridians: Choose language </a>
[![](./lanpic/EN.png)](./readme.md)
[![](./lanpic/ES.png)](./readme-es.md)
[![](./lanpic/PT.png)](./readme-pt.md)
[![](./lanpic/FR.png)](./readme-fr.md)
[![](./lanpic/DE.png)](./readme-de.md)
[![](./lanpic/IT.png)](./readme-it.md)
[![](./lanpic/JP.png)](./readme-jp.md)
[![](./lanpic/KR.png)](./readme-kr.md)
[![](./lanpic/RU.png)](./readme-ru.md)
<!-- [![](./lanpic/SA.png)](./readme-ar.md) -->

----
## :book: Guía del usuario del hotend M4V6
El extremo caliente de color mixto ZONESTAR 4-IN-1-OUT tiene 4 canales de entrada y 1 boquilla, cuatro filamentos se mezclan en el extremo caliente y luego se extruyen a través de una boquilla, por lo que no solo permite a la impresora imprimir el color original de los filamentos, sino también También permite imprimir más colores ajustando la proporción de mezcla de filamentos.

### Contenido
- **[Atención](#A0)**
- **[Principio de funcionamiento](#A1)**
- **[Especificaciones](#A2)**
- **[Componentes de M4V6](#A3)**
- **[Cableado](#A4)**
- **[Estructura](#A5)**
- **[Dimensiones](#A6)**
- **[Instalación y cableado](#A7)**
- **[Cargar/descargar filamentos](#A8)**
- **[Pasos para imprimir usando el hotend M4V6](#A9)**
- **[Guía de corte](#A10)**
- **[Solución de problemas](#A11)**
- **[Apéndice](#A12)**

## <a id="A0">:warning: ATENCIÓN POR FAVOR</a>
### :loudspeaker: Antes de usar el hot end M4V6, lea atentamente [:book:Precauciones para usar M4V6][M4V6_CAUTION].
### :loudspeaker: Debe cargar 4 filamentos en el hotend M4V6 simultáneamente, el funcionamiento incorrecto puede bloquear el hotend de mezcla de colores. Si el bloqueo del extremo caliente es causado por una operación incorrecta, no está cubierto por la garantía.
### :loudspeaker: NO extraiga los "tubos internos de PTFE" del hotend M4V6.
### :loudspeaker: Una vez que los filamentos ya hayan ingresado al hotend M4V6, NO use el menú "Carga rápida" para cargar los filamentos.

### <a id="A1">Principio de funcionamiento</a>
**:warning: antes de usar el M4V6, lea el [:book: Introducción al extrusor mezclador de colores][MIXING_COLOE] para comprender los principios de funcionamiento del extrusor mezclador de colores.**
###### 
[](https://github.com/ZONESTAR3D/Document-and-User-Guide/assets/29502731/2b9f4d75-b6fd-486f-aaa7-7a1163383316)

### <a id="A2">Especificaciones</a>
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

### <a id="A3">Componentes</a>
![](./2.jpg) ![](./1.jpg)

### <a id="A4">Terminal de cableado</a>
![](./wire.jpg)
:pushpin: extender el cable es opcional.

### <a id="A5">Estructura</a>
![](./3.jpg)

### <a id="A6">Dimensiones</a>
![](./size.jpg)

### <a id="A7">Instalación y cableado</a>
La posición de montaje del hot end M4 se ajusta al "estándar de montaje del hot end ZONESTAR", que se puede instalar en casi todas las impresoras 3D ZONESTAR, incluidas las series de productos P802, M8, D805S, Z8, Z9, Z10, etc.
#### Instalación
Simplemente retire los 3 tornillos detrás del conjunto del hotend e instale el conjunto del hotend M4 en el soporte X de la máquina.
![](./M4_installation.jpg)
#### Alambrado
##### :loudspeaker: ATENCIÓN
- **Por favor tenga cuidado para distinguir los terminales 3 y 4**, porque el color de sus terminales es el mismo, pero el color de los cables es diferente.
Si los cables de 3 y 4 están conectados al revés, podrá ver que la temperatura de la boquilla que se muestra en la pantalla LCD será mucho más alta que la temperatura ambiente después de encender la máquina.
- Al enchufar el terminal, **tenga cuidado de no empujar el terminal metálico fuera de la caja de plástico**.
#### :loudspeaker: **Tenga en cuenta**
- **El ventilador de refrigeración debe estar encendido** (cuando la temperatura del hot end es superior a 60 °C), de lo contrario el hot end podría bloquearse o incluso dañarse.
  - De forma predeterminada, el **voltaje de trabajo** del ventilador y el calentador en el extremo caliente es **DC 24V**.
#### Siga la definición de terminales para conectar el hotend a su tablero de control.
- **Sin cable de extensión**
![](./wiring1.jpg)
- **Con cable extendido**
![](./wiring2.jpg)
#### Configure el tipo de hotend en el MENÚ LCD: Control>>Configurar>>Tipo de hotend: Mezcla
![](./hotendtype-mix.jpg)  

### <a id="A8">Cargar/Descargar filamentos</a>
#### :warning: ¡ATENCIÓN POR FAVOR! Necesita cargar 4 filamentos en el extremo caliente incluso si imprime un modelo 3D en color, NO deje ningún canal vacío antes de imprimir.
#### :warning: ¡ATENCIÓN POR FAVOR! El menú "Carga rápida" solo se puede usar cuando se carga el filamento desde la extrusora al extremo caliente; una vez que el filamento ingresó al extremo caliente, use el menú "Carga lenta" pero no "Carga rápida".
- **Cargar filamento en el hotend:**     
###### [![](https://img.youtube.com/vi/-47yB95uIxI/0.jpg)](https://www.youtube.com/watch?v=-47yB95uIxI)
   - Corta la parte frontal del filamento con unos alicates diagonales antes de cargarlo en el extrusor y en el extremo caliente.
   - Cargue 4 filamentos en todos los extrusores uno por uno.
   - Gire el engranaje de los extrusores para cargar los filamentos uno por uno, no gire cada extrusor más de 2 vueltas a la vez, hasta que todos los filamentos entren al tubo interno de PTFE del extremo caliente, extruya más de 4 a 5 vueltas para cada extrusor y luego se detiene.    
   :warning: No alimente filamentos al hotend cuando algún canal del hotend esté vacío.     
   :warning: Asegúrese de que los filamentos de cada canal lleguen al fondo del extremo caliente antes de alimentar el filamento.    
- **Descargar filamento del hotend:**
   - Calentar la boquilla (200℃ para PLA / 230℃ para PETG/ABS).
   - Alimente simultáneamente el filamento al menos 10 mm en los 4 canales.
   - Opere en el menú LCD o gire el engranaje del extrusor para descargar los filamentos.

### <a id="A9">Pasos para imprimir usando el hotend M4V6</a>
#### Imprime un modelo 3D de un color
- **Preparar archivo gcode**. Para cortar el modelo 3D utilizando la configuración de una impresora 3D de un color, consulte [**aquí**][SLICING_2].
- **Cargar filamentos**. Cargue **los 4 filamentos** en los extrusores y luego introduzca los filamentos en la parte inferior del extremo caliente M4V6.
- **Imprimir desde tarjeta SD**. Mueva el elemento al elemento **Imprimir** en la pantalla LCD y haga clic en la perilla y elija el archivo gcode, haga clic en la perilla para comenzar a imprimir.
- **Ajuste la altura de la boquilla**. Espere a que se calienten la boquilla y la cama caliente, y cuando la impresora comience a imprimir la primera capa, haga doble clic en la perilla de la pantalla LCD para ajustar la distancia entre la boquilla y la cama, y luego espere a que termine.
#### Imprimir modelo 3D multicolor
- **Preparar archivo gcode**. Para cortar el modelo 3D utilizando la configuración de la impresora 3D multicolor M4, consulte [**aquí**][SLICING_M4].
- **Cargar filamentos**. Cargue **los 4 filamentos** en los extrusores y luego introduzca los filamentos en la parte inferior del extremo caliente M4V6.
- **Imprimir desde tarjeta SD**. Mueva el elemento al elemento **Imprimir** en la pantalla LCD y haga clic en la perilla y elija el archivo gcode, haga clic en la perilla para comenzar a imprimir.
- **Ajuste la altura de la boquilla**. Espere a que se calienten la boquilla y la cama caliente, y cuando la impresora comience a imprimir la primera capa, haga doble clic en la perilla de la pantalla LCD para ajustar la distancia entre la boquilla y la cama, y luego espere a que termine.

### <a id="A10">Rebanar</a>
Recomendamos utilizar PrusaSlicer para cortar. Para tutoriales de instalación y uso, consulte el siguiente enlace:
- **[Instalar software Prusaslicer][SLICING_1]**
- **[Guía de corte para hotend M4][SLICING_M4]**
Para obtener más tutoriales sobre el uso de otro software de corte, consulte [:book:esta guía][SLICING_0].

### <a id="A11">Solución de problemas</a>
Si hay algún problema al usar el hot-end M4V6, consulte [**:book: este manual de solución de problemas**](./M4V6_FAQ/readme.md) para encontrar una solución primero.

### <a id="A12">:paperclip: Apéndice</a>
#### :book: Apéndice I: [Logre una impresión rápida utilizando el extremo caliente M4V6](./HighFlow/readme.md)
Al imprimir un modelo 3D de un solo color, M4V6 puede admitir caudales más altos. Para obtener más detalles, consulte [:book: esta guía](./HighFlow/readme.md).

#### :book: Apéndice II: [Cómo cambiar entre hotend E4 y hotend M4][FAQ_M4E4]
