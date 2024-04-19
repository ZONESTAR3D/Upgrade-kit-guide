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
## :warning: ПОЖАЛУЙСТА, ВНИМАНИЕ :warning:
- **Прочитайте [:book: Руководство пользователя E4 Hot End][E4GUIDE], чтобы понять принцип его работы и меры предосторожности перед использованием.**
- **Перед печатью обратите внимание на [:book: предварительную загрузку нити][PRELOAD]: неправильная операция может заблокировать горячий конец.**
- **Обратите внимание на расстояние между соплом и станиной, слишком маленькое расстояние может повредить хотэнд и наклейку.**
- **Длина втягивания в режиме нарезки не должна превышать 10 мм для горячего конца E4.**
- **Обратите внимание на различие проводов между двумя вентиляторами, если вы повторно подключили кабель горячего конца.**
 
----
## 4-В-1-ВЫХ Руководство пользователя Hotend без смешивания цветов
### [Принцип пробуждения][E4WORKINGPRINCIPLE]
Горячий конец несмешиваемых цветов 4-В-1-ВЫХ состоит из радиатора, воронкообразного коллектора, нагревательного блока, сопла и т. д. Во время печати в горячий конец E4 загружается только одна нить. При переключении на нить другого цвета экструдер должен вытащить нить предыдущего цвета из горячего конца E4, а затем загрузить другую нить в горячий конец E4. Следующее изображение (слева направо) кратко демонстрирует этот процесс. Вы также можете обратиться к [:clapper: этой анимации](./User_guide/E4_principle.gif), чтобы понять принцип работы горячего конца E4.
![](./User_guide/E4-5.jpg)

### :book: Руководство пользователя
- **[:book: Руководство пользователя](./User_guide/readme.md)**
- **[:green_book: PDF-файл руководства пользователя](./User_guide/E4_V2.jpg)**

### :mortar_board: Тестовый файл gcode
- **[:beginner: Тестовые файлы gcode](./example/readme.md)**
- **[:surfer: Больше тестовых файлов gcode](https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer/test_gcode/E4)**

### [:hammer: Устранение неполадок](./FAQ/readme.md)

----
## Приложение: Вентиляторный канал
### [:arrow_down: stl-файл воздуховода вентилятора](./Fan_Duct/fan_duct_e4.zip)

----