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
# E4 및 M4 핫엔드에 대한 FAQ
- [**E4와 M4 핫엔드의 차이점은 무엇인가요?**](#A1)
- [**어떤 종류의 핫엔드를 선택해야 하나요?**](#A2)
- [**핫엔드에 필라멘트를 올바르게 로드하는 방법은 무엇입니까?**](#A3)
- [**M4 핫엔드와 E4 핫엔드의 슬라이싱 설정 차이점은 무엇입니까**](#A4)
- [**M4와 E4 핫엔드 간에 어떻게 전환합니까?**](#A5)


-----
## <a id="A1">E4와 M4 핫엔드의 차이점은 무엇인가요?</a>
- **M4 핫엔드**는 다양한 색상의 필라멘트를 혼합하여 새로운 색상의 필라멘트를 생성할 수 있습니다. **E4 hotend**에는 이 기능이 없습니다.
- **E4 hotend**는 단색 또는 다중 색상 3D 개체(최대 4색)를 인쇄하는 데 적합합니다.
- **M4 핫엔드**는 그라데이션 색상의 3D 개체를 인쇄하는 데 적합하며 4콜로 이상의 3D 개체도 인쇄할 수 있습니다(필라멘트를 혼합하여).
### E4 핫엔드의 작동 원리
![](./E4/User_guide/E4_principle.gif)
### M4 핫엔드의 작동 원리
[](https://github.com/ZONESTAR3D/Document-and-User-Guide/assets/29502731/2b9f4d75-b6fd-486f-aaa7-7a1163383316)

### E4 핫엔드의 장점
1. 다중 색상 3D 개체를 인쇄하는 동안 더 작은 "압출기 스위치 프라임 타워".
2. 단일 색상의 3D 개체를 인쇄할 때 품질이 향상됩니다.
3. 동일한 3D 물체에 다양한 유형의 필라멘트를 인쇄할 수 있습니다.
### M4 핫엔드의 장점
1. 다양한 색상의 필라멘트를 새로운 색상으로 혼합하는 기능을 지원합니다.
2. 그라데이션 컬러 인쇄를 지원합니다.
3. 더 높은 유량을 지원합니다.
![](M4VSE4.jpg)

-----
## <a id="A2"> M4와 E4 중 어떤 핫엔드를 선택해야 하나요?</a>
- 그라디언트 색상 3D 모델을 인쇄할 **필요가 없는** 경우 **E4 핫엔드**를 선택하는 것이 좋습니다. 단일 색상 및 다중 색상 3D 인쇄를 인쇄할 때 더 나은 품질을 얻을 수 있습니다.
- **그라디언트 색상** 3D 모델을 인쇄하고 싶거나 **다른 색상의 필라멘트를 다른 색상으로 혼합**하려면 M4 핫엔드를 선택하세요.

-----
## <a id="A3"> 필라멘트를 올바르게 로드/언로드하는 방법</a>
### M4 핫엔드용
#### M4V6 핫엔드에 필라멘트를 로드하는 단계:
##### [![](https://img.youtube.com/vi/-47yB95uIxI/0.jpg)](https://www.youtube.com/watch?v=-47yB95uIxI)
M4 핫엔드에 필라멘트를 로드할 때 프린팅 중에 사용해야 하는 압출기 수에 관계없이 ***필라멘트 4개를 모두 핫엔드에 로드해야 하며, 그리고 인쇄를 시작하기 전에 모든 가는 실을 hotend의 아래쪽에 마운트해야 합니다***.     
:warning: ***단색 또는 다색 인쇄 여부에 관계없이 4개의 필라멘트를 모두 M4V6 핫엔드에 맞춰야 합니다.***      
1. 필라멘트를 압출기와 핫엔드에 장착하기 전에 대각선 펜치로 필라멘트의 앞부분을 자릅니다.
2. 4개의 필라멘트를 모든 Extruder에 하나씩 로딩합니다.
3. 압출기의 기어를 회전시켜 필라멘트를 하나씩 로드합니다. 모든 필라멘트가 핫엔드의 내부 PTFE 튜브에 들어갈 때까지 각 압출기를 한 번에 2바퀴 이상 회전하지 마십시오. 각 압출기마다 4~5바퀴 더 압출합니다. 그런 다음 중지하십시오.
:warning: ***핫엔드의 채널이 비어 있을 때 핫엔드에 필라멘트를 공급하지 마십시오.***
:warning: ***필라멘트를 공급하기 전에 각 채널의 필라멘트가 핫엔드 하단에 도달했는지 확인하세요.***

#### M4V6 핫엔드에서 필라멘트를 언로드하는 단계:
1. 노즐을 가열합니다(PLA는 200℃, PETG/ABS는 230℃). ***Menu: Prepare>>Filament>>Preheat: 200/230***
2. 4개 채널 모두에 동시에 최소 10mm의 필라멘트를 공급합니다. ***Menu: Prepare>>Filament>>Extruder: All; Prepare>>Filament>>Slowly Load***
3. 핫엔드에서 필라멘트를 언로드합니다. ***Menu: Prepare>>Filament>>Slowly unload***
  
### E4 핫엔드의 경우
#### <a id = "PRELOAD_FILAMENT">E4 핫엔드에 필라멘트를 로드하는 단계:</a>
##### [![](https://img.youtube.com/vi/FyHrAMytlT8/0.jpg)](https://www.youtube.com/watch?v=FyHrAMytlT8)
E4 핫엔드의 작동 원리를 이해했다면 다중 색상을 인쇄할 때 기계가 먼저 핫엔드에서 이전에 로드한 필라멘트를 언로드한 후 다음 필라멘트를 로드해야 한다는 것을 이미 알고 있어야 합니다. 그러나 일반적으로 ***프린팅을 시작하기 전에 필라멘트 앞부분과 노즐 사이의 거리를 인식하는 기능이 기계에 없습니다***. 따라서 <u>***"필라멘트 사전 로드"***</u>라는 프로세스를 설정해야 합니다. 이는 기계가 이전에 기계에 알려진 적절한 위치로 미세한 실을 이동할 수 있도록 하는 것을 목표로 합니다. 개체를 인쇄합니다.
:warning: ***gcode 파일에 사용해야 하는 압출기의 필라멘트만 E4 핫엔드에 로드해야 합니다.***

### E4 핫엔드에서 필라멘트를 언로드하는 단계:
1. 노즐을 가열합니다(PLA는 200℃, PETG/ABS는 230℃). ***Menu: Prepare>>Filament>>Preheat: 200/230***
2. 사용한 Extruder에 필라멘트를 10mm 이상 공급합니다. ***Menu: Prepare>>Filament>>Extruder: 1/2/3/4; Prepare>>Filament>>Slowly Load***
3. 핫엔드에서 필라멘트를 꺼냅니다. ***Menu: Prepare>>Filament>>Slowly unload***

-----
## <a id = "A4">M4와 E4 핫엔드의 슬라이싱 설정 차이점은 무엇입니까:</a>
:pushpin: 이 설정은 당사가 제공하는 PrusaSlicer 소프트웨어의 프로필에 설정되어 있습니다. 귀하의 기계와 핫엔드 유형에 따라 올바른 **프린터 사전 설정**을 선택하기만 하면 됩니다.
### 다색 인쇄를 위한 슬라이스 설정
다중 색상 인쇄의 경우 E4 핫엔드와 M4 핫엔드의 슬라이싱 설정은 주로 다음과 같이 다릅니다.
- **gcode 시작**
   - **E4 핫엔드**의 경우 프린팅을 시작하기 전에 "필라멘트를 미리 로드"해야 합니다([**이유를 알다**](#PRELOAD_FILAMENT)). 자세한 내용은 [**E4의 시작 gcode를 참조하세요. 핫엔드**][E4_STARTGCODE].
   - **M4 핫엔드**의 경우 4색 이하로 인쇄하는 경우 시작 gcode를 특별히 변경할 필요가 없습니다. 하지만 **4개 이상의 색상을 인쇄해야 하는 경우**(다른 색상의 필라멘트를 여러 색상으로 혼합) 시작 gcode에서 색상 혼합 비율을 설정할 수 있습니다. 자세한 내용은 [**M4 핫엔드를 사용하여 4색 이상 인쇄하는 방법**][M4_MIXMULTICOLORPRINT]을 참조하세요.
- **압출기의 후퇴 설정**
   - **E4 핫엔드**의 경우 권장 **후퇴 길이**는 6~8mm(10mm 미만이어야 함)입니다.
   - **M4 핫엔드**의 권장 **후퇴 길이**는 8~15mm입니다.
- **와이프 타워(프라임 타워)**      
:pushpin: 여러 압출기 프린터를 지원하는 슬라이싱 소프트웨어에는 **"Wipe Tower(프라임 타워)"** 옵션이 있습니다. 프린터가 한 압출기에서 다른 압출기로 전환할 때 먼저 핫 엔드에 있는 이전 색상의 가는 실을 청소해야 하는 경우가 많기 때문입니다. 삭제 타워 옵션을 켠 후 슬라이싱 소프트웨어는 gcode 파일에 "추가" 인쇄물을 생성하여 핫 엔드에 남아 있는 필라멘트를 정리할 수 있습니다.
   - **E4 핫엔드**의 경우 와이어 타워에 필요한 부피가 상대적으로 작습니다.
   - **M4 핫엔드**의 경우 와이어 타워에 필요한 부피가 상대적으로 큽니다.
- **공구 변경 G 코드**
   - **E4 핫엔드**의 경우 Extruder를 전환할 때 이전 컬러 필라멘트를 핫엔드에서 빼낸 후 다음 컬러 필라멘트를 핫엔드에 장착해야 합니다. 따라서 이 작업을 수행하려면 도구 변경 Gcode를 설정해야 합니다. 자세한 내용은 [**E4 핫엔드용 공구 변경 G 코드**][E4_TOOLCHANGE]를 참조하세요.
   - **M4 핫엔드**의 경우 **공구 변경 G 코드**가 필요하지 않습니다.

-----
## <a id="A5"> M4 핫엔드와 E4 핫엔드 간 전환 방법</a>
### 1. 핫엔드 하우징에 있는 나사 3개를 풀고 기계(x 풀리)에서 기존 핫엔드를 제거합니다. 그런 다음 새 핫엔드를 기계(x 풀리)에 설치하고 나사를 잠급니다.
![](./E4/User_guide/E4-4.jpg)
### 2. 새로운 핫엔드의 전선을 기계에 연결합니다.
![](./E4/User_guide/wiring1.jpg) ![](./E4/User_guide/wiring2.jpg)
### 3. LCD 메뉴에서 핫엔드 유형을 설정합니다: *control>>Configure>>Hotend Type*
![](./E4/User_guide/hotendtype-mix.jpg)![](./E4/User_guide/hotendtype-nonmix.jpg)
#### :pushpin: Z9V5 프린트 헤드의 커넥터는 기계 내부에 숨겨져 있으므로 고무 링을 제거하고 커넥터를 당겨야 합니다.
![](./Z9V5HotendWire.jpg)
### :warning: 참고 1: LCD 화면에서 "핫엔드 유형" 메뉴를 찾을 수 없는 경우 최신 펌웨어를 프린터에 업로드하십시오.
[**:point_right: Z9V5용 펌웨어**][FW_Z9V5] / [**:point_right: Z8P용 펌웨어**][FW_Z8P] / [**:point_right: Z9M4용 펌웨어**][FW_Z9M4]
### :warning: 참고 2: 혼합 색상 핫엔드와 비혼합 색상 핫엔드는 서로 다른 슬라이스 설정을 사용해야 하므로 구별에 주의하십시오. 잘못된 슬라이스 설정을 사용하면 핫엔드가 차단될 수 있습니다.

-----