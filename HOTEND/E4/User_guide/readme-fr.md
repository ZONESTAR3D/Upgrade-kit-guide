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
## Manuel d'utilisation du Hotend E4
ZONESTAR 4-IN-1-OUT **Non mix color** hot end (appelé **E4 Hot end**) dispose de 4 canaux d'entrée et 1 buse, lors du changement de couleur, le filament de couleur précédent doit être déchargé ( retiré) de l’extrémité chaude, puis chargez le filament de couleur suivant.

### <a id="A1"> 1. Spécifications </a>
| Article | Paramètres | Article | Paramètres |
|:-------------------------:|:--------------------------:|:--------------------------:|:------------------------------:|
| Tension nominale | DC24 V/60 W maximum | Diamètre de la buse | Par défaut 0,4 mm<sup>1</sup> |
| Canal d'entrée | 4 | Modèle de buse | E3D V6 |
| Numéro de buses | 1 | Diamètre du filament | 1,75 mm |
| Chauffage | 24V/60W ⌀6x25mm | Capteur de température | Thermistance CTN 100K B3950 |
| Ventilateur de refroidissement | 4010/5000RPM/24V 0,15A | Ventilateur d'extrudeuse | 4010/5000RPM/24V 0,15A |
| Filaments de soutien | PLA/PLA+/PETG/ABS/ASA etc. Température de travail | 260 ℃ Maxime |
| Longueur du fil | 1 mètre | Dimensions extérieures | 50x60x75mm |
| Poids net | 220g | Poids brut | 350g |

### <a id="A2"> 2. Composants </a>
L'ensemble hot end E4 comprend les pièces/accessoires suivants :
![](./E4-2.jpg)
>
     1. Ventilateur de refroidissement 2. Boîtier 3. Trou d'installation du capteur de nivellement du lit 4. Vis montées
     5. Ventilateur de l'extrudeuse 6. Ventilateur "canard" imprimés 7. Bloc chauffant 8. Dissipateur thermique
     9. Buse 10. Cartouche chauffante 11. Capteur de température 12. Gorge
     13. Manchon en silicone 14. Raccords (connecteurs pneumatiques) 15. Câble

### <a id="A3"> 3. Fil </a>
![](./E4-3.jpg)

### <a id="A4"> 4. Installation & câblage </a>
La position de montage de l'extrémité chaude E4 est conforme à la « norme de montage de l'extrémité chaude ZONESTAR », qui peut être installée sur presque toutes les imprimantes 3D ZONESTAR, y compris les séries de produits P802, M8, D805S, Z8, Z9, Z10, etc.
#### 4.1 Installation
Retirez simplement les 3 vis derrière l'ensemble hotend et installez l'ensemble hotend E4 sur le support X de la machine.
![](./E4-4.jpg)
#### 4.2 Câblage
##### :loudspeaker: Attention 
- **Veuillez faire attention à distinguer les bornes 3 et 4**, car la couleur de leurs bornes est la même, mais la couleur des fils est différente.
Si les fils 3 et 4 sont connectés à l'envers, vous pouvez voir que la température de la buse affichée sur l'écran LCD sera beaucoup plus élevée que la température ambiante après la mise sous tension de la machine.
- Lors du branchement du terminal, **veillez à ne pas pousser le terminal métallique hors du boîtier en plastique**.
##### :loudspeaker: Veuillez noter
- **Le ventilateur de refroidissement doit être allumé** (lorsque la température de la partie chaude est supérieure à 60°C), sinon la partie chaude pourrait être bloquée voire endommagée.   
- Par défaut, la **tension de fonctionnement** du ventilateur et du chauffage à l'extrémité chaude est de **DC 24 V**.   
#### Veuillez suivre la définition des terminaux pour connecter le hotend à votre carte de contrôle.
- **Sans câble d'extension**
![](./filage1.jpg)
- **Avec câble d'extension**
![](./filage2.jpg)
#### 4.3 Définir le type de hotend sur le MENU LCD : Contrôle>>Configurer>>Type de hotend : Sans mélange
- :warning: Si votre imprimante ne dispose pas d'un écran TFT-LCD de 4,3", ignorez cette étape.
- :warning: Si vous ne voyez pas le menu sur l'écran LCD de votre imprimante, veuillez mettre à niveau vers la version la plus récente. [:link : **Lien de téléchargement du micrologiciel**][FIRMWARE]
##### ![](./hotendtype-nonmix.jpg)

### <a id="A5"> 5. Principe de fonctionnement </a>
L'extrémité chaude E4 (4-IN-1-OUT Non-Mix Color) est composée d'un dissipateur thermique, d'un collecteur à entonnoir, d'un bloc chauffant, d'une buse, etc. Pendant l'impression, un seul filament peut être chargé dans l'extrémité chaude. Lors du passage à un filament d'une autre couleur, l'extrudeuse retire le filament de couleur précédent de l'extrémité chaude E4, puis charge un autre filament dans l'extrémité chaude E4. L'image suivante (de gauche à droite) montre brièvement ce processus.
##### ![](./E4-5.jpg)
#### Vous pouvez également vous référer à une animation pour bien comprendre le principe de fonctionnement du hot end E4.
![](./E4_principle.gif).
##### :book: À propos de la "Tour Wipe"
Parce qu'il y a encore des filaments fondus de la couleur précédente dans la buse après le chargement d'un nouveau filament de couleur, nous devons donc « nettoyer » la buse avant de commencer à imprimer le nouveau filament de couleur. Sinon, la partie initiale imprimée sera de la couleur précédente mais pas de la nouvelle couleur comme prévu. La solution est d'ajouter une **"tour d'essuyage"** après le passage à une nouvelle extrudeuse dans le logiciel de tranchage.
Pour plus de détails, veuillez vous référer à [**:point_right: Slicing**](#A9).
:bulb: La tour Wipe est appelée "Prime tower" dans Cura Slicer et "Prime Pillar" dans Simplify3d Slicer.

### <a id="A6"> 6. Dimensions </a>
![](./E4_size.jpg)

### <a id="A7"> 7. Précharger les filaments </a>
#### 7.1 Pour une impression en une seule couleur
[![](https://img.youtube.com/vi/6aTF5QnFhi4/0.jpg)](https://www.youtube.com/watch?v=6aTF5QnFhi4)
#### 7.2 Pour l'impression multicolore
[![](https://img.youtube.com/vi/FyHrAMytlT8/0.jpg)](https://www.youtube.com/watch?v=FyHrAMytlT8)     
Avant d'imprimer, veuillez précharger les filaments dans la position appropriée de l'extrémité chaude afin que l'extrudeuse puisse charger en douceur les filaments dans et hors de l'extrémité chaude.    
- **Étape 1:** Chargez les filaments de l'extrudeuse et laissez-les s'étendre d'environ 10 mm hors des tubes PTFE.
- **Étape 2:** Branchez les tubes PTFE (avec filaments) dans le HOTEND.    
  - :pushpin: **S'il y a un filament dans l'extrémité chaude, chauffez et utilisez la buse, puis retirez-le d'abord. Référez-vous à [Décharger les filaments](#A8) pour le faire.**
  - :pushpin: Couper l'avant des filaments en une forme pointue avant de charger le filament.
  - :pushpin: Si l'extrudeuse n'a pas été utilisée pendant l'impression, il n'est pas nécessaire de charger le filament jusqu'à l'extrémité chaude.     
     ![](./E4-6.jpg)
  - :pushpin: Ajoutez quelques gcodes dans le **"Start gcode"** ([:point_right: View][STARTGCODE]) du logiciel de découpage à imprimer.    
     ![](./Preload_line.jpg)    
  - :pushpin: Ajoutez quelques gcodes dans le **"End gcode"** ([:point_right: View][ENDGCODE]) du logiciel de slicing pour retirer le dernier filament imprimé du hotend.  

### <a id="A8"> 8. Décharger les filaments </a>
Veuillez suivre les étapes ci-dessous pour décharger le filament du hotend :
- **Étape 1:** Chauffer la buse (190 degrés pour le PLA et 230 degrés pour l'ABS).
- **Étape 2:** Faites tourner l'engrenage de l'extrudeuse pour décharger le filament.
:star2: Certaines imprimantes 3D (par exemple Z9V5Pro) ont un menu « Filament » sur l'écran LCD, veuillez utiliser l'écran LCD et utiliser le menu ***« Préparer>>Filament »*** pour préchauffer la buse, choisir l'extrudeuse et décharger. filaments.

### <a id="A9"> 9. Découpage </a>
Guide de l'utilisateur (tutoriel vidéo) pour le logiciel de découpage PrusaSlicer/Cura/Simplify3d.
- **:+1: PrusaSlicer**, veuillez vous référer à :point_right : [**ici**][PRUSA].
- **Cura slicer**, veuillez vous référer à :point_right: [**ici**][CURA].
- **Simplify3d Slicer**, veuillez vous référer à :point_right: [**ici**][S3D].

### <a id="A10"> 10. Test du gcode </a>
Nous avons téléchargé quelques fichiers de test sur notre page Github, vous pouvez les télécharger depuis [**ici**](../example/readme.md).

### <a id="A11"> 11. Dépannage </a>
Si vous rencontrez des problèmes lors de l'utilisation du hot end E4, veuillez d'abord vous référer au [**guide de dépannage**](../FAQ/readme.md) pour trouver une solution. Si le problème ne peut toujours pas être résolu, veuillez contacter notre ingénieur du support technique par email: :email: support@zonestar3d.com.

----
### Lien de vente
[:gift: **ZONESTAR Offical Store**](https://bit.ly/39qDtKp)     
[:gift: **Aliexpress**](https://www.aliexpress.com/item/1005002951777699.html)

----