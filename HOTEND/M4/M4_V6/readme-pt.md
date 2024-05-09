[M4V6_CAUTION]: https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/M4/M4_V6/M4V6_Precaution.md
[MIXING_COLOE]: https://github.com/ZONESTAR3D/Document-and-User-Guide/tree/master/Mixing_Color
[SLICING_0]: https://github.com/ZONESTAR3D/Slicing-Guide
[SLICING_1]: https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer
[SLICING_2]: https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer#4-slicing-one-color
[SLICING_M4]: https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/PrusaSlicerGuide_M4.md
[FAQ_M4E4]: https://github.com/ZONESTAR3D/Upgrade-kit-guide/blob/main/HOTEND/FAQ_M4E4.md

----
## <a id="choose-language">:globe_with_meridians: Choose language </a>
[![](./lanpic/EN.png)](./readme.md)
[![](./lanpic/ES.png)](./readme-es.md)
[![](./lanpic/PT.png)](./readme-pt.md)
[![](./lanpic/FR.png)](./readme-fr.md)
[![](./lanpic/DE.png)](./readme-de.md)
[![](./lanpic/IT.png)](./readme-it.md)
[![](./lanpic/JP.png)](./readme-jp.md)
[![](./lanpic/KR.png)](./readme-kr.md)
[![](./lanpic/RU.png)](./readme-ru.md)
<!-- [![](./lanpic/SA.png)](./readme-ar.md) -->

## :book: Guia do usuário do Hotend M4V6
O hot end de cores misturadas ZONESTAR 4-IN-1-OUT tem 4 canais de entrada e 1 bico, quatro filamentos são misturados no hot end e depois extrudados através de um bico, portanto, não apenas permite que a impressora imprima a cor original dos filamentos, mas também permite imprimir mais cores ajustando a proporção de mistura do filamento.

### Conteúdo
- **[Atenção](#A0)**
- **[Princípio de funcionamento](#A1)**
- **[Especificações](#A2)**
- **[Componentes do M4V6](#A3)**
- **[Fiação](#A4)**
- **[Estrutura](#A5)**
- **[Dimensões](#A6)**
- **[Instalação e fiação](#A7)**
- **[Carregar/descarregar filamentos](#A8)**
- **[Etapas para imprimir usando hotend M4V6](#A9)**
- **[Guia de fatiamento](#A10)**
- **[Solução de problemas](#A11)**
- **[Apêndice](#A12)**

## <a id="A0">:warning: ATENÇÃO POR FAVOR</a>
### :loudspeaker: Antes de usar o hot end M4V6, leia [:book: Precauções para usar M4V6][M4V6_CAUTION] com atenção.
### :loudspeaker: Deve carregar 4 filamentos no hotend M4V6 simultaneamente, a operação incorreta pode bloquear o hotend de cores misturadas. Se o bloqueio do hot end for causado por operação incorreta, não será coberto pela garantia.
### :loudspeaker: NÃO puxe os "tubos internos de PTFE" para fora do hotend M4V6.
### :loudspeaker: Depois que os filamentos já tiverem entrado no hotend M4V6, NÃO use o menu "Carregar rapidamente" para carregar os filamentos.

### <a id="A1">Princípio de funcionamento</a>
**:warning: antes de usar o M4V6, leia [:book: Introdução à Extrusora de Mistura de Cores][MIXING_COLOE] para entender os princípios de funcionamento da extrusora de mistura de cores.**
######
[](https://github.com/ZONESTAR3D/Document-and-User-Guide/assets/29502731/2b9f4d75-b6fd-486f-aaa7-7a1163383316)

### <a id="A2">Especificações</a>
| Artigo | Parâmetros | Artigo | Parâmetros |
|:--------------------------:|:--------------------------:|:--------------------------:|:--------------------------:|
| Tensão nominal | DC24V/60W Máx. | Diâmetro do bico | Padrão 0,4 mm<sup>1</sup> |
| Canal de entrada | 4 | Modelo de bico | E3D V6 |
| Número de bicos | 1 | Diâmetro do Filamento | 1,75mm |
| Aquecedor | 24V/60W ⌀6x25mm | Sensor de temperatura | Termistor NTC 100K B3950 |
| Ventilador de resfriamento | 4010/5000RPM/24V 0,15A | Ventilador Extrusor | 4010/5000RPM/24V 0,15A |
| Filamentos de suporte | PLA/PLA+/PETG/ABS/ASA etc. | Temperatura de trabalho | 260°C Máximo |
| Comprimento do fio | 1 metro | Dimensões externas | 50x60x75mm |
| Peso líquido | 220g | Peso bruto | 350g |

### <a id="A3">Componentes</a>
![](./2.jpg) ![](./1.jpg)

### <a id="A4">Terminal de fiação</a>
![](./wire.jpg)
:pushpin: Estender o cabo é opcional.

### <a id="A5">Estrutura</a>
![](./3.jpg)

### <a id="A6">Dimensões</a>
![](./size.jpg)

### <a id="A7">Instalação e fiação</a>
A posição de montagem do hot end M4 está em conformidade com o "padrão de montagem de hot end ZONESTAR", que pode ser instalado em quase todas as impressoras 3D ZONESTAR, incluindo séries de produtos P802, M8, D805S, Z8, Z9, Z10 etc.
#### Instalação
Simplesmente remova os 3 parafusos atrás do conjunto hotend e instale o conjunto hotend M4 no suporte X da máquina.     
![](./M4_installation.jpg)
#### Fiação
##### :loudspeaker: ATENÇÃO
- **Atenção para distinguir os terminais 3 e 4**, pois a cor dos terminais é a mesma, mas a cor dos fios é diferente.
Se os fios 3 e 4 estiverem conectados inversamente, você poderá ver que a temperatura do bico exibida na tela LCD será muito mais alta do que a temperatura ambiente depois de ligar a máquina.
- Ao conectar o terminal, **tenha cuidado para não empurrar o terminal metálico da caixa plástica**.
#### :loudspeaker: **Atenção**
- **A ventoinha de resfriamento deve estar ligada** (quando a temperatura do hot end for superior a 60°C), caso contrário o hot end poderá ficar bloqueado ou até mesmo danificado.
  - Por padrão, a **tensão de trabalho** do ventilador e do aquecedor no hot end é **DC 24V**.
#### Siga a definição dos terminais para conectar o hotend à sua placa de controle.
- **Sem cabo de extensão**    
![](./wiring1.jpg)
- **Com cabo extensor**    
![](./wiring2.jpg)
#### Defina o tipo de hot end no LCD MENU: Control>>Configure>>Hotend Type: Mixing    
![](./hotendtype-mix.jpg)  

### <a id="A8">Carregar/Descarregar filamentos</a>
#### :warning: ATENÇÃO POR FAVOR! Você precisa carregar 4 filamentos no hot end, mesmo imprimindo um modelo 3D de uma cor, NÃO deixe nenhum canal vazio antes de imprimir.
#### :warning: ATENÇÃO POR FAVOR! O menu "Carregar rapidamente" só pode ser usado ao carregar o filamento da extrusora para o hot end, uma vez que o filamento entrou no hot end, use o menu "Carregar lentamente" mas não "Carregar rapidamente".
- **Carregue o filamento no hotend:**
###### [![](https://img.youtube.com/vi/-47yB95uIxI/0.jpg)](https://www.youtube.com/watch?v=-47yB95uIxI)
   - Corte a frente do filamento com um alicate diagonal antes de carregá-lo na extrusora e hot end.
   - Carregue 4 filamentos em todas as extrusoras, um por um.
   - Gire a engrenagem das extrusoras para carregar o filamento um por um, não gire cada extrusora mais de 2 voltas por vez, até que todos os filamentos entrem no tubo interno de PTFE da extremidade quente, extrude mais 4 ~ 5 voltas para cada extrusora e Então pare.   
   :warning: Não alimente filamentos no hotend quando qualquer canal do hot end estiver vazio.   
   :warning: Certifique-se de que os filamentos de cada canal alcancem a parte inferior do hot end antes de alimentar o filamento.   
- **Descarregar o filamento do hotend:**
   - Aquecimento do bico (200°C para PLA / 230°C para PETG/ABS).
   - Alimente simultaneamente o filamento pelo menos 10mm em todos os 4 canais.
   - Operar no menu LCD ou girar a engrenagem da extrusora para descarregar os filamentos.

### <a id="A9">Etapas para imprimir usando hotend M4V6</a>
#### Imprimir modelo 3D em uma cor
- **Prepare o arquivo gcode**. Fatiando o modelo 3D usando configurações de impressora 3D de uma cor, consulte [**aqui**][SLICING_2].
- **Carregar filamentos**. Carregue **todos os 4 filamentos** nas extrusoras e, em seguida, alimente os filamentos na parte inferior do hot end M4V6.
- **Imprimir do cartão SD**. Mova o item para **Imprimir** item na tela LCD e clique no botão e escolha o arquivo gcode, clique no botão para iniciar a impressão.
- **Ajuste a altura do bico**. Aguarde o aquecimento do bico e do viveiro e, quando a impressora começar a imprimir a primeira camada, clique duas vezes no botão da tela LCD para ajustar a distância do bico à base e aguarde o término.
#### Imprimir modelo 3D multicolorido
- **Prepare o arquivo gcode**. Fatiando o modelo 3D usando as configurações da impressora 3D multicolorida M4, consulte [**aqui**][SLICING_M4].
- **Carregar filamentos**. Carregue **todos os 4 filamentos** nas extrusoras e, em seguida, alimente os filamentos na parte inferior do hot end M4V6.
- **Imprimir do cartão SD**. Mova o item para **Imprimir** item na tela LCD e clique no botão e escolha o arquivo gcode, clique no botão para iniciar a impressão.
- **Ajuste a altura do bico**. Aguarde o aquecimento do bico e do viveiro e, quando a impressora começar a imprimir a primeira camada, clique duas vezes no botão da tela LCD para ajustar a distância do bico à base e aguarde o término.


### <a id="A10">Fatiamento</a>
Recomendamos o uso do PrusaSlicer para fatiar. Para tutoriais de instalação e uso, consulte o seguinte link:
- **[Instale o software Prusaslicer][SLICING_1]**
- **[Guia de fatiamento para hotend M4][SLICING_M4]**
Para obter mais tutoriais sobre como usar outro software de fatiamento, consulte [:book:este guia][SLICING_0].

### <a id="A11">Soluções de problemas</a>
Se houver algum problema ao usar o hot end M4V6, consulte [**:book: este manual de solução de problemas**](./M4V6_FAQ/readme.md) para encontrar uma solução primeiro.

### <a id="A12">:paperclip: Apêndice</a>
#### :book: Apêndice I: [Obtenha impressão rápida usando hot end M4V6](./HighFlow/readme.md)
Ao imprimir um modelo 3D de uma única cor, o M4V6 pode suportar taxas de fluxo mais altas. Sobre os detalhes, consulte [:book: this guide](./HighFlow/readme.md).

#### :book: Apêndice II: [Como alternar entre hotend E4 e hotend M4][FAQ_M4E4]
