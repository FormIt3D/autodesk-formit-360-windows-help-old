# 1.11 – Importar modelos com a biblioteca de conteúdo

_Neste capítulo, vamos importar modelos existentes do SketchUp, além de usar a Biblioteca de conteúdo do FormIt para inserir famílias prontas para uso que foram convertidas do Revit. Observe que, ao abrir arquivos SKP com o FormIt, eles apresentam as seguintes categorias intactas: Materiais, Grupos e componentes, Camadas \(Identificadores\) e Cenas. Pode ser necessário fazer alguma limpeza para manter os projetos organizados e arrumados._

_Para este capítulo, vamos usar arquivos da pasta_ **Conjunto de dados de Farnsworth House > Arquivos de suporte**. Se você ainda não tiver os arquivos, faça o download das pastas necessárias ou de todo o conjunto de dados, nos _**Conjuntos de dados da Parte 1 do Manual do FormIt**._

## **Importar e editar arquivos SKP**

_Primeiro, vamos analisar o processo de adicionar um item de conteúdo transferido por download à sua própria biblioteca de conteúdo pessoal_. Observe que neste exercício usaremos somente arquivos SKP. Para saber mais sobre como abrir/importar outros formatos de arquivo, consulte [**esta postagem do blog sobre os recursos do Formit 2021.2**](https://formit.autodesk.com/blog/post/formit-2021-2-and-new-revit-add-in-now-available) e **este capítulo sobre** **Formatos de arquivos de importação e exportação expandidos**.

1 – Certifique-se de **Salvar \(Ctrl + S\)** todos os trabalhos abertos e, em seguida, inicie um novo esboço do FormIt. Para isso, é possível:

1. Abrir outra sessão no FormIt em uma nova janela clicando com o botão direito do mouse no ícone do FormIt, na **barra de tarefas do Windows**, e clicando no ícone do **FormIt**. Isso vai abrir uma nova janela do FormIt, permitindo que você execute duas sessões do FormIt lado a lado.
2. OU, após salvar, iniciar um **Novo esboço \(Ctrl + N\)** no menu suspenso **Arquivo**, na barra do **Menu principal**.

![](../../.gitbook/assets/0%20%2819%29.png)

2 – Crie uma nova pasta denominada **Conteúdo personalizado do FormIt** dentro da pasta **Conjunto de dados da Farnsworth House &gt; Arquivos de suporte &gt; FormIt**, no _**Conjunto de dados da Farnsworth House**._

3 – **Salve \(Ctrl + S\)** o novo esboço nessa pasta. Recomendamos nomeá-lo como: **Ottoman – Barcelona\_Mies.axm**

4 – No novo arquivo vazio do FormIt:

1. **Importe um arquivo local \(Ctrl + I\)** selecionando **Importar &gt; Localmente...** no menu suspenso **Arquivo** na barra do **Menu Principal**.
2. Selecione o arquivo **Ottoman – Barcelona\_Mies.skp** no **Conjunto de dados da Farnsworth House &gt; Arquivos de suporte &gt; SketchUp** e clique em **Abrir**.

_**Observação:**_ _Se você não encontrar o arquivo_ _**Ottoman – Barcelona\_Mise.skp**, verifique se o menu suspenso de formato de arquivos, na parte inferior direita, está definido como_ _**Todos os formatos suportados**._

![](../../.gitbook/assets/1%20%287%29.png)

5 –Renomeie o grupo importado como **Otomana – Barcelona\_Mies**.

6 – Quando importarmos esse modelo para o nosso arquivo da Farnsworth House, ele será posicionado usando o ponto de **origem** desse arquivo. Para controlar o ponto de posicionamento l, vamos mover o grupo **Otomana – Barcelona\_Mies** para que um de seus cantos esteja localizado no ponto de **origem**. Para isso:

1. Assegure-se de que a opção **Snap à grade \(SG\)** esteja ativada. Desenhe uma **Linha \(L\)** de referência, começando no ponto de **origem** \(onde os eixos X, Y e Z efetuam uma interseção\). Clique em qualquer lugar para inserir o segundo ponto.
2. Selecione o grupo otomana e inicie o comando para mover clicando uma vez no canto inferior esquerdo da perna, conforme mostrado. _Para saber mais sobre como mover objetos, consulte os capítulos anteriores._
3. Mova o grupo para o ponto de **origem**, efetuando o snap para o ponto inicial da linha de referência que acabamos de desenhar.
4. Exclua a linha de referência.

![](../../.gitbook/assets/2%20%2817%29.png)

7 – Recomendamos excluir todas as camadas indesejadas que foram importadas com o arquivo SKP, já que quaisquer camadas que esse modelo apresente serão importadas para o nosso modelo da Farnsworth House. Para fazer isso, vá para a **paleta Camadas**, selecione **Camada 0** e clique no botão **-**. Isso vai excluir a camada e, ao mesmo tempo, manter sua geometria.

![](../../.gitbook/assets/3%20%2816%29.png)

_**Observação:**_ _Sempre que você exclui uma camada, qualquer geometria ou grupos que estavam nessa camada são atribuídos para a classificação de_ _**Sem camada**, que é o valor padrão para qualquer objeto que ainda não tenha sido atribuído a uma camada._

## **Criar a miniatura de conteúdo**

_Nesta próxima etapa, será configurada uma cena a ser usada como a miniatura de_ _**conteúdo**_ _, que será exibida na_ _**paleta Biblioteca de conteúdo**._

1 – Para definir as configurações de vista para a cena em miniatura:

1. Na guia **Ambiente** da **paleta Estilos visuais**, desmarque todas as caixas de seleção e defina a cor de **Inferior/ Plano de fundo** como branca.
2. Certifique-se de que o modo de vista esteja definido como **Perspectiva** \(VP\)**.**
3. Use as **ferramentas de navegação de vistas** para aumentar o zoom de uma localização de câmera que represente bem o objeto, de forma semelhante à imagem abaixo.

![](../../.gitbook/assets/4%20%2813%29.png)

2 – Para salvar as configurações que você acabou de definir, crie uma cena:

1. Vá para a **paleta Cenas**.
2. Clique no botão **+**. Isso criará uma nova cena com base nas configurações atuais.
3. Renomeie-a como **Miniatura** e assegure-se de que pelo menos as primeiras quatro \(4\) caixas de seleção estejam marcadas: **Câmera**, **Camadas**, **Sol e sombras** e **Estilos visuais**. O restante das configurações de cena não é realmente relevante para a criação da imagem em miniatura.
4. Use o botão **Atualizar cena** sempre que desejar atualizar a **Cena** para efetuar a correspondência entre a vista da câmera atual e as configurações visuais.

![](../../.gitbook/assets/5%20%2811%29.png)

3 – **Salve \(Ctrl + S\)** novamente o modelo concluído da otomana. Observe que a **Miniatura de conteúdo** é criada com base na vista atual quando o modelo foi salvo pela última vez; portanto, assegure-se de que você esteja na **Cena em miniatura** antes de salvar.

_Se desejar, será possível comparar o arquivo com o nosso abrindo o arquivo __**Ottoman – Barcelona\_Mies.axm**__ salvo no __**Conjunto de dados da Farnsworth House &gt; Arquivos de suporte &gt; FormIt &gt; Mobiliário** __, no_ _**Conjunto de dados da Farnsworth House**.‌_

_Você pode seguir as mesmas etapas indicadas acima com os arquivos SKP de banco e cadeira, localizados na mesma pasta da otomana._

_**Dica:**_ _Para acelerar o processo, recomendamos usar o arquivo_ _**Ottoman – Barcelona\_Mies.axm**_ _que você acabou de criar como um modelo. Durante a modelagem, você pode desejar ativar a_ _**Grade**_ _e os_ _**Eixos**_ _novamente na_ _**paleta Estilos visuais**. Ao ajustar somente a posição da câmera da_ _**Cena em miniatura**_ _para cada peça de mobiliário, você garante que as_ _**Miniaturas de conteúdo**_ _permaneçam consistentes para todos os modelos de conteúdo._

## **Vincular uma biblioteca de conteúdo**

_Agora, vamos voltar ao projeto da Farnsworth House. Vamos aprender como vincular a pasta **FormIt** ao **Conjunto de dados da Farnsworth House**, para acessar facilmente todos os arquivos, incluindo o_ **Conteúdo personalizado do FormIt** _que acabamos de criar em nosso projeto._

1 – Após voltar ou reabrir o modelo da Farnsworth House. _Se você não concluiu o último capítulo, faça download e abra o arquivo_ _**1.11 – Import Models with Content Library.axm**_ _do_ _**Conjunto de dados da Farnsworth House**._

1. Abra a **paleta Biblioteca de conteúdo** e clique no ícone **Vincular diretório da biblioteca de conteúdo**. A janela **Preferências** será exibida com a guia **Biblioteca de conteúdo** aberta.
2. Clique no ícone **+** para **Adicionar uma nova localização da biblioteca de conteúdo**. Uma terceira janela será exibida para navegar no diretório do computador e selecionar uma pasta.
3. No _**Conjunto de dados da Farnsworth House**, navegue pelas pastas:_ _**Arquivos de suporte > FormIt**. Você encontrará as_ pastas com os arquivos **.axm** que criamos anteriormente neste capítulo. Clique duas vezes na pasta **FormIt** para selecioná-la.
4. Clique em **Selecionar pasta** e o caminho dessa pasta será exibido no painel **Localizações da biblioteca – Local**.
5. De volta à janela **Preferências**, clique em **OK** e a pasta vinculada será adicionada à **Biblioteca de conteúdo**.
6. Para acessar essa nova biblioteca, abra o menu suspenso na parte superior da **paleta Biblioteca de conteúdo** e selecione **FormIt**.
7. Observe que a estrutura das pastas e todos os arquivos **.axm** na pasta vinculada serão exibidos na **paleta Biblioteca de conteúdo**. Clique duas vezes em qualquer subpasta para acessar os arquivos contidos nela.

![](../../.gitbook/assets/link-library-content.png)

**Observação:** Se você tiver acesso ao **Autodesk Docs** \(anteriormente conhecido como Autodesk 360\), também poderá acessar os arquivos que foram armazenados lá por meio do menu suspenso **Biblioteca de conteúdo**.

## **Inserir conteúdo da biblioteca**

_‌Agora, vamos inserir os itens de conteúdo que criamos no modelo Farnsworth._

1 – Para que possamos ver dentro da casa para colocar o mobiliário, desative a camada **Telhado** e use a **Órbita \(O\)** para girar a vista em perspectiva até que seja possível ver todo o piso do edifício principal.

2 – De volta à **paleta Biblioteca de conteúdo**, verifique se o menu suspenso ainda está definido como **FormIt**. Antes de colocar qualquer um dos móveis que acabamos de criar, precisamos incluir o “núcleo” da casa:

1. Clique na pasta **Outro** para abri-la e, em seguida, clique na miniatura **Farnsworth House – Núcleo** para selecioná-la.
2. Passe o cursor do mouse sobre o **Piso do edifício principal** para clicar no **Centroide** do piso e colocar o **Núcleo**.
3. Para voltar à pasta FormIt, use o botão **Navegar para cima**.

![](../../.gitbook/assets/7%20%282%29.jpeg)

3 – Defina a câmera como **Ortogonal \(VO\)** **Vista superior \(VT\)** e ative a opção **Piso do edifício principal** para ver a **Imagem da planta**. Consulte os capítulos anteriores para saber mais sobre as configurações de **Vistas** e **Camadas**.

4 – Selecione a opção **Farnsworth House – Núcleo** e mova-a até que ela se alinhe estreitamente com a imagem da planta.

![](../../.gitbook/assets/8%20%281%29.png)

_**Observação:**_ _Ao mover o_ _**Núcleo**, tenha cuidado para não alterar sua elevação. É possível usar a tecla_ _**Shift**_ _para restringir o movimento de modo a que esteja sempre ao longo de um dos eixos ou assegurar que os pontos de referência inicial e final do comando_ _**Mover \(M\)**_ _estejam na mesma altura, clicando somente na_ _**Imagem da planta**e não no_ _**Núcleo**_ _. Consulte os capítulos anteriores para saber mais sobre a ferramenta_ _**Mover \(M\)**_ _.‌_

## **Inserir mobiliário da biblioteca**

1 – Com base em um processo semelhante, agora é possível inserir o mobiliário criado anteriormente neste capítulo, da pasta **Conteúdo personalizado do FormIt**. Se você não tiver convertido todos os três \(3\) arquivos SKP, será possível usar as versões predefinidas da pasta **Mobiliário**.

_**Observações:**_

* _Ative novamente a camada_ _**Piso do edifício principal**_ _, para que você possa colocar o mobiliário diretamente na superfície do_ _**Piso do edifício principal**._
* _Ao inserir um novo objeto, use a tecla __**Tab**__ para alternar entre os planos de posicionamento._
* _Ao inserir um novo objeto, use a tecla __**barra de espaço**__ para rotacioná-lo em 90 intervalos antes de inserir._

![](../../.gitbook/assets/9%20%283%29.png)

2 – De forma similar, explore as **Amostras da biblioteca de conteúdo** para inserir conteúdo pronto para uso. Observe que vários desses itens apresentam diferentes tamanhos para escolher, de modo semelhante aos tipos de famílias no Revit.

![](../../.gitbook/assets/10%20%286%29.png)

## **Usar a ferramenta Escala**

1 – Com as técnicas que você acabou de aprender, insira uma instância do componente **pinheiro** da pasta **Conjunto de dados da Farnsworth House &gt; FormIt &gt; Vegetação**.

1. Uma vez inserido o componente, selecione o grupo e renomeie-o como **Árvore**. Clique com o botão direito do mouse para acessar o **Menu de contexto** e selecione **Escala não uniforme \(NU\)**.
2. Clique em um dos **botões de Escala não uniforme** para redimensionar e alterar as proporções do grupo **Árvore**, conforme desejado.

![](../../.gitbook/assets/11%20%283%29.png)

![](../../.gitbook/assets/12%20%282%29.png)

_**Observação:**_ _De modo similar, a ferramenta_ _**Escala \(SC\)**_ _pode ser usada para redimensionar um grupo ou modelo inteiro de forma uniforme._

2 – Copie esse grupo e coloque várias árvores em torno da casa, usando as **ferramentas de escala** para criar uma variedade de tamanhos e proporções.

![](../../.gitbook/assets/13%20%286%29.png)

_**Observação:**_ _Embora as árvores sejam todas instâncias do mesmo grupo, conseguimos_ _**dimensioná-las**_ _em diferentes tamanhos. Se usar_ _**Escala \(SC\)**_ _e_ _**Escala não uniforme \(NU\)**_ _fora do modo de edição de grupo, será possível modificar as instâncias individuais do mesmo grupo. Se editarmos um dos grupos de_ _**Árvores**_ _e modificarmos sua geometria ou seu material, todas as instâncias do grupo serão atualizadas, mas cada uma manterá sua escala personalizada atual. Experimente._

### **Manter o modelo organizado**

_Lembre-se de sempre classificar o conteúdo adicionado em camadas. Neste exemplo, recomendamos colocar o núcleo e todo o mobiliário na camada_ _**Piso do edifício principal**_ _e as árvores em uma nova camada denominada_ _**Vegetação**._

