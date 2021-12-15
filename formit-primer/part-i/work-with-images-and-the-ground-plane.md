# 1.2 – Configuração de projeto com imagens e grade

_É possível importar imagens PNG ou JPG para o plano de chão do modelo selecionando Arquivo &gt; Importar na barra de navegação. No entanto, para obter mais controle sobre a escala e a posição de uma imagem importada, podemos criar um material personalizado e aplicá-lo a um retângulo que nós mesmos desenhamos._

_Se você não tiver concluído a última seção, faça o download e abra o arquivo_ _**1.2 – Project Set Up with Images and Grid.axm**_ _nos_ _**Conjuntos de dados da Parte 1 do Manual do FormIt**._

## **Calcular tamanho da imagem**

O arquivo **plan.png** fornecido é uma imagem de uma planta impressa em uma folha de 24" x 26" \(ARCO D\), que tem 3600 pixels de largura por 2400 pixels de altura. Conhecendo a escala de desenho \(¼"=1'-0"\) e as cotas da imagem, é possível calcular que 1’ = 25 pixels, o que significa que a imagem deve ser 144'x96' quando importada para o FormIt em escala completa.

![](../../.gitbook/assets/0%20%281%29.png)

## **Importar uma imagem para escala**

1 – Clique no ícone **Vista superior** na **Barra de navegação flutuante** para ver a cena de cima.

![](../../.gitbook/assets/1%20%281%29.png)

2 – Selecione a **ferramenta Retângulo \(R\)** na barra de ferramentas de esboço 3D.

![](../../.gitbook/assets/2%20%281%29.png)

3 – Para criar um retângulo que seja exatamente **144’** x **96’**, clique em qualquer lugar no espaço de trabalho para definir o ponto inicial e, em seguida, mova o mouse para visualizar e definir o comprimento do primeiro lado. Comece a digitar um valor de cota para acessar uma caixa de diálogo na qual é possível inserir a cota exata. Clique em **OK** ou pressione a tecla **Enter** para confirmar a cota. Repita o processo para definir o comprimento do segundo lado e concluir o retângulo.

![ Insira o comprimento do primeiro lado do retângulo.](../../.gitbook/assets/3%20%281%29.png)

![ Insira o comprimento do segundo lado do retângulo.](../../.gitbook/assets/4%20%281%29.png)

![Conclua o retângulo.](../../.gitbook/assets/5%20%281%29.png)

4 – Para criar o novo material de “Planta de piso”:

1. Abra a **paleta Materiais**.
2. Clique no ícone **+** para criar um novo material.
3. Nomeie o novo material “**Planta de piso”.**
4. Em **MAPAS**, clique na miniatura de visualização **Textura** e navegue para **plan.png** na pasta **Conjunto de dados da Residência Farnsworth &gt; Arquivos de suporte &gt Imagens**. Em seguida, clique em **Abrir**.
5. Em **PROPRIEDADES**, altere a escala da imagem inserindo **144'** no campo **Escala horizontal** e **96'** no campo **Escala vertical**. Observe que desbloquear as escalas horizontal e vertical \(ícone **elo de corrente**\) pode ser necessário para inserir valores que alteram as proporções da imagem.
6. Marque **Transparência** e defina-a em torno da metade. Isso ajudará a alinhar a imagem da planta de piso importada com a imagem de satélite.
7. Clique em **OK** para finalizar o material.

![](../../.gitbook/assets/create-1.png)

5 – Para pintar o retângulo:

1. Na **paleta Materiais**, clique uma vez na miniatura **Material da planta de piso** para pintar com esse material.
2. Clique no retângulo desenhado para pintá-lo. Pressione **Esc** para sair da ferramenta Pincel.

![](../../.gitbook/assets/7.jpeg)

6 – Se o material for exibido invertido ou em sentido contrário, talvez seja necessário inverter a face. É possível fazer isso clicando com o botão direito do mouse para acessar o **menu de contexto** e selecionando o botão Inverter face \(FF\).

![](../../.gitbook/assets/8.png)

## **Alinhar a imagem importada com a imagem de satélite**

1 – Para mover a imagem, primeiro selecione o retângulo clicando duas vezes nele. Em seguida, clique e arraste o retângulo e mova-o até que ele se sobreponha à construção na imagem de satélite. Voltaremos a alinhar perfeitamente mais tarde, apenas tentaremos aproximá-lo por enquanto.

![](../../.gitbook/assets/9.png)

2 – Para rotacionar o retângulo para alinhar com a imagem do satélite:

1. Clique com o botão direito do mouse no retângulo para abrir o menu de contexto. Selecione **Rotacionar \(Q\).**
2. O **widget Rotacionar** é exibido no meio do retângulo. Selecione o widget clicando uma vez na alça laranja no meio. Mova o widget para o canto inferior esquerdo do retângulo. Ele efetuará o snap ao canto. Clique para posicioná-lo.
3. Digite **9**. A caixa de cota será exibida. Clique em **OK** para rotacionar o retângulo em sentido anti-horário em 9 graus.

![](../../.gitbook/assets/10.png)

![](../../.gitbook/assets/11.png)

## **Alinhar a grade com a imagem do satélite**

1 – Agora, alinharemos a grade com a imagem do satélite e a planta de piso. Clique com o botão direito do mouse em qualquer lugar no **plano de chão** e selecione **Definir eixos \(SZ\)**.

![](../../.gitbook/assets/12.png)

2 – O widget **Definir eixo** será exibido. Mova o eixo para o canto inferior esquerdo do retângulo, onde ele deve efetuar o snap. Clique para posicioná-lo.

![](../../.gitbook/assets/13.png)

3 – Clique na alça na extremidade do eixo vermelho. Mova a alça para o canto inferior direito do retângulo para que o eixo vermelho se alinhe com a aresta inferior do plano. Clique fora do espaço para confirmar essa alteração.

![](../../.gitbook/assets/14.png)

4 – Para alinhar a vista com a nova grade, clique no ícone Vista superior na barra de navegação para redefinir a cena.

![](../../.gitbook/assets/15.png)

5 – Para garantir que as construções em ambas as imagens se sobreponham, selecione a planta para movê-la mais uma vez até que ela se sobreponha corretamente à imagem de satélite.

![](../../.gitbook/assets/16.png)

6 – A imagem de satélite, o retângulo e a grade agora estão alinhados, o que simplificará o esboço 3D.

