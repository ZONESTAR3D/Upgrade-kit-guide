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
# E4 および M4 ホットエンドに関する FAQ
- [**E4 ホットエンドと M4 ホットエンドの違いは何ですか?**](#A1)
- [**どのタイプのホットエンドを選択すればよいですか?**](#A2)
- [**フィラメントをホットエンドに正しくロードするにはどうすればよいですか?**](#A3)
- [**M4 ホットエンドと E4 ホットエンドのスライス設定の違いは何ですか**](#A4)
- [**M4 と E4 ホットエンドを切り替えるにはどうすればよいですか?**](#A5)


-----
## <a id="A1">E4 ホットエンドと M4 ホットエンドの違いは何ですか?</a>
- **M4 ホットエンド** は、異なる色のフィラメントを混合して新しい色のフィラメントを生成できます。 **E4 ホットエンド** にはこの機能がありません。
- **E4 ホットエンド** は、1 色または複数色の 3D オブジェクト (最大 4 色) の印刷に優れています。
- **M4 ホットエンド** は、グラデーション カラー 3D オブジェクトの印刷に優れており、(フィラメントを混合することにより) 4 色以上の 3D オブジェクトも印刷できます。
### E4 ホットエンドの動作原理
![](./E4/User_guide/E4_principle.gif)
### M4 ホットエンドの動作原理
[](https://github.com/ZONESTAR3D/Document-and-User-Guide/assets/29502731/2b9f4d75-b6fd-486f-aaa7-7a1163383316)

### E4 ホットエンドの利点
1. マルチカラー 3D オブジェクトを印刷する際の「エクストルーダー スイッチ プライム タワー」を小型化。
2. 1 色の 3D オブジェクトを印刷する場合の品質が向上します。
3. 同じ 3D オブジェクト上に異なるタイプのフィラメントを印刷することをサポートします。
### M4 ホットエンドの利点
1. 異なる色のフィラメントを混合して新しい色を作成することをサポートします。
2. グラデーションカラー印刷をサポートします。
3. より高い流量をサポートします。
![](M4VSE4.jpg)

-----
## <a id="A2"> M4 と E4 のどちらのホットエンドを選択すればよいですか?</a>
- グラデーション カラー 3D モデルを印刷する**必要がない**場合は、**E4 ホットエンド**を選択することをお勧めします。これにより、単色およびマルチカラー 3D プリントの印刷品質が向上します。
- **グラデーション カラー** 3D モデルを印刷する場合、または **異なる色のフィラメントを別の色に混合する**場合は、M4 ホットエンドを選択します。

-----
## <a id="A3"> フィラメントを正しくロード/アンロードする方法</a>
### M4 ホットエンド用
#### M4V6 ホットエンドにフィラメントをロードする手順:
##### [![](https://img.youtube.com/vi/-47yB95uIxI/0.jpg)](https://www.youtube.com/watch?v=-47yB95uIxI)
フィラメントを M4 ホットエンドにロードするときは、印刷中に使用する必要がある押出機の数に関係なく、***4 つのフィラメントすべてをホットエンドにロードする必要があります***。また、**すべてのフィラメントが確実にロードされていることを確認することが重要です。 印刷を開始する前に、ホットエンド***の下部にロードされます。
:warning: ***モノクロで印刷する場合でも、マルチカラーで印刷する場合でも、4 本のフィラメントすべてを M4V6 ホットエンドに取り付ける必要があります。***
1. エクストルーダーとホットエンドにロードする前に、フィラメントの前面を斜めペンチでカットします。
2. 4 本のフィラメントをすべての押出機に 1 つずつロードします。
3. 押出機のギアを回転させてフィラメントを 1 つずつロードします。すべてのフィラメントがホットエンドの内側 PTFE チューブに入るまで、各押出機を一度に 2 回転以上回転させないでください。各押出機でさらに 4 ～ 5 回転押し出します。 そして停止します。
:warning: ***ホットエンドのチャンネルが空の場合は、ホットエンドにフィラメントを供給しないでください。***
:warning: ***フィラメントに給電する前に、各チャンネルのフィラメントがホットエンドの底に到達していることを確認してください。***

#### M4V6 ホットエンドからフィラメントをアンロードする手順:
1. ノズルを加熱します (PLA の場合は 200℃ / PETG/ABS の場合は 230℃)。 ***Menu: Prepare>>Filament>>Preheat: 200/230***
2. 4 つのチャンネルすべてに同時にフィラメントを少なくとも 10 mm 供給します。 ***Menu: Prepare>>Filament>>Extruder: All; Prepare>>Filament>>Slowly Load***
3. ホットエンドからフィラメントをアンロードします。 ***Menu: Prepare>>Filament>>Slowly unload***
  
### E4 ホットエンド用
#### <a id = "PRELOAD_FILAMENT">E4 ホットエンドにフィラメントをロードする手順:</a>
##### [![](https://img.youtube.com/vi/FyHrAMytlT8/0.jpg)](https://www.youtube.com/watch?v=FyHrAMytlT8)
E4 ホットエンドの動作原理を理解している場合は、マルチカラーを印刷する場合、マシンはまず以前にロードされたフィラメントをホットエンドからアンロードし、次に次のフィラメントをロードする必要があることをすでに知っているはずです。 ただし、通常、**機械には印刷を開始する前にフィラメントの先端とノズルの間の距離を認識する機能がありません***。 したがって、<u>***「フィラメントのプリロード」***</u> と呼ばれるプロセスをセットアップする必要があります。これは、機械が事前に知っている適切な位置に細い糸を移動できるようにすることを目的としています。 オブジェクトを印刷します。
:warning: ***gcode ファイルで使用する必要があるエクストルーダーのフィラメントのみを E4 ホットエンドにロードする必要があります。***

### E4 ホットエンドからフィラメントをアンロードする手順:
1. ノズルを加熱します (PLA の場合は 200℃ / PETG/ABS の場合は 230℃)。 ***Menu: Prepare>>Filament>>Preheat: 200/230***
2. 使用済みエクストルーダーにフィラメントを少なくとも 10mm 供給します。 ***Menu: Prepare>>Filament>>Extruder: 1/2/3/4; Prepare>>Filament>>Slowly Load***.
3. フィラメントをホットエンドからアンロードします。 ***Menu: Prepare>>Filament>>Slowly unload***

-----
## <a id = "A4">M4 ホットエンドと E4 ホットエンドのスライス設定の違いは何ですか:</a>
:pushpin: これらの設定は、当社が提供する PrusaSlicer ソフトウェアのプロファイルに設定されています。 必要なのは、お使いのマシンとホットエンドのタイプに応じて正しい **プリンター プリセット** を選択することだけです。
### 多色印刷のスライス設定
マルチカラー印刷の場合、E4 ホットエンドと M4 ホットエンドのスライス設定は主に次のように異なります。
- **gcode を開始**
   - **E4 ホットエンド**の場合、印刷を開始する前に「フィラメントのプリロード」が必要です ([**Know Why**](#PRELOAD_FILAMENT))。詳細については、[**E4 ホットエンドの gcode の開始**][E4_STARTGCODE] を参照してください。
   - **M4 ホットエンド**の場合、4 色以下を印刷する場合、開始 gcode に特別な変更を加える必要はありません。 ただし、**4 色以上を印刷する必要がある** (異なる色のフィラメントを複数の色に混合する) 場合は、開始 gcode で色の混合比を設定できます。 詳細については、[**M4 ホットエンドを使用して 4 色以上の色を印刷する方法**][M4_MIXMULTICOLORPRINT]を参照してください。
- **エクストルーダーのリトラクション設定**
   - **E4 ホットエンド**の場合、推奨される**後退長**は 6 ～ 8mm (10mm 未満である必要があります) です。
   - **M4 ホットエンド**の場合、推奨**後退長**は 8 ～ 15mm です。
- **ワイプタワー（プライムタワー）**
:pushpin: 複数のエクストルーダープリンターをサポートするスライシングソフトウェアには、**「ワイプタワー(プライムタワー)」** オプションがあります。 なぜなら、プリンターがある押出機から別の押出機に切り替えるとき、多くの場合、最初にホットエンドにある前の色の細い糸をクリーニングする必要があるからです。 タワー消去オプションをオンにすると、スライシング ソフトウェアは gcode ファイルに「追加」プリントを生成し、ホット エンドに残っているフィラメントをクリーンアップします。
   - **E4 ホットエンド**の場合、必要なワイヤ タワーの体積は比較的小さくなります。
   - **M4 ホットエンド**の場合、必要なワイヤー タワーの体積は比較的大きくなります。
- **ツール交換 G コード**
   - **E4 ホットエンド**の場合、エクストルーダーを切り替えるときに、前の色のフィラメントをホットエンドから引き出し、次の色のフィラメントをホットエンドにロードする必要があります。 したがって、この操作を実現するにはツールチェンジ Gcode を設定する必要があります。 詳細については、[**E4 ホットエンド用ツール変更 G コード**][E4_TOOLCHANGE] を参照してください。
   - **M4 ホットエンド**の場合、**ツール変更 G コード**は必要ありません。

-----
## <a id="A5"> M4 ホットエンドと E4 ホットエンドを切り替える方法</a>
### 1. ホットエンド ハウジングの 3 本のネジを緩め、古いホットエンドをマシン (X プーリー) から取り外します。 次に、新しいホットエンドを機械 (X プーリー) に取り付け、ネジをロックします。
![](./E4/ユーザーガイド/E4-4.jpg)
### 2. 新しいホットエンドのワイヤをマシンに接続します。
![](./E4/User_guide/wiring1.jpg) ![](./E4/User_guide/wiring2.jpg)
### 3. LCD メニューでホットエンド タイプを設定します: *Control>>Configure>>Hotend Type*
![](./E4/User_guide/hotendtype-mix.jpg)![](./E4/User_guide/hotendtype-nonmix.jpg)
#### :pushpin: Z9V5 プリントヘッドのコネクタは機械の内部に隠されているため、ゴムリングを取り外してコネクタを引き抜く必要があります。
![](./Z9V5HotendWire.jpg)
### :warning: 注 1: LCD 画面に「ホットエンド タイプ」メニューが見つからない場合は、最新のファームウェアをプリンタにアップロードしてください。
[**:point_right: Z9V5 用ファームウェア**][FW_Z9V5] / [**:point_right: Z8P 用ファームウェア**][FW_Z8P] / [**:point_right: Z9M4 用ファームウェア**][FW_Z9M4]
### :warning: 注 2: ミックス カラー ホットエンドと非ミックス カラー ホットエンドは異なるスライス設定を使用する必要があります。区別するように注意してください。 間違ったスライス設定を使用すると、ホットエンドがブロックされる可能性があります。

-----