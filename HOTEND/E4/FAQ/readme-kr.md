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
## E4 핫엔드 문제 해결
1000회 이상의 프린트 테스트를 거쳐 E4 핫엔드에서 발생할 수 있는 문제, 특히 필라멘트 막힘(막힘)의 원인과 해결 방법을 정리하여 참고하실 수 있습니다.
- E4(4-IN-1-OUT 비혼합 색상) 핫엔드의 작동 원리를 모르는 경우 이 문서를 읽어 보시기 바랍니다([**:point_down:E4 핫엔드 작동 원리**](#F0 )) 첫 번째.
- E4 핫엔드를 인쇄에 사용할 수 없는 이유는 핫엔드 자체에서 비롯된 것이 아닐 수도 있습니다. 따라서 판단 전, [**:point_down:핫엔드가 정상적으로 작동하는지 테스트**](#F1)를 참고하여 간단히 E4 핫엔드가 정상적으로 작동하는지 테스트해 보시는 것이 가장 좋습니다.
- E4 핫엔드를 사용하시면 기본적으로 프린팅은 완료되지만, 프린팅된 부분에 결함이 있는 경우 [**:point_down:인쇄 결함 문제**](#F2)를 참조하세요.
- E4 핫엔드가 자주 막히는 경우 [**:point_down:심각한 막힘 문제**](#F3)를 참조하세요.

-----
### <a id="F0"></a> E4 핫엔드에 대해 알아야 할 몇 가지 사항
#### :one: [E4 핫엔드의 작동 원리][E4FAQ1]
E4의 작동 원리가 명확하지 않은 경우 [**여기**][E4FAQ1]를 클릭하여 E4의 작동 방식을 이해하면 문제와 원인을 이해하는 데 도움이 됩니다.
#### :two: E4 핫엔드 구조 개요
다음 문서를 더 잘 찾아보려면 이 섹션을 읽고 E4 핫엔드 각 부분의 이름과 기능을 알아보세요.
우리가 판매하는 E4 핫엔드에는 두 가지 버전(E4_V2 및 E4_V3)이 있으며 사용 및 인쇄 품질에는 큰 차이가 없습니다.
**E4_V3의 개선 사항:**
- 필라멘트가 노즐 내부로 원활하게 들어갈 수 있도록 깔때기 구조를 수정합니다.
- 목구멍(열 차단부)의 방열을 개선하기 위해 쿠퍼 튜브를 추가합니다.
![](./E4_struct.png)
:warning: E4 핫엔드의 부품/액세서리를 교체해야 하는 경우 보유하고 있는 버전을 구별하십시오.
#### 부품 설명:
>
     1. 피팅(PC4 기관 관절) 2. 방열판 3. 깔때기 수집기(E4V2) 4. 열 브레이크(목)
     5. 내부 PTFE 튜브(E4V2) 6. 히팅 블록 7. 노즐 8. 구리 튜브(E4V3) 9. 깔대기 콜렉터(E4V3)
- :pushpin: 가열 알루미늄 블록의 크기를 업데이트했으며, 새로운 가열 알루미늄 블록이 좌우 대칭이므로 압출기 팬의 공기 배출구를 막지 않습니다. 또한 서미스터를 고정하기 위해 나사가 추가되었습니다.
- :pushpin: PC, PET, PA 등과 같은 고온 필라멘트 프린팅에 적합한 V3H 가열 키트를 출시했습니다.
![](./HeatingBlock.jpg)

#### :three: 적절한 필라멘트를 선택하세요 <a id="choose필라멘트"></a>
E4 핫엔드는 ABS, PLA, PLA+, PETG 등 다양한 필라멘트에 적용 가능합니다. 하지만 아시다시피 Extruder를 전환하는 동안 핫엔드에서 필라멘트가 Unload되었다가 다시 Anthoer 필라멘트를 Load하게 됩니다. 따라서 다음과 같은 필라멘트 특성은 E4 핫엔드에 적합하지 않을 수 있습니다.
1. **가열 후 너무 많이 팽창함** -- 다시 로드할 때 핫엔드에 들어갈 수 없습니다.
2. **너무 부드럽습니다** -- 다중 로드/언로드 중에 압출기 기어로 긁히기 쉽습니다.
3. **언로드 후 긴 끈으로** -- 필라멘트가 핫엔드에 들어가는 것을 차단합니다.     
필라멘트의 강인성, 유동성 및 외관을 개선하기 위해 필라멘트 제조업체는 필라멘트에 일부 첨가제를 추가합니다. 이로 인해 필라멘트가 E4 핫엔드에 "접근할 수 없는" 특성을 갖게 될 수 있으므로 아래 단계를 수행하여 확인하는 것이 좋습니다. 새 필라멘트를 사용하기 전에: **노즐 가열 >> 핫엔드에 수동으로 필라멘트 넣기 >> 약간의 필라멘트(50mm 정도) 퍼지 >> 핫엔드에서 천천히 빼내기 >> 크기와 줄 길이를 핫엔드에서 확인하세요. 필라멘트의 끝.**

-----
### <a id="F1"></a> 핫엔드가 정상적으로 작동하는지 테스트
![](https://github.com/ZONESTAR3D/Upgrade-kit-guide/assets/29502731/621f4c4c-c821-4602-b997-dc060fadedc2)
#### 1. 핫엔드(노즐)를 200℃로 가열합니다.
#### 2. 핫엔드의 각 채널에 필라멘트를 하나씩 장착한 후 노즐에서 필라멘트가 흘러나오는지 확인합니다.
:warning: **참고:**
- **필라멘트를 장착하기 전에 앞부분을 평평하게 잘라주세요**
- **필라멘트가 노즐에 도달하면 천천히 밀어줍니다(<2mm/s).**
- **필라멘트를 잡아당길 때 더 빠른 속도(>10mm/s)를 사용하세요.**

-----
### <a id="F2"></a> 정상적으로 프린팅이 완료되었으나, 프린팅된 개체에 결함이 있습니다.
이런 문제가 발생할 수도 있습니다. 대부분 정상적으로 인쇄가 가능하지만 특정 레이어로 인쇄할 때 명백한 결함이 있으며 인쇄 중에 압출기의 비정상적인 카카 소음이 간헐적으로 들립니다.
##### :pill: 해결 방법 <a id="A7"></a>
이 문제는 일반적으로 압출기를 전환할 때 필라멘트를 로드 및 언로드하지 못하여 발생합니다. 아래 단계에 따라 확인하십시오.
- [:point_up: **압출기 압력 확인**](#HOW1)
- **필라멘트 확인 또는 교체**[:point_up: 1](#Q5) [:point_up: 2](#Q6) [:point_up: 3](#choose필라멘트).
- [**슬라이싱 설정을 수정하여 당기고 밀기 길이를 추가하세요**](#A5).
- [**핫엔드 발열부 재설치**](#HOW2)
- **Extruder와 핫엔드에 연결된 PTFE 가이드를 확인하세요.** 사용 기간이 지나면 PTFE 튜브(특히 피팅을 연결하는 부분)가 변형될 수 있으며, 이는 필라멘트가 PTFE 내부로 이동하는 저항을 크게 증가시킵니다. 튜브.
- **:+1: 듀얼 기어 압출기로 업그레이드.** 더블 기어 압출기는 가는 와이어를 밀고 당기는 힘을 크게 증가시켜 뜨거운 끝 부분에서 가는 와이어를 원활하게 제거하지 못해 발생하는 막힘 가능성을 줄입니다.
- [**새 핫엔드를 교체하세요.**](https://bit.ly/39qDtKp)

-----
### <a id="F3"></a> E4 핫엔드가 심각하게 차단되어 인쇄할 수 없는 경우가 많습니다.
핫엔드에서 필라멘트를 빼낼 수 없거나 핫엔드의 깔때기 수집기에서 필라멘트가 꼬이거나 변형되는 등 핫엔드에서 심각한 막힘 문제를 발견한 경우 다음 단계에 따라 확인하십시오.
:warning: 참고 :warning: **기기에 필라멘트 소모 센서가 장착되어 있는 경우 먼저 이를 우회하고 필라멘트가 압출기에 직접 로드되도록 하는 것이 좋습니다. [:point_right: 여기](./E4FAQ를 참조하세요. -4.jpg)**.

#### :one: 핫엔드의 냉각팬은 잘 돌아가나요? <a id="Q1"></a>
**[E4 핫엔드의 냉각 팬][E4FAQ6]**이 작동해야 합니다(항상 작동하거나 노즐 온도가 60°C보다 높을 때 작동할 수 있음). 냉각팬이 작동하지 않으면 핫엔드가 막히기 쉽습니다.

#### :two: 노즐이 인쇄판에 너무 가깝나요? <a id="Q2"></a>
노즐이 인쇄판(핫베드)에 너무 가까이 붙어 있으면 인쇄 시 노즐에서 필라멘트가 압출되지 않아 핫엔드가 막힐 수 있으며, 심한 경우 깔때기 속에서 필라멘트가 꼬이는 현상이 발생할 수 있습니다. 핫엔드 수집가. 이 문제는 일반적으로 첫 번째 레이어를 인쇄할 때 발생합니다.
##### :pill: 해결 방법 <a id="A2"></a>
- 첫 번째 레이어를 출력할 때 **babysteps** 메뉴를 사용하여 노즐에서 인쇄판까지의 거리를 조정합니다.
- 슬라이스 시 첫 번째 레이어의 높이 설정(레이어 두께의 150% 또는 노즐 직경의 80%)에 주의하세요.

#### :three: Extruder가 필라멘트를 잘 밀고 당길 수 있나요? <a id="Q3"></a>
Extruder가 필라멘트를 잘 밀거나 당기지 못하는 경우, 필라멘트가 핫엔드에 정체되어 새로운 필라멘트가 들어가는 것을 막을 수 있습니다.
##### :pill: 해결 방법 <a id="A3"></a>
1. Extruder의 압력을 확인하고 조정하세요. [:point_right: **여기**](#HOW1)를 참조하세요.
2. **듀얼 기어 압출기로 업그레이드하면 가는 실이 미끄러지는 문제를 효과적으로 해결할 수 있습니다. [:point_right: 여기][BMG]**를 참조하세요.

#### :four: 슬라이싱 설정이 올바른가요? <a id="Q4"></a>
당사에서 제공한 테스트 gcode 파일을 인쇄할 때 핫엔드가 잘 작동하지만 자체 슬라이스로 gcode 파일을 인쇄할 때 쉽게 차단되는 경우, 슬라이싱 설정, 특히 다음 매개변수를 확인하십시오.
1. ***"전환 압출기"***의 길이 및 당김/밀기 속도는 **[:point_right: 여기][E4FAQ2]**를 참조하세요.
2. ***"후퇴 길이"*** 설정은 10mm를 초과할 수 없습니다. **[:point_right: 여기][E4FAQ3]**를 참조하십시오.
3. 동일한 층의 Extruder에서 압출되는 필라멘트의 양이 10mm 미만인 경우 막힘이 발생할 가능성이 있습니다. 따라서 PrusaSlicer에서 여러 색상의 3D 프린트를 그리거나 3D 모델에 색상을 칠할 때 동일한 레이어의 최소 크기에 주의하세요.
<!-- [**이 그림**](./small_parts.jpg)과 같습니다. -->

#### :five: 핫엔드에서 필라멘트를 빼내면 긴 끈이 생기나요? <a id="Q5"></a>
핫엔드에서 뽑아낸 필라멘트 끝에 "끈"이 있습니다. 문자열이 너무 길면(기본 80mm 당기기/밀기 길이의 경우 문자열 길이가 45mm 미만이어야 함) 필라멘트가 들어가는 것을 막을 수 있습니다. 핫엔드.
##### ![](./strings.jpg)
##### :pill: 해결 방법 <a id="A5"></a>
- "공구 변경 G 코드"에서 압출기 전환의 밀기/당기기 길이를 수정합니다. 자세한 내용은 **[:point_right: PrusaSlicer][E4FAQ4] [:point_right: Cura Silcer][E4FAQ5]**를 참조하세요.
- 새 필라멘트를 더 짧은 스트링으로 교체하십시오. 일반적으로 스트링 길이는 **ABS <(*보다 짧음*) PLA+ < PLA < PLA-Slik.**입니다.
- 인쇄/슬라이싱 시 노즐 온도를 수정합니다.

#### :six: 핫엔드에서 필라멘트를 빼내면 앞부분이 너무 두꺼워지나요? <a id="Q6"></a>
Extruder를 전환하면 뽑아낸 필라멘트의 끝부분이 원래 필라멘트보다 약간 두꺼워질 수 있으며, E4 핫엔드에서는 최대 필라멘트 직경이 2.2mm까지 허용됩니다. 끝부분이 너무 두꺼워져 허용 직경을 초과할 경우 필라멘트가 노즐에 정상적으로 들어가지 못할 수 있습니다.
##### ![](./front.jpg)
##### :pill: 해결 방법 <a id="A6"></a>
1. 필라멘트를 교체하세요.
2. 이 문제는 내부 PTFE 튜브도 변형되었기 때문일 수 있습니다(E4V2의 경우). 교체하려면 [:point_right: **여기**](#HOW3)를 참조하세요.

-----
## 설치 및 유지 관리 매뉴얼
### :hammer: E4 핫엔드 피팅 교체 방법
[![](https://img.youtube.com/vi/LAQNazdMeu8/0.jpg)](https://www.youtube.com/watch?v=LAQNazdMeu8)
#### [:gift: **피팅 판매 링크**](https://www.aliexpress.com/item/3256801261619202.html)

### :hammer: 압출기 압력을 적절한 값으로 조정하는 방법 <a id="HOW1"></a>
1. 필라멘트를 압출기에 로드하되 핫엔드에는 로드하지 마십시오. 즉, PTFE 가이드를 핫엔드에 연결하지 마십시오. [:point_right: **이 그림**](./E4FAQ-5.jpg)과 같습니다.
2. 엄지와 검지로 필라멘트를 잡은 후 손으로 Extruder의 기어를 회전시킵니다.
#### ![동영상 튜토리얼](./pressure_test.gif)
손가락으로 필라멘트를 잡을 수 없다면 압출기의 압력으로 충분합니다. 그렇지 않은 경우 압출기 압력을 조정하십시오.
#### ![동영상 튜토리얼](./pressure_adjust.gif)
:warning: **압력은 적절하게 조정해야 하지만 클수록 좋지는 않습니다**. 왜냐하면 프린팅 중 동일한 위치의 필라멘트가 기어에 의해 앞뒤로 밀려서 필라멘트가 긁힐 수 있기 때문입니다. 긁힌 필라멘트는 출력 중에 노즐로 전달되지 않으며, 필라멘트라도 핫엔드에 정상적으로 들어가지 못합니다.

### <a id="HOW2"></a> [:hammer: E4 핫엔드 분해 방법](./How_to_disassemble_E4_hotend/readme.md)
필라멘트가 핫엔드 내부에 막혀서 빼거나 밀어넣을 수 없는 경우 핫엔드를 분해하여 청소해야 합니다. 다음 단계를 따르세요.
#### :warning: 작동하기 전에 핫엔드가 식을 때까지 기다리십시오.:warning:
![](E4-8.jpg)
1. 3D 프린터의 X 캐리어에서 핫엔드 어셈블리를 제거하고 실리콘 절연 슬리브를 떼어냅니다.
2. 핫엔드 하우징에서 케이블을 제거합니다.
3. 핫엔드를 고정하고 있는 나사 2개를 풀어줍니다.
4. 핫엔드를 방열판에서 당겨 빼냅니다.

### :hammer: 내부 PTFE 파이프 교체 방법(E4V2에만 해당) <a id="HOW3"></a>
막힘이 발생하기 쉬운 경우 내장 PTFE 파이프도 교체하는 것이 좋습니다. 단계는 다음과 같습니다.
#### ![](E4-9.jpg)
1. 온도센서와 히터를 고정하고 있는 나사를 제거하고 온도센서와 히터를 떼어냅니다.
2. 렌치를 사용하여 노즐을 제거합니다.
3. 교체할 내장 PTFE 파이프를 제거합니다.
4. 새 PTFE 파이프를 설치하고 종이 절단기를 사용하여 잘라냅니다.
5. PTFE 파이프는 목구멍보다 약 0.5mm 길어야 하며 그렇지 않으면 직접 플러시될 수 있습니다.
6. PTFE 파이프 절단시 내경이 얇아질 수 있으므로 작은 금속 얇은 막대를 사용하여 안쪽으로 돌리십시오.
7. 핫엔드를 역순으로 다시 설치합니다.

-----