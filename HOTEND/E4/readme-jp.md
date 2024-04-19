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
## :warning: 注意してください :warning:
- **使用する前に、[:book: E4 ホット エンド ユーザー マニュアル][E4GUIDE]を読んで、その動作原理と注意事項を理解してください。**
- **印刷する前に [:book: フィラメントのプリロード][PRELOAD] に注意してください。誤った操作を行うとホット エンドがブロックされる可能性があります。**
- **ノズルとベッドの間の距離に注意してください。距離が短すぎると、ホットエンドとステッカーが損傷する可能性があります。**
- **E4 ホットエンドの場合、スライス設定における後退長は 10mm を超えてはなりません。**
- **ホットエンド ケーブルを再接続した場合は、2 つのファン間の配線の区別に注意してください。**
 
----
## 4-IN-1-OUT 非混合カラー Hotend ユーザー ガイド
### [動作原理][E4WORKINGPRINCIPLE]
4-IN-1-OUT 非混合カラー ホット エンドは、ヒートシンク、ファンネル コレクター、加熱ブロック、ノズルなどで構成されます。印刷中、フィラメント 1 つだけが E4 ホット エンドにロードされます。 別の色のフィラメントに切り替えるとき、押出機は前の色のフィラメントを E4 ホットエンドから引き出し、別のフィラメントを E4 ホットエンドにロードする必要があります。 次の画像 (左から右) は、このプロセスを簡単に示しています。また、[:clapper: このアニメーション](./User_guide/E4_principle.gif) を参照して、E4 ホット エンドの動作原理を理解することもできます。
![](./User_guide/E4-5.jpg)

### :book: ユーザーガイド
- **[:book: ユーザーガイド](./User_guide/readme.md)**
- **[:green_book: ユーザーガイド PDF ファイル](./User_guide/E4_V2.jpg)**

### :mortar_board: gcode ファイルのテスト
- **[:beginner: gcode ファイルのテスト](./example/readme.md)**
- **[:surfer: その他のテスト gcode ファイル](https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer/test_gcode/E4)**

### [:hammer: トラブルシューティング](./FAQ/readme.md)

----
## 付録: ファンダクト
### [:arrow_down: ファンダクト stl ファイル](./Fan_Duct/fan_duct_e4.zip)

----