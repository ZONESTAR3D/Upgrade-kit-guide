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
## :warning: 주의하세요 :warning:
- **사용하기 전에 [:book: E4 hot end 사용자 매뉴얼][E4GUIDE]를 읽고 작동 원리와 주의 사항을 숙지하세요.**
- **인쇄 전 [:book: 필라멘트 사전 로딩][PRELOAD]에 주의하세요. 잘못된 조작으로 인해 핫엔드가 차단될 수 있습니다.**
- **노즐과 베드 사이의 거리에 주의하세요. 거리가 너무 짧으면 핫엔드와 스티커가 손상될 수 있습니다.**
- **슬라이싱 설정의 후퇴 길이는 E4 핫 엔드의 경우 10mm를 초과해서는 안 됩니다.**
- **핫엔드 케이블을 다시 연결하는 경우 두 팬 사이의 배선을 구별하도록 주의하세요.**
 
----
## 4-IN-1-OUT 비혼합 색상 핫엔드 사용자 가이드
### [작업 원리][E4WORKINGPRINCIPLE]
4-IN-1-OUT 비혼합 컬러 핫엔드는 방열판, 깔때기 수집기, 가열 블록, 노즐 등으로 구성됩니다. 인쇄 중에는 E4 핫엔드에 하나의 필라멘트만 로드됩니다. 다른 색상 필라멘트로 전환하는 동안 압출기는 이전 색상 필라멘트를 E4 핫 엔드에서 끌어낸 다음 다른 필라멘트를 E4 핫 엔드에 로드해야 합니다. 다음 이미지(왼쪽에서 오른쪽으로)는 이 과정을 간략하게 보여주며, [:clapper: 이 애니메이션](./User_guide/E4_principle.gif)을 참조하여 E4 핫엔드의 작동 원리를 이해할 수도 있습니다.
![](./User_guide/E4-5.jpg)

### :book: 사용자 가이드
- **[:book: 사용 설명서](./User_guide/readme.md)**
- **[:green_book: 사용 설명서 pdf 파일](./User_guide/E4_V2.jpg)**

### :mortar_board: gcode 파일 테스트
- **[:beginner: gcode 파일 테스트](./example/readme.md)**
- **[:surfer: 추가 테스트 gcode 파일](https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer/test_gcode/E4)**

### [:hammer: 문제 해결](./FAQ/readme.md)

----
## 부록: 팬 덕트
### [:arrow_down: 팬 덕트 stl 파일](./Fan_Duct/fan_duct_e4.zip)

----