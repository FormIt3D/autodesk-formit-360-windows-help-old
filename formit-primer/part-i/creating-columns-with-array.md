# 1.8 – Criar colunas com matriz

_Neste exercício, vamos desenhar um elemento detalhado – uma coluna de viga em I. Em seguida, usaremos a ferramenta Matriz para criar rapidamente várias cópias uniformemente espaçadas._

_Se você não tiver concluído a última seção, faça o download e abra o arquivo_ _**1.8 – Create Columns with Array.axm**_ _nos_ _**Conjuntos de dados da Parte 1 do Manual do FormIt**._

## **Desenhar o perfil da coluna**

1 – Para facilitar o processo de desenho:

1. Acesse **Vista superior \(VT\)**.
2. Alterne o modo de visualização para **Ortográfico \(VO\)**.
3. Desative as camadas **Prédio principal** **Piso** e **Telhado**. Essa etapa impedirá que a nova geometria efetue o snap à geometria existente nessas camadas.
4. Aplique zoom no canto superior esquerdo da imagem da **planta de piso importada** para que você possa visualizar a coluna em detalhes.
5. Desative o recurso **Snap à grade \(SG\)** \(se estiver ativado\). Isso vai ajudar a desenhar as linhas de detalhe.

![](../../.gitbook/assets/0%20%2813%29.png)

_Para desenhar a coluna, primeiro vamos desenhar uma metade e, em seguida, espelhá-la para criar rapidamente a outra metade simétrica._

2 – Para criar a primeira metade da viga em I, use a **ferramenta Linha \(L\)** para fazer o seguinte esboço usando as cotas especificadas. Não se preocupe ainda com a posição exata da coluna na imagem da planta.

![](../../.gitbook/assets/1%20%2818%29.png)

3 – Para espelhar a forma que você acabou de desenhar:

1. Clique duas vezes para selecionar todas as faces e arestas da geometria desenhada.
2. Clique com o botão direito do mouse e selecione a **ferramenta Espelhar \(MI\)**.
3. Clique na alça laranja central do **Widget de espelho** e coloque-a no canto inferior esquerdo da geometria.
4. Use a seta inferior do botão de seta dupla no Widget para rotacionar o eixo de espelhamento em 90 graus \(sentido horário\).
5. Clique uma vez no espaço ou pressione **Esc** para concluir o processo de espelhamento. O resultado deve ser semelhante a um perfil de viga em I com uma linha no meio. Pressione novamente **ESC** para limpar a seleção.

![](../../.gitbook/assets/2%20%285%29.png)

![](../../.gitbook/assets/3%20%287%29.png)

_**Observação**: A orientação e a localização da geometria final são visualizadas com a forma azul fantasma enquanto você estiver ajustando o widget de espelho. É possível usar essa visualização como uma referência para espelhar a geometria para a localização desejada._

4 – Para unir ambos os lados em uma única geometria, remova a linha divisória clicando nela para selecioná-la e, em seguida, pressione **Excluir**. Agora, as duas superfícies estão unidas em uma única superfície.

5 – Para mover a geometria para sua posição final:

1. Se estiverem desativadas, ative as camadas **Imagem da planta** e **Telhado** para usá-las como guia.
2. Clique duas vezes no perfil da coluna para selecionar sua face e todas as suas linhas. Comece a mover a seleção ao longo do eixo verde \(**Eixo Y**\). Mantenha pressionada a tecla **Shift** e mova o perfil até que ele se alinhe com o telhado e, em seguida, clique para posicioná-lo.
3. De forma semelhante à etapa anterior, mova a geometria novamente, desta vez bloqueando-a no eixo vermelho \(**Eixo X**\).
4. Clique para posicioná-la na parte superior da viga em I desenhada na **Imagem da planta**. É suficiente ficar próximo da posição desejada, como na imagem a seguir, a posição horizontal não precisa ser perfeita.

_**Observação:**_ _A tecla_ _**Shift**_ _bloqueará a geometria para que o movimento aconteça ao longo de apenas um eixo. Neste caso, o verde \(**Eixo Y**\). Isso vai garantir que o perfil da coluna não se mova acidentalmente para cima e se alinhe com a parte superior do plano do telhado._

![](../../.gitbook/assets/4%20%289%29.png)

## **Extrusão e matriz da coluna**

1 – Para facilitar o próximo processo de desenho, alterne o modo de vista de volta para **Perspectiva \(VP\)** e use a **Órbita \(O\)** para posicionar a câmera de forma a visualizar o perfil da viga em I da perspectiva noroeste. Use a seta de norte no canto inferior esquerdo para ajudar a posicionar a vista.

![](../../.gitbook/assets/5%20%281%29.jpeg)

_**Observação:**_ _Para saber como navegar pelo esboço, recomendamos consultar o capítulo_ _**Navegar na cena**_ _._

2 – Selecione a face do perfil da coluna e faça a extrusão da face para cima em **17’-8"**.

_**Observação:**_ _Se, ao mover o perfil da coluna, ele se alinhar com o telhado, faça a extrusão da face para baixo em_ _**17’-8"**  , em vez de para cima._

3 – Diminua o zoom e ative a camada **Telhado** \(se estiver desativada\). A parte superior da coluna deve se alinhar com a parte superior do telhado.

![](../../.gitbook/assets/6%20%289%29.png)

4 – Para manter o modelo organizado e arrumado, selecione a geometria da coluna novamente e faça o seguinte:

1. **Agrupe \(G\)** e nomeie-a como **Altura da coluna**.
2. Crie uma nova **Camada** chamada **Coluna** e adicione o grupo à camada.
3. Importe o material **Metal – Escovado – Colorido** e pinte o grupo com ele.

![](../../.gitbook/assets/7%20%284%29.png)

_**Observação:**_ _Consulte os capítulos anteriores para obter mais informações sobre_ _**Grupos**,_ _**Camadas**e_ _**Materiais**._

4 – Clique em **Esc** para limpar a ferramenta de pincel.

## **Matriz de colunas**

1 – Vá para a **Vista superior \(VT\)** e alterne novamente o modo de câmera para **Ortogonal \(VO\)**.

2 – Desative a camada **Telhado**.

3 – Para iniciar o processo de matriz:

1. Clique uma vez para selecionar o grupo de colunas. Clique com o botão direito do mouse para abrir o **Menu de contexto** e selecione **Matriz \(AR\)**.
2. Na caixa de diálogo **Propriedades da matriz**, use as seguintes configurações:
   * **Comprimento entre cópias**
   * **Linear** \(padrão\)
   * **Agrupar cada sólido e, em seguida, a matriz** \(padrão\)
   * **Número de cópias: 3**
   * Clique em **OK** para fechar a caixa de diálogo.

![](../../.gitbook/assets/8%20%283%29.png)

4 – Para posicionar os novos elementos:

1. Clique uma vez na coluna para iniciar a **Matriz**. Mova o cursor ao longo do eixo vermelho \(**Eixo X**\).
2. Defina a cota como **22'**. Agora, existem **quatro** colunas a uma distância de **22'**.
3. Pressione **Esc** para limpar a seleção.

![](../../.gitbook/assets/9%20%286%29.png)

5 – Para selecionar todos os grupos da **Coluna Altura** de uma vez, passe o cursor do mouse sobre um deles e pressione a tecla **Tab** uma única vez. Observe que todas as caixas delimitadoras das quatro colunas foram realçadas. Clique uma vez na coluna sobre a qual está o cursor do mouse e todas serão selecionadas. Essa é uma forma rápida de selecionar todas as instâncias do mesmo grupo de uma só vez.

6 – Execute outra **Matriz \(AR\)** para criar as colunas no outro lado do edifício. Desta vez, faça uma cópia ao longo do eixo verde em todo o edifício. Defina a cota como **29'- 4 5/8".**

_**Observação:**_ _29’ 4 5/8" = 8 5/8" \(profundidade da coluna\) + 28’-8" \(largura do edifício principal\)._

7 – Para visualizar todo o edifício, vá para a opção **Vista 3D \(V3\)** e defina-a como **Perspectiva \(VP\)**. Se estiverem desativadas, ative as camadas **Piso do edifício principal**, **Telhado**, **Terraço inferior** e **Coluna**.

![](../../.gitbook/assets/10%20%287%29.png)

## **Criar as colunas do terraço**

_Agora, vamos duplicar as colunas do edifício principal para criar versões semelhantes, mas menores, para o terraço._

1 – Para facilitar o desenho, recomendamos voltar para uma configuração **Ortogonal \(OV\)** e com **Vista superior \(VT\)**.

2 – Para criar as novas colunas:

1. Mantenha pressionada a tecla **Ctrl** ou **Shift**, clique nas três colunas mais próximas do **Piso do terraço inferior** para selecioná-las.
2. Clique uma vez em qualquer uma das colunas para começar a mover todas as três colunas selecionadas de uma só vez. Pressione a tecla **Ctrl** uma vez para criar uma **cópia rápida**. Uma visualização fantasma da cópia será exibida.
3. Mova as cópias para baixo ao longo do eixo verde \(**Eixo Y**\) por **23’-4 3/8**". Pressione **Esc**.
4. Sem desmarcar, mova as colunas copiadas ao longo do eixo vermelho \(**Eixo X**\) por **22’** para colocá-las em sua posição final.
5. Novamente, com as três novas colunas ainda selecionadas, clique com o botão direito do mouse em uma das colunas copiadas e selecione **Tornar único \(MU\)**. Agora, essas colunas estão associadas entre si, mas são exclusivas dos originais.

_**Observação:**_ _Ao manter pressionada a tecla_ _**Shift**_ _ou a tecla_ _**Ctrl**_ _, é possível selecionar vários elementos de uma só vez ou remover elementos da seleção atual._

![](../../.gitbook/assets/11%20%287%29.png)

3 – Modificar o novo grupo de colunas:

1. Clique duas vezes para editar um dos novos grupos e renomeie-o como **Coluna curta.**
2. Ajuste a altura da nova coluna para alinhar com a parte superior do **Piso do** **terraço inferior** \(3’-2"\). Para fazer isso, selecione e arraste a face da coluna para baixo ao longo do eixo azul \(**Eixo Z**\) e mantenha pressionada a tecla **Shift**. Passe o cursor sobre qualquer lugar na face superior do **Piso do terraço inferior** e a altura da coluna será automaticamente alinhada com o Terraço inferior. Uma vez definida a altura, clique para concluir.

![](../../.gitbook/assets/12%20%284%29.png)

_**Observação:**_ _É possível verificar a altura das colunas curtas usando a ferramenta_ _**Medir \(ME\)**_ _. Outra opção é selecionar uma das arestas verticais da coluna e ver seu comprimento na_ _**paleta Propriedades**._

4 – Com as técnicas que você acabou de aprender, copie a coluna curta mais afastada para o lado oposto do **Piso do terraço inferior** para criar a última coluna restante.

![](../../.gitbook/assets/13%20%284%29.png)

