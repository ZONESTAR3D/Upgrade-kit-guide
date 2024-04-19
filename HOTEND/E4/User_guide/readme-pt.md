[PRUSA]: https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/PrusaSlicer#6-slicing-muti-color-for-e4-hotend
[CURA]: https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/cura
[S3D]: https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/Simplify3D#slicing-video-toturial-for-z9v5-with-e4-hotend
[ENDGCODE]: https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/Custom_Gcode.md#end-g-code
[STARTGCODE]: https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/Custom_Gcode.md#start-gcode
[FIRMWARE]: https://github.com/ZONESTAR3D/Firmware

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
## Manual do usuário do hotend E4
ZONESTAR 4-IN-1-OUT **Cor sem mistura** hot end (referido como **E4 Hot end**) tem 4 canais de entrada e 1 bocal, ao mudar de cor, o filamento de cor anterior precisa ser descarregado ( puxado para fora) da extremidade quente e, em seguida, carregue o próximo filamento de cor.

### <a id="A1"> 1. Especificações </a>
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

### <a id="A2"> 2. Componentes </a>
O conjunto hot end E4 inclui as seguintes peças/acessórios:
![](./E4-2.jpg)
>
     1. Ventilador de resfriamento 2. Carcaça 3. Orifício de instalação do sensor de nivelamento da cama 4. Parafusos montados
     5. Ventilador da extrusora 6. Impressões de "pato" do ventilador 7. Bloco de aquecimento 8. Dissipador de calor
     9. Bico 10. Aquecedor do cartucho 11.Sensor de temperatura 12. Garganta
     13. Luva de silicone 14. Conexões (conectores pneumáticos) 15. Cabo

### <a id="A3"> 3. Fio </a>
![](./E4-3.jpg)

### <a id="A4"> 4. Instalação e fiação </a>
A posição de montagem do hot end E4 está em conformidade com o "padrão de montagem de hot end ZONESTAR", que pode ser instalado em quase todas as impressoras 3D ZONESTAR, incluindo as séries de produtos P802, M8, D805S, Z8, Z9, Z10 etc.
#### 4.1 Instalação
Simplesmente remova os 3 parafusos atrás do conjunto hotend e instale o conjunto hotend E4 no transportador X da máquina.
![](./E4-4.jpg)
#### 4.2 Fiação
##### :loudspeaker: **Atenção**
- **Atenção para distinguir os terminais 3 e 4**, pois a cor dos terminais é a mesma, mas a cor dos fios é diferente.
Se os fios 3 e 4 estiverem conectados inversamente, você poderá ver que a temperatura do bico exibida na tela LCD será muito mais alta do que a temperatura ambiente depois de ligar a máquina.
- Ao conectar o terminal, **tenha cuidado para não empurrar o terminal metálico da caixa plástica**.
##### :loudspeaker: **Atenção**
- **A ventoinha de resfriamento deve estar ligada** (quando a temperatura do hot end for superior a 60°C), caso contrário o hot end poderá ficar bloqueado ou até mesmo danificado.
  - Por padrão, a **tensão de trabalho** do ventilador e do aquecedor no hot end é **DC 24V**.
#### Siga a definição dos terminais para conectar o hotend à sua placa de controle.
- **Sem cabo de extensão**
![](./fiação1.jpg)
- **Com cabo extensor**
![](./wiring2.jpg)
#### 4.3 Definir tipo de hot end no LCD MENU: Controle >> Configurar >> Tipo de Hotend: Sem mistura
- :warning: Se a sua impressora não possui uma tela TFT-LCD de 4,3", ignore esta etapa.
- :warning: se você não conseguir ver o menu na tela LCD da sua impressora, atualize para a versão mais recente. [:link: **Link para download de firmware**][FIRMWARE]
##### ![](./hotendtype-nonmix.jpg)

### <a id="A5"> 5. Princípio de funcionamento </a>
O hot end E4 (4-IN-1-OUT Non-Mix Color) é composto de dissipador de calor, coletor de funil, bloco de aquecimento, bico, etc. Durante a impressão, apenas um filamento pode ser carregado no hot end. Ao mudar para outro filamento de cor, a extrusora puxa o filamento de cor anterior para fora do hot end E4 e, em seguida, carrega outro filamento no hot end E4. A imagem a seguir (da esquerda para a direita) demonstra brevemente esse processo.
##### ![](./E4-5.jpg)
#### Você também pode consultar uma animação para entender bem o princípio de funcionamento do hot end E4.
![](./E4_principle.gif).
##### :book: Sobre "Torre de limpeza"
Como ainda existem filamentos derretidos da cor anterior no bocal após o carregamento de um novo filamento de cor, precisamos “limpar” o bocal antes de começar a imprimir o novo filamento de cor. Caso contrário, a parte inicial impressa será a cor anterior, mas não a nova cor como esperamos. A solução é adicionar **"wipe tower"** depois de mudar para uma nova extrusora no software de fatiamento.
Sobre detalhes, consulte [**:point_right: Fatiar**](#A9).
:bulb: A torre Wipe é chamada de "Torre Prime" no Cura Slicer e "Prime Pillar" no Simplify3d Slicer.

### <a id="A6"> 6. Dimensões </a>
![](./E4_size.jpg)

### <a id="A7"> 7. Pré-carregar filamentos </a>
#### 7.1 Para impressão em uma cor
[![](https://img.youtube.com/vi/6aTF5QnFhi4/0.jpg)](https://www.youtube.com/watch?v=6aTF5QnFhi4)
#### 7.2 Para impressão multicolorida
[![](https://img.youtube.com/vi/FyHrAMytlT8/0.jpg)](https://www.youtube.com/watch?v=FyHrAMytlT8)
Antes de imprimir, pré-carregue os filamentos na posição apropriada da extremidade quente para que a extrusora possa carregar suavemente os filamentos para dentro e para fora da extremidade quente.
- **Etapa 1:** Carregue os filamentos da extrusora e deixe-os se estenderem cerca de 10 mm para fora dos tubos de PTFE.
- **Etapa 2:** Conecte os tubos de PTFE (com filamentos) no HOTEND.
     - :pushpin: **Se houver um filamento na extremidade quente, aqueça e noozle e depois puxe-o para fora primeiro. Consulte [Descarregar filamentos](#A8) para fazer isso.**
     - :pushpin: Cortar a frente dos filamentos em um formato afiado antes de carregar o filamento.
     - :pushpin: Se a extrusora não foi usada durante a impressão, não é necessário carregar o filamento no hot end.
     ![](./E4-6.jpg)
     - :pushpin: Adicione alguns gcodes no **"Iniciar gcode"** ([:point_right: View][STARTGCODE]) do software de fatiamento para imprimir.
     ![](./Preload_line.jpg)
     - :pushpin: Adicione alguns gcodes no **"End gcode"** ([:point_right: View][ENDGCODE]) do software de fatiamento para retirar o último filamento impresso do hotend.

### <a id="A8"> 8. Descarregue os filamentos </a>
Siga as etapas abaixo para descarregar o filamento do hotend:
- **Etapa 1:** Aquecimento do bico (190 graus para PLA e 230 graus para ABS).
- **Etapa 2:** Gire a engrenagem da extrusora para descarregar o filamento.
:star2: Algumas impressoras 3D (por exemplo, Z9V5Pro) possuem um menu “Filament” na tela LCD, opere a tela LCD e use o menu ***“Prepare>>Filament”*** para pré-aquecer o bico, escolha a extrusora e descarregar filamentos.

### <a id="A9"> 9. Fatiar </a>
Guia do usuário (tutorial em vídeo) do software de fatiamento PrusaSlicer/Cura/Simplify3d.
- **:+1: PrusaSlicer**, consulte :point_right: [**aqui**][PRUSA].
- **Cura slicer**, consulte :point_right: [**aqui**][CURA].
- **Simplify3d Slicer**, consulte :point_right: [**aqui**][S3D].

### <a id="A10"> 10. Testando gcode </a>
Carregamos alguns arquivos de teste em nossa página do Github, você pode baixá-los em [**aqui**](../example/readme.md).

### <a id="A11"> 11. Solução de problemas </a>
Se você encontrar problemas ao usar o hot end E4, consulte primeiro o [**guia de solução de problemas**](../FAQ/readme.md) para encontrar uma solução. Se o problema ainda não puder ser resolvido, entre em contato com nosso engenheiro de suporte técnico por email: :email: support@zonestar3d.com.

----
### Link de venda
[:gift: **ZONESTAR Offical Store**](https://bit.ly/39qDtKp)     
[:gift: **Aliexpress**](https://www.aliexpress.com/item/1005002951777699.html)

----