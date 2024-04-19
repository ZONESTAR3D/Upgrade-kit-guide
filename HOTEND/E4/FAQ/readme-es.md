[E4FAQ1]:https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/E4/User_guide/readme.md#5-working-principle
[E4FAQ2]:https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/Custom_Gcode.md
[E4FAQ3]:https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/PrusaSlicerGuide_E4.md#step-6-set-the-print-settings
[E4FAQ4]:https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/Custom_Gcode.md#tool-change-g-code
[E4FAQ5]:https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/cura/E4_hotend/readme.md#exturder-startend-gcode-of-e4-hotend
[E4FAQ6]:https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/E4/User_guide/readme.md#2-components
[BMG]: https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/Dual_Gear_Extruder#manual-for-upgraded-dual-gear-extruder

----
## <a id="choose-language">:globe_with_meridians: Choose language </a>
[![](../../../lanpic/EN.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/FAQ/readme.md)
[![](../../../lanpic/ES.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/FAQ/readme-es.md)
[![](../../../lanpic/PT.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/FAQ/readme-pt.md)
[![](../../../lanpic/FR.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/FAQ/readme-fr.md)
[![](../../../lanpic/DE.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/FAQ/readme-de.md)
[![](../../../lanpic/IT.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/FAQ/readme-it.md)
[![](../../../lanpic/RU.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/FAQ/readme-ru.md)
[![](../../../lanpic/JP.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/FAQ/readme-jp.md)
[![](../../../lanpic/KR.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/FAQ/readme-kr.md)
<!-- [![](../../../lanpic/SA.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/FAQ/readme-ar.md) -->

-----
## Solución de problemas del hotend E4
Después de realizar más de 1000 pruebas de impresión, resumimos los posibles problemas en el hotend E4, especialmente las causas de la obstrucción (bloqueo) de los filamentos y sus soluciones para su referencia.
- Si no conoce el principio de funcionamiento del hotend E4 (4-IN-1-OUT sin mezcla de colores), le sugerimos que lea este documento ([**:point_down:Principio de funcionamiento del hotend E4**](#F0 )) primero.
- La razón por la que el hot end E4 no se puede utilizar para imprimir puede no provenir del propio hot end. Por lo tanto, antes de emitir un juicio, es mejor consultar [**:point_down:Probar si el hotend puede funcionar normalmente**](#F1) para simplemente probar si el hotend E4 puede funcionar normalmente.
- Si su hotend E4 básicamente puede completar la impresión, pero hay defectos en la parte impresa, consulte [**:point_down:Problema de defecto de impresión**](#F2).
- Si su hotend E4 a menudo tiene un bloqueo grave, consulte [**:point_down:problema de obstrucción grave**](#F3).

-----
### <a id="F0"></a> Algunas cosas que debes saber sobre el hotend E4
#### :one: [Principio de funcionamiento del hotend E4][E4FAQ1]
Si no tiene claro el principio de funcionamiento de E4, haga clic en [**aquí**][E4FAQ1] para verlo. Comprender cómo funciona E4 le ayudará a comprender el problema y la razón que lo causó.
#### :two: Resumen de la estructura del hotend E4
Para explorar mejor los siguientes documentos, lea esta sección para conocer los nombres y funciones de cada parte del hotend E4.
Hay dos versiones del hotend E4 que vendemos (E4_V2 y E4_V3), no hay mucha diferencia en uso y calidad de impresión.
**Lo que mejoró E4_V3:**
- Modifique la estructura del embudo para ayudar a que el filamento entre suavemente en la boquilla.
- Añadir un tubo de cobre para mejorar la disipación del calor de la garganta (parte rompe-calor).
![](./E4_struct.png)
:warning: Si necesita reemplazar las piezas/accesorios del hotend E4, distinga la versión que tiene.
#### Descripción de las piezas:
>
     1. Accesorio (articulación traqueal PC4) 2. Disipador de calor 3. Colector de embudo (E4V2) 4. Disipador de calor (garganta)
     5. Tubo interior de PTFE (E4V2) 6. Bloque calefactor 7. Boquilla 8. Tubo de cobre (E4V3) 9. Colector de embudo (E4V3)
:pushpin: Hemos actualizado el tamaño del bloque de aluminio calefactor y el nuevo bloque de aluminio calefactor es simétrico a izquierda y derecha, por lo que no bloqueará la salida de aire del ventilador del extrusor. Además, se han agregado tornillos para fijar el termistor.
:pushpin: Lanzamos un kit de calentamiento V3H, es adecuado para imprimir filamentos de alta temperatura como PC, PET, PA, etc.
![](./CalefacciónBlock.jpg)

#### :three: Elija el filamento apropiado <a id="choosefilament"></a>
El hotend E4 se puede aplicar a una amplia gama de filamentos como ABS, PLA, PLA+, PETG, etc. Pero como sabes, al cambiar de extrusora, se descargará un filamento del hotend y luego se volverá a cargar otro filamento. Por lo tanto, las siguientes características del filamento pueden no ser buenas para el hotend E4:
1. **Se expande demasiado después de calentarlo**: no puede ingresar al hotend cuando se recarga.
2. **Demasiado blando**: es fácil que el engranaje del extrusor lo raye durante múltiples cargas/descargas.
3. **Con cuerdas largas después de descargar**: bloquee el filamento para ingresar al hotend.    

Para mejorar la tenacidad, fluidez y apariencia del filamento, los fabricantes de filamentos agregarán algunos aditivos al filamento, lo que puede causar que el filamento tenga estas características "inaccesibles" para el hotend E4, por lo que le sugerimos que siga los pasos a continuación para verificar antes de usar un filamento nuevo: **Calentar la boquilla >> cargue manualmente el filamento en el hotend >> purgue un poco de filamento (50 mm aproximadamente) >> sáquelo del hotend lentamente >> verifique el tamaño y la longitud de las cuerdas en el Fin del filamento.**

-----
### <a id="F1"></a> Pruebe si el hot end puede funcionar normalmente
![](https://github.com/ZONESTAR3D/Upgrade-kit-guide/assets/29502731/621f4c4c-c821-4602-b997-dc060fadedc2)
#### 1. Caliente el extremo caliente (boquilla) a 200 ℃.
#### 2. Cargue los filamentos en cada canal del extremo caliente uno por uno y observe si el filamento puede salir de la boquilla.
:warning: **Tenga en cuenta:**
- **Corta el extremo frontal antes de cargar el filamento**
- **Empuje lentamente (<2mm/s) el filamento cuando llegue a la boquilla.**
- **Utilice una velocidad más rápida (>10 mm/s) al sacar los filamentos.**

-----
### <a id="F2"></a> La impresión se puede completar normalmente, pero hay defectos en los objetos impresos.
También puede encontrar este problema: en general, la impresión se puede realizar normalmente, pero hay defectos obvios al imprimir en ciertas capas y ocasionalmente se escucha el ruido anormal de Kaká del extrusor durante la impresión.
##### :pill: Solución <a id="A7"></a>
Este problema generalmente se debe a que no se carga ni descarga el filamento al cambiar de extrusora. Siga los pasos a continuación para verificarlo:
- [:point_up: **Compruebe la presión del extrusor**](#HOW1)
- **Revise o reemplace el filamento**[:point_up: 1](#Q5) [:point_up: 2](#Q6) [:point_up: 3](#choosefilament).
- [**Agregue longitud de tirar y empujar modificando la configuración de corte**](#A5).
- [**Reinstalar la parte térmica del hotend**](#HOW2)
- **Revise las guías de PTFE que conectan al extrusor y al hotend.** Después de un período de uso, el tubo de PTFE puede deformarse (especialmente la parte que conecta los accesorios), lo que aumenta en gran medida la resistencia del filamento a moverse dentro del PTFE. tubos.
- **:+1: Actualización a extrusoras de doble engranaje.** La extrusora de doble engranaje puede aumentar en gran medida la fuerza de empujar y tirar del cable fino, reduciendo la posibilidad de bloqueo causado por no retirar suavemente el cable fino del extremo caliente.
- [**Reemplazar un hotend nuevo.**](https://bit.ly/39qDtKp)

-----
### <a id="F3"></a> El hotend E4 a menudo está gravemente bloqueado y no puede imprimir por completo
Si encuentra un problema grave de bloqueo en el hotend, como que el filamento no se puede sacar del hotend, o el filamento está retorcido y deformado en el embudo colector del hotend, siga los siguientes pasos para verificarlo:
:warning:**NOTA :warning: Si su máquina está equipada con sensores de agotamiento de filamento, se recomienda omitirlos primero y dejar que los filamentos se carguen directamente en las extrusoras; consulte [:point_right: aquí](./E4FAQ-4.jpg)**.

#### :one: ¿Funciona bien el ventilador de refrigeración del hotend? <a id="Q1"></a>
El **[VENTILADOR de refrigeración del hotend E4][E4FAQ6]** debería funcionar (puede funcionar todo el tiempo o funcionar cuando la temperatura de la boquilla es superior a 60 °C). Si el VENTILADOR de refrigeración no funciona, es fácil que el hotend se bloquee.

#### :two: ¿Está la boquilla demasiado cerca de la plancha de impresión? <a id="Q2"></a>
Si la boquilla está demasiado cerca de la placa de impresión (cama caliente), el filamento no se puede extruir de la boquilla al imprimir, puede causar que se bloquee el hotend, en casos severos, puede causar que el filamento se retuerza en el embudo. Colector de hotend. Este problema suele ocurrir al imprimir la primera capa.
##### :pill: Solución <a id="A2"></a>
- Al imprimir la primera capa, utilice el menú **babysteps** para ajustar la distancia desde la boquilla hasta la plancha de impresión.
- Al cortar, preste atención a ajustar la altura de la primera capa (150% del espesor de la capa o 80% del diámetro de la boquilla).

#### :three: ¿Puede el extrusor empujar y tirar bien de los filamentos? <a id="T3"></a>
Si el extrusor no puede empujar o tirar bien del filamento, puede hacer que el filamento se quede en el hotend y bloquee la entrada de un nuevo filamento.
##### :pill: Solución <a id="A3"></a>
1. Verifique y ajuste la presión del extrusor, consulte [:point_right: **aquí**](#HOW1).
2. **Actualice a extrusoras de doble engranaje, puede resolver eficazmente el problema del deslizamiento de hilos finos, consulte [:point_right: aquí][BMG]**.

#### :four: ¿Son correctas las configuraciones de corte? <a id="Q4"></a>
Si el hotend funciona bien al imprimir el archivo gcode de prueba que proporcionamos, pero se bloquea fácilmente al imprimir el archivo gcode con su propio corte, verifique la configuración de corte, especialmente los siguientes parámetros:
1. La longitud y la velocidad de tracción/empuje en ***"extrusor de conmutación"***, consulte **[:point_right: aquí][E4FAQ2]**.
2. El ajuste de ***"Longitud de retracción"*** no debe ser superior a 10 mm; consulte **[:point_right: aquí][E4FAQ3]**.
3. Si el volumen de filamentos extruidos por una extrusora en la misma capa es inferior a 10 mm, existe una cierta probabilidad de obstrucción. Por lo tanto, cuando dibuje impresiones 3D de varios colores o pinte colores en un modelo 3D en PrusaSlicer, preste atención al tamaño mínimo en la misma capa.
<!-- Como se muestra en [**esta figura**](./small_parts.jpg). -->

#### :five: Cuando se extrae el filamento del fusor, ¿habrá hilos largos? <a id="Q5"></a>
Habrá unas "cuerdas" en el extremo de los filamentos que se sacaron del fusor. Si las cuerdas son demasiado largas (para una longitud predeterminada de tracción/empuje de 80 mm, la longitud de las cuerdas debe ser inferior a 45 mm), puede bloquear la entrada del filamento. el hotend.
![](./cadenas.jpg)
##### :pill: Solución <a id="A5"></a>
- Modifique la longitud de empujar/tirar al cambiar la extrusora en "código G de cambio de herramienta". Para obtener más información, consulte **[:point_right: PrusaSlicer][E4FAQ4] [:point_right: Cura Silcer][E4FAQ5]**.
- Reemplace un filamento nuevo con cuerdas más cortas, generalmente la longitud de la cuerda es: **ABS <(*más corta que*) PLA+ < PLA < PLA-Slik.**
- Modificar la temperatura de la boquilla al imprimir/cortar.

#### :six: Cuando se extrae el filamento del hotend, ¿el extremo frontal se volverá demasiado grueso? <a id="Q6"></a>
Al cambiar el extrusor, el extremo del filamento extraído puede volverse ligeramente más grueso que el original. El hotend E4 permite que el diámetro máximo del filamento sea de 2,2 mm. Si el extremo se vuelve demasiado grueso y excede el diámetro permitido, es posible que el filamento no ingrese normalmente a la boquilla.
![](./frontal.jpg)
##### :pill: Solución <a id="A6"></a>
1. Reemplace los filamentos.
2. Este problema puede deberse a que el tubo interior de PTFE también está deformado (para E4V2). Consulte [:point_right: **aquí**](#HOW3) para reemplazarlo.

-----
## Manual de instalación y mantenimiento
### :hammer: Cómo reemplazar el conector del Hotend E4
[![](https://img.youtube.com/vi/LAQNazdMeu8/0.jpg)](https://www.youtube.com/watch?v=LAQNazdMeu8)      
[:gift: **Enlace de venta de accesorios**](https://www.aliexpress.com/item/3256801261619202.html)

### :hammer: Cómo ajustar la presión del extrusor a un valor adecuado <a id="HOW1"></a>
1. Cargue los filamentos en los extrusores pero no los cargue en el hotend, es decir, no conecte la guía de PTFE al hotend, como se muestra en [:point_right: **this Fig**](./E4FAQ-5.jpg).
2. Intente sujetar el filamento con el pulgar y el índice y luego gire el engranaje del extrusor con la mano.
![vídeo tutorial](./pressure_test.gif)
Si no puedes sujetar el filamento con los dedos, la presión del extrusor es suficiente. De lo contrario, ajuste la presión del extrusor.
![vídeo tutorial](./presión_adjust.gif)
:warning: **Tenga en cuenta que la presión debe ajustarse adecuadamente, pero no cuanto más grande, mejor**. Porque el engranaje puede empujar la misma posición del filamento hacia adelante y hacia atrás durante la impresión, lo que puede provocar que el filamento se raye. El filamento rayado no se puede transmitir a la boquilla durante la impresión, e incluso el filamento no puede ingresar normalmente al hotend.

### <a id="HOW2"></a> [:hammer: Cómo desmontar el hotend E4](./How_to_disassemble_E4_hotend/readme.md)
Si el filamento está obstruido dentro del hotend y no se puede sacar ni empujar hacia adentro, debe desmontar el hotend y limpiarlo, los pasos son los siguientes:
:warning: Espere a que el hotend se enfríe antes de operar.:warning:
![](E4-8.jpg)
1. Retire el conjunto del hotend del soporte X de la impresora 3D y retire la funda aislante de silicona.
2. Retire el cable de la carcasa del hotend.
3. Afloje los 2 tornillos que fijan el hotend.
4. Saque el hotend del disipador de calor.

### :hammer: Cómo reemplazar el tubo interior de PTFE (solo para E4V2) <a id="HOW3"></a>
Si la obstrucción es fácil de producir, se recomienda reemplazar también la tubería de PTFE incorporada, siguiendo los siguientes pasos:
![](E4-9.jpg)
1. Retire los tornillos que fijaron el sensor de temperatura y el calentador y retire el sensor de temperatura y el calentador.
2. Utilice una llave para quitar la boquilla.
3. Retire el tubo de PTFE incorporado que se va a reemplazar.
4. Instale un nuevo tubo de PTFE y utilice un cortador de papel para cortarlo.
5. El tubo de PTFE debe ser aproximadamente 0,5 mm más largo que la garganta, o puede quedar directamente al ras.
6. Utilice una pequeña varilla delgada de metal para girarlo hacia adentro, ya que al cortar el tubo de PTFE, su diámetro interior puede adelgazarse.
7. Vuelva a instalar el hotend en orden inverso.

-----
