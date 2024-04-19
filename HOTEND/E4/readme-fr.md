[E4GUIDE]: https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/E4/User_guide/readme.md
[PRELOAD]: https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/User_guide#7-pre-load-filaments
[E4WORKINGPRINCIPLE]:https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/E4/User_guide/readme.md#5-working-principle

----
## <a id="choose-language">:globe_with_meridians: Choose language </a>
[![](../../lanpic/EN.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/readme.md)
[![](../../lanpic/ES.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/readme-es.md)
[![](../../lanpic/PT.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/readme-pt.md)
[![](../../lanpic/FR.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/readme-fr.md)
[![](../../lanpic/DE.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/readme-de.md)
[![](../../lanpic/IT.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/readme-it.md)
[![](../../lanpic/RU.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/readme-ru.md)
[![](../../lanpic/JP.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/readme-jp.md)
[![](../../lanpic/KR.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/readme-kr.md)
<!-- [![](../../lanpic/SA.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/E4/readme-ar.md) -->

----
## :warning: ATTENTION S'IL VOUS PLAÎT :warning:
- **Lisez le [:book: E4 hot end user manual][E4GUIDE]pour comprendre son principe de fonctionnement et ses précautions avant utilisation.**
- **Faites attention à [:book: pre-loading filament][PRELOAD] avant d'imprimer, une opération incorrecte peut bloquer la partie chaude.**
- **Faites attention à la distance entre la buse et le lit, une distance trop petite peut endommager l'extrémité chaude et l'autocollant.**
- **La longueur de rétraction dans le réglage de tranchage ne doit pas dépasser 10 mm pour l'extrémité chaude E4.**
- **Faites attention à bien distinguer le câblage entre les deux ventilateurs si vous avez reconnecté le câble de l'extrémité chaude.**
 
----
## Guide de l'utilisateur du Hotend 4-IN-1-OUT sans mélange de couleurs
### [Principe de Woking][E4WORKINGPRINCIPLE]
L'extrémité chaude 4-IN-1-OUT Non-Mix Color est composée d'un dissipateur thermique, d'un collecteur en entonnoir, d'un bloc chauffant, d'une buse, etc. Pendant l'impression, un seul filament est chargé dans l'extrémité chaude E4. Lors du passage à un filament d'une autre couleur, l'extrudeuse doit retirer le filament de couleur précédent de l'extrémité chaude E4, puis charger un autre filament dans l'extrémité chaude E4. L'image suivante (de gauche à droite) illustre brièvement ce processus, et vous pouvez également vous référer à [:clapper: this animation](./User_guide/E4_principle.gif) pour comprendre le principe de fonctionnement du hot end E4.
![](./Guide_utilisateur/E4-5.jpg)

### :book: Guide de l'utilisateur
- **[:book: Guide de l'utilisateur](./User_guide/readme.md)**
- **[:green_book: fichier pdf du guide de l'utilisateur](./User_guide/E4_V2.jpg)**

### :mortar_board: Test du fichier gcode
- **[:beginner: tester les fichiers gcode](./example/readme.md)**
- **[:surfer: Plus de fichiers gcode de test](https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer/test_gcode/E4)**

### [:hammer: Dépannage](./FAQ/readme.md)

----
## Annexe: Conduit de ventilation
### [:arrow_down: Fichier stl de conduit de ventilateur](./Fan_Duct/fan_duct_e4.zip)

----