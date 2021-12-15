# 1.10 – Grupos computacionais com o Dynamo

_Neste capítulo, aproveitaremos o poder computacional do_ [_**Dynamo**_](http://dynamobim.org/) _para inserir e modificar grupos flexíveis que estão vinculados a amostras de gráficos do Dynamo prontas para uso._

_Se você não tiver concluído a última seção, faça o download e abra o arquivo_ _**1.10 – Computational Groups with Dynamo.axm**_ _nos_ _**Conjuntos de dados da Parte 1 do Manual do FormIt**._

_Você pode_ [_**aprender mais aqui**_](http://formit.autodesk.com/page/formit-dynamo) _sobre como o FormIt e o Dynamo funcionam juntos para os fluxos de trabalho do projeto computacional._

## **Criar escadas de terraço inferior**

1 – Assegure-se de que as camadas **Lower Terrace, Main Building Floor** e **Plan Image** estejam ativadas, pois é onde adicionaremos as escadas.

2 – Para colocar um grupo de escadas vinculado a uma das amostras do Dynamo prontas para uso:

1. Abra a **Dynamo Palette** na barra de paletas. Você deve ver alguns objetos internos do Dynamo no diretório **Dynamo Samples**.
2. Clique uma vez na amostra do Dynamo **Stairs** para levá-la para o espaço do modelo. O FormIt executará o gráfico em segundo plano e gerará a geometria da escada com base nesse gráfico.
3. Mova o cursor sobre a tela e, quando a escada estiver carregada, uma visualização fantasma da geometria da escada será movida junto com o mouse. Mova o cursor sobre a tela, perto do terraço, e clique para posicionar a escada. Pressione **ESC** para limpar a seleção. Observe que, após posicionar as escadas, a **Properties Palette** será aberta automaticamente.

![](../../.gitbook/assets/0%20%2815%29.png)

_**Observação:**_ [_**Também é possível vincular diretórios locais**_](https://formit.autodesk.com/page/formit-dynamo#dynamo-getting-started) _que contêm gráficos do Dynamo e executar seus próprios gráficos locais do Dynamo como essas amostras._

3 – Para atualizar as cotas de escadas:

1. Com o grupo de escadas selecionado, modifique as entradas disponíveis na seção **INPUTS** do Dynamo na parte inferior da **Properties Palette** para coincidir com o mostrado abaixo. A maioria dos grupos criados por meio de scripts do Dynamo terá uma seção do Dynamo incluída em suas propriedades quando selecionada.
   * Add Top Landing = False
   * Add Middle Landing = False
   * Add Bottom Landing = False
   * Floor-to-Floor Height = 2,6
   * Stair Width = 12
   * Riser Height = 0.6
   * Tread Length = 1.25
   * Tread Overlap = 0.25
   * Tread Thickness = 0.25
   * Height Between Middle Landings = \(não relevante, pois nenhum patamar do meio está sendo criado\)
   * Middle Landing Length = \(não relevante, pois nenhum patamar do meio está sendo criado\)
   * Top/Bottom Landing Length = \(não relevante, pois nenhum patamar está sendo criado\)
2. Clique no botão **Run** para executar novamente o script do Dynamo usando os valores de entrada atualizados.
3. Mova o grupo conforme necessário para colocar a escada na localização correta de acordo com a **Plan Image**. Tome cuidado para não alterar a elevação do grupo de escadas ao movê-la. Consulte os capítulos anteriores para saber mais sobre truques e técnicas ao mover elementos do modelo.

![](../../.gitbook/assets/1%20%2811%29.png)

_**‌Observação:**_ _A entrada_ _**Floor-to-Floor Height**_ _é uma aproximação da altura total da escada. A_ _**Riser Height**_ _é o parâmetro que realmente define a altura das escadas. Neste exemplo, definimos a __**Floor-to-Floor Height**__ como 2,6’, mas a altura final da escada é 3,0’ \(0,6’\(**Riser Height**\) x 5 \(número de espelhos\)\). Como o vão entre o chão e a parte superior do piso do terraço é de 3’-2", o restante valor de 2" está contido no espelho do degrau superior._

## **Criar escadas de construção principais**

_Nas etapas anteriores, criamos uma escada sem patamares. Agora, criaremos uma escada que usa um patamar superior que se alinha com o_ _**Main Building Floor**._

1 – Comece fazendo uma cópia das escadas que acabamos de fazer:

1. Selecione a escada existente e, em seguida, clique em qualquer lugar na **Plan Image** para iniciar um comando de deslocamento. Isso fará com que o FormIt use a elevação da **Plan Image** como a altura de referência inicial para posicionar nossa nova cópia. Pressione **Ctrl** para criar uma **cópia rápida**.
2. Mova o cursor sobre o edifício principal acima do terraço. Observe que agora a face superior do terraço é o novo plano de referência. Clique para colocar o grupo.

![](../../.gitbook/assets/2%20%289%29.png)

_**Observação:**_ _Como a_ _**Plan Image**_ _está no plano do_ _**Ground Level**_ _, a_ _**Move Tool**_ _usará esse plano como referência para seu ponto inicial. Observe a dica de ferramenta_ _**On Face**_ _na imagem acima, indicando que a face da imagem da planta está selecionada como a referência inicial e a face superior do_ _**Lower Terrace Floor**_ _está selecionada como a referência final._

2 – Use a ferramenta **Make Unique \(MU\)** para que quando alterarmos as entradas do Dynamo dessa escada, ela não afete a escada inferior. Reposicione o grupo conforme necessário para que ele fique próximo de sua localização final. Vamos ajustar isso mais tarde. É possível alternar a visibilidade da camada **Lower Terrace** para ver a planta abaixo para ajudar a posicioná-la, mas, novamente, tenha cuidado para não alterar a elevação da nova escada ao movê-la.

3 – Na **Properties Palette**, atualize as **Dynamo Inputs** como mostrado abaixo e execute o script mais uma vez.

* Add Top Landing = True
* Floor-to-Floor Height = 2,333
* Riser Height = 0,466
* Tread Length = 1,5
* Top/Bottom Landing Length = 2,5

![](../../.gitbook/assets/3%20%281%29.jpeg)

_**Observação:**_ _Se você tiver definido_ _**Add Bottom Landing**_ _como_ _**true**_ _e executar novamente o script, a face superior do patamar inferior deverá se alinhar com a face superior do_ _**Lower Terrace Floor**. Isso está acontecendo porque – diferentemente das escadas anteriores – ajustamos a_ _**Riser Height**_ _para fazer corresponder a_ _**Floor-to-Floor Height**_ _à altura real que desejamos \(2’-4" ou 2,333’\)._

2 – Reposicione o grupo novamente em sua posição final. O patamar superior deve estar alinhado com o **Main Building Floor**.

3 – Para finalizar as escadas, adicione o material **Stone - Travertine** para coincidir com os pisos. Para saber mais sobre como aplicar materiais, consulte os capítulos anteriores.

