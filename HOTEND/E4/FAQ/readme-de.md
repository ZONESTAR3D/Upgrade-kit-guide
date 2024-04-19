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
## Fehlerbehebung beim E4-Hotend
Nachdem wir mehr als 1000 Drucktests durchgeführt haben, haben wir die möglichen Probleme am E4-Hotend zusammengefasst, insbesondere die Ursachen für verstopfte(s) Filament(e) und deren Lösungen als Referenz.
- Wenn Sie das Funktionsprinzip des E4-Hotends (4-IN-1-OUT Non-Mix-Color) nicht kennen, empfehlen wir Ihnen, dieses Dokument zu lesen ([**:point_down:E4-Hotend-Funktionsprinzip**](#F0 )) Erste.
- Der Grund, warum das E4-Hot-End nicht zum Drucken verwendet werden kann, liegt möglicherweise nicht am Hot-End selbst. Bevor Sie ein Urteil fällen, lesen Sie daher am besten [**:point_down:Test, ob das Hot-End normal funktionieren kann**](#F1), um einfach zu testen, ob das E4-Hot-End normal funktionieren kann.
- Wenn Ihr E4-Hot-End den Druck grundsätzlich abschließen kann, es aber Mängel am gedruckten Teil gibt, lesen Sie bitte [**:point_down:Problem mit Druckfehlern**](#F2).
- Wenn Ihr E4-Hot-End häufig stark verstopft ist, lesen Sie bitte [**:point_down:schwerwiegendes Verstopfungsproblem**](#F3).

-----
### <a id="F0"></a> Einige Dinge müssen Sie über das E4-Hotend wissen
#### :one: [Woking-Prinzip des E4-Hotends][E4FAQ1]
Wenn Sie sich über das Funktionsprinzip von E4 nicht im Klaren sind, klicken Sie bitte [**hier**][E4FAQ1], um es anzuzeigen. Um zu verstehen, wie E4 funktioniert, können Sie das Problem und die Ursache besser verstehen.
#### :two: Kurzbeschreibung der E4-Hotend-Struktur
Um die folgenden Dokumente besser durchsuchen zu können, lesen Sie bitte diesen Abschnitt, um die Namen und Funktionen der einzelnen Teile des E4-Hotends zu erfahren.
Es gibt zwei Versionen des E4-Hotends, die wir verkaufen (E4_V2 und E4_V3), sie unterscheiden sich kaum in der Verwendung und Druckqualität.
**Was E4_V3 verbessert hat:**
- Ändern Sie die Trichterstruktur, damit das Filament reibungslos in die Düse gelangt.
- Fügen Sie ein Kupferrohr hinzu, um die Wärmeableitung des Halses zu verbessern (Heat-Break-Teil).
![](./E4_struct.png)
:warning: Wenn Sie Teile/Zubehör des E4-Hotends austauschen müssen, unterscheiden Sie bitte die Version, die Sie besitzen.
#### Teilebeschreibung:
>
     1. Fitting (PC4-Trachealgelenk) 2. Kühlkörper 3. Trichterkollektor (E4V2) 4. Heat Break (Hals)
     5. Inneres PTFE-Rohr (E4V2) 6. Heizblock 7. Düse 8. Kupferrohr (E4V3) 9. Trichterkollektor (E4V3)
:pushpin: Wir haben die Größe des Heizaluminiumblocks aktualisiert und der neue Heizaluminiumblock ist links und rechts symmetrisch, sodass er den Luftauslass des Extruderventilators nicht blockiert. Zusätzlich wurden Schrauben zur Befestigung des Thermistors hinzugefügt.     
:pushpin: Wir haben ein V3H-Heizset auf den Markt gebracht, das zum Drucken von Hochtemperaturfilamenten wie PC, PET, PA usw. geeignet ist.
![](./HeatingBlock.jpg)

#### :three: Wählen Sie das entsprechende Filament <a id="choosefilament"></a>
Das E4-Hotend kann auf eine Vielzahl von Filamenten wie ABS, PLA, PLA+, PETG usw. angewendet werden. Wie Sie jedoch wissen, wird beim Wechseln des Extruders ein Filament aus dem Hotend entladen und dann das andere Filament wieder geladen. Daher sind die folgenden Eigenschaften des Filaments möglicherweise nicht gut für das E4-Hotend:
1. **Dehnt sich nach dem Erhitzen zu stark aus** – beim erneuten Laden kann das Hotend nicht betreten werden.
2. **Zu weich** – kann beim mehrfachen Be- und Entladen leicht durch das Zahnrad des Extruders zerkratzt werden.
3. **Mit langen Saiten nach dem Entladen** – blockieren Sie den Eintritt des Filaments in das Hotend.

Um die Zähigkeit, Fließfähigkeit und das Aussehen des Filaments zu verbessern, fügen die Filamenthersteller dem Filament einige Zusatzstoffe hinzu. Dies kann dazu führen, dass das Filament diese für E4-Hotends „unerreichbaren“ Eigenschaften aufweist. Wir empfehlen Ihnen daher, die folgenden Schritte zur Überprüfung durchzuführen Bevor Sie ein neues Filament verwenden: **Erwärmen Sie die Düse >> Laden Sie das Filament manuell in das Hotend >> Entleeren Sie ein wenig Filament (ca. 50 mm) >>Ziehen Sie es langsam aus dem Hotend heraus>> Überprüfen Sie die Größe und Saitenlänge am Ende des Filaments.**

-----
### <a id="F1"></a> Testen Sie, ob das Hotend normal funktionieren kann
![](https://github.com/ZONESTAR3D/Upgrade-kit-guide/assets/29502731/621f4c4c-c821-4602-b997-dc060fadedc2)
#### 1. Erhitzen Sie das heiße Ende (Düse) auf 200 ℃.
#### 2. Laden Sie Filamente nacheinander in jeden Kanal des Hot-Ends und beobachten Sie, ob das Filament aus der Düse fließen kann.
:warning: **Bitte beachten Sie:**
- **Schneiden Sie das vordere Ende flach, bevor Sie das Filament laden**
- **Drücken Sie das Filament langsam (<2 mm/s), wenn es die Düse erreicht.**
- **Verwenden Sie beim Herausziehen der Filamente eine höhere Geschwindigkeit (>10 mm/s).**

-----
### <a id="F2"></a> Der Druck kann normal abgeschlossen werden, es gibt jedoch Mängel an den gedruckten Objekten
Sie können auch auf ein solches Problem stoßen: Meistens kann der Druck normal durchgeführt werden, beim Drucken auf bestimmte Schichten treten jedoch offensichtliche Mängel auf, und während des Druckens ist gelegentlich das ungewöhnliche Kaka-Geräusch des Extruders zu hören.
##### :pill: Lösung <a id="A7"></a>
Dieses Problem wird normalerweise dadurch verursacht, dass beim Wechseln des Extruders das Filament nicht geladen und entladen wird. Bitte befolgen Sie zur Überprüfung die folgenden Schritte:
- [:point_up: **Überprüfen Sie den Extruderdruck**](#HOW1)
- **Filament prüfen oder ersetzen**[:point_up: 1](#Q5) [:point_up: 2](#Q6) [:point_up: 3](#choosefilament).
- [**Zug- und Drucklänge hinzufügen, indem Sie die Slicing-Einstellungen ändern**](#A5).
- [**Heizteil des Hotends neu installieren**](#HOW2)
- **Überprüfen Sie die PTFE-Führungen, die mit dem Extruder und dem Hotend verbunden sind.** Nach längerem Gebrauch kann sich der PTFE-Schlauch verformen (insbesondere der Teil, der die Anschlüsse verbindet), was den Widerstand des Filaments gegen die Bewegung im PTFE erheblich erhöht Röhren.
- **:+1: Upgrade auf Doppelzahnrad-Extruder.** Der Doppelzahnrad-Extruder kann die Kraft beim Drücken und Ziehen des feinen Drahts erheblich erhöhen und so die Möglichkeit einer Verstopfung verringern, die durch nicht reibungsloses Entfernen des feinen Drahts vom heißen Ende verursacht wird.
- [**Ersetzen Sie ein neues Hotend.**](https://bit.ly/39qDtKp)

-----
### <a id="F3"></a> Das E4-Hot-End ist häufig stark blockiert und kann überhaupt nicht drucken
Wenn Sie ein schwerwiegendes Verstopfungsproblem im Hotend feststellen, z. B. wenn das Filament nicht aus dem Hotend herausgezogen werden kann oder das Filament im Trichtersammler des Hotends verdreht und deformiert ist, befolgen Sie bitte die folgenden Schritte zur Überprüfung:
:Warnung:**HINWEIS:Warnung: Wenn Ihre Maschine mit Filament-Auslaufsensoren ausgestattet ist, wird empfohlen, diese zuerst zu umgehen und die Filamente direkt in die Extruder laden zu lassen, siehe [:point_right: hier](./E4FAQ -4.jpg)**.

#### :one: Funktioniert der Lüfter des Hotends gut? <a id="Q1"></a>
Der **[Lüfter des E4-Hotends][E4FAQ6]** sollte funktionieren (er kann die ganze Zeit funktionieren oder funktionieren, wenn die Düsentemperatur höher als 60 °C ist). Wenn der Lüfter nicht funktioniert, kann es leicht zu einer Verstopfung des Hotends kommen.

#### :two: Befindet sich die Düse zu nah an der Druckplatte? <a id="Q2"></a>
Wenn die Düse zu nah an der Druckplatte (Hotbed) ist, kann das Filament beim Drucken nicht aus der Düse extrudiert werden, es kann zu einer Blockierung des Hotends kommen, in schweren Fällen kann es dazu führen, dass das Filament im Trichter verdreht wird Sammler von Hotend. Dieses Problem tritt normalerweise beim Drucken der ersten Schicht auf.
##### :pill: Lösung <a id="A2"></a>
- Wenn Sie die erste Schicht drucken, verwenden Sie das Menü **Babyschritte**, um den Abstand von der Düse zur Druckplatte anzupassen.
- Achten Sie beim Schneiden auf die Einstellung der Höhe der ersten Schicht (150 % der Schichtdicke bzw. 80 % des Düsendurchmessers).

#### :three: Kann der Extruder die Filamente gut drücken und ziehen? <a id="Q3"></a>
Wenn der Extruder das Filament nicht gut drücken oder ziehen kann, kann dies dazu führen, dass das Filament im Hotend stecken bleibt und den Eintritt eines neuen Filaments blockiert.
##### :pill: Lösung <a id="A3"></a>
1. Überprüfen und stellen Sie den Druck des Extruders ein, siehe [:point_right: **hier**](#HOW1).
2. **Upgrade auf Dual Gear Extruder, es kann das Problem des Abrutschens feiner Gewinde effektiv lösen, siehe [:point_right: hier][BMG]**.

#### :four: Sind die Slicing-Einstellungen korrekt? <a id="Q4"></a>
Wenn das Hotend beim Drucken der von uns bereitgestellten Test-Gcode-Datei gut funktioniert, es aber beim Drucken der Gcode-Datei durch Ihr eigenes Slicing leicht blockiert wird, überprüfen Sie bitte die Slicing-Einstellungen, insbesondere die folgenden Parameter:
1. Die Länge und Zug-/Druckgeschwindigkeit des ***„Switching-Extruders“*** finden Sie **[:point_right: hier][E4FAQ2]**.
2. Die Einstellung von ***„Rückzugslänge“*** darf nicht größer als 10 mm sein, siehe **[:point_right: hier][E4FAQ3]**.
3. Wenn das Volumen der von einem Extruder in derselben Schicht extrudierten Filamente weniger als 10 mm beträgt, besteht eine gewisse Wahrscheinlichkeit einer Verstopfung. Wenn Sie also in PrusaSlicer einen mehrfarbigen 3D-Druck zeichnen oder Farbe auf ein 3D-Modell malen, achten Sie bitte auf die Mindestgröße auf derselben Ebene.

#### :five: Wenn das Filament aus dem Hotend herausgezogen wird, bleiben dann lange Fäden zurück? <a id="Q5"></a>
Am Ende der Filamente, die aus dem Hotend herausgezogen werden, befindet sich eine „Schnur“. Wenn die Fäden zu lang sind (bei einer standardmäßigen Zug-/Drucklänge von 80 mm sollte die Länge der Fäden weniger als 45 mm betragen), kann dies den Filamenteintritt blockieren das Hotend.
##### ![](./strings.jpg)
##### :pill: Lösung <a id="A5"></a>
- Ändern Sie die Push-/Pull-Länge beim Umschalten des Extruders im „Werkzeugwechsel-G-Code“. Einzelheiten finden Sie unter **[:point_right: PrusaSlicer][E4FAQ4] [:point_right: Cura Silcer][E4FAQ5]**.
- Ersetzen Sie ein neues Filament durch kürzere Saiten. Normalerweise beträgt die Länge der Saite: **ABS <(*kürzer als*) PLA+ < PLA < PLA-Slik.**
- Ändern Sie die Düsentemperatur beim Drucken/Schneiden.

#### :six: Wird das vordere Ende zu dick, wenn das Filament aus dem Hotend herausgezogen wird? <a id="Q6"></a>
Beim Wechseln des Extruders kann das Ende des herausgezogenen Filaments etwas dicker werden als das ursprüngliche E4-Hotend. Der maximale Filamentdurchmesser beträgt 2,2 mm. Wenn das Ende zu dick wird und den zulässigen Durchmesser überschreitet, gelangt das Filament möglicherweise nicht normal in die Düse.
##### ![](./front.jpg)
##### :pill: Lösung <a id="A6"></a>
1. Filamente ersetzen.
2. Dieses Problem liegt möglicherweise daran, dass auch der innere PTFE-Schlauch verformt ist (für E4V2). Bitte beziehen Sie sich auf [:point_right: **hier**](#HOW3), um ihn zu ersetzen.

-----
## Einrichtungs- und Wartungshandbuch
### :hammer: So tauschen Sie die Armatur des E4 Hotends aus
[![](https://img.youtube.com/vi/LAQNazdMeu8/0.jpg)](https://www.youtube.com/watch?v=LAQNazdMeu8)
#### [:gift: **Link zum Verkauf von Armaturen**](https://www.aliexpress.com/item/3256801261619202.html)

### :hammer: So stellen Sie den Extruderdruck auf einen richtigen Wert ein <a id="HOW1"></a>
1. Laden Sie die Filamente in die Extruder, aber nicht in das Hotend, d. h. verbinden Sie die PTFE-Führung nicht mit dem Hotend, wie in [:point_right: **diese Abbildung**](./E4FAQ-5.jpg).
2. Versuchen Sie, das Filament mit Daumen und Zeigefinger zu halten und drehen Sie dann das Zahnrad des Extruders von Hand.
#### ![Video-Tutorial](./pressure_test.gif)
Wenn Sie das Filament nicht mit den Fingern halten können, reicht der Druck des Extruders aus. Wenn nicht, passen Sie den Extruderdruck an.
#### ![Video-Tutorial](./pressure_adjust.gif)
:Warnung: **Bitte beachten Sie, dass der Druck entsprechend angepasst werden sollte, aber nicht je größer, desto besser**. Denn die gleiche Position des Filaments kann beim Drucken durch das Zahnrad hin und her geschoben werden, was zu Kratzern am Filament führen kann. Das zerkratzte Filament kann beim Drucken nicht auf die Düse übertragen werden und selbst das Filament kann nicht normal in das Hotend gelangen.

### <a id="HOW2"></a> [:hammer: So zerlegen Sie das E4-Hotend](./How_to_disassemble_E4_hotend/readme.md)
Wenn das Filament im Hotend verstopft ist und sich nicht herausziehen und hineinschieben lässt, müssen Sie das Hotend zerlegen und reinigen. Gehen Sie dabei wie folgt vor:
#### :warning: Warten Sie, bis das Hotend abgekühlt ist, bevor Sie es in Betrieb nehmen.:warning:
![](E4-8.jpg)
1. Entfernen Sie die Hotend-Baugruppe vom X-Träger des 3D-Druckers und nehmen Sie die Silikon-Isolierhülse ab.
2. Entfernen Sie das Kabel vom Hotend-Gehäuse.
3. Lösen Sie die 2 Schrauben, mit denen das Hotend befestigt ist.
4. Ziehen Sie das Hotend aus dem Kühlkörper.

### :hammer: So ersetzen Sie das innere PTFE-Rohr (nur für E4V2) <a id="HOW3"></a>
Wenn die Verstopfung leicht auftritt, wird empfohlen, auch das eingebaute PTFE-Rohr auszutauschen. Gehen Sie dabei wie folgt vor:
#### ![](E4-9.jpg)
1. Entfernen Sie die Schrauben, mit denen der Temperatursensor und die Heizung befestigt sind, und nehmen Sie den Temperatursensor und die Heizung ab.
2. Entfernen Sie die Düse mit einem Schraubenschlüssel.
3. Entfernen Sie das zu ersetzende eingebaute PTFE-Rohr.
4. Installieren Sie ein neues PTFE-Rohr und schneiden Sie es mit einem Papierschneider ab.
5. Das PTFE-Rohr sollte etwa 0,5 mm länger als der Hals sein, oder es kann direkt bündig sein.
6. Drehen Sie es mit einem kleinen dünnen Metallstab nach innen, da beim Schneiden des PTFE-Rohrs dessen Innendurchmesser möglicherweise dünner wird.
7. Installieren Sie das Hotend in umgekehrter Reihenfolge wieder.

-----