# 1.7 – Pintar com materiais

Como vimos em um **exercício anterior**, você pode criar seus próprios materiais e, em seguida, pintar faces com esses materiais no FormIt. Neste exercício, você vai criar e editar mais materiais, bem como importar materiais da Bibliotecas de materiais da Autodesk.

_Se você não tiver concluído a última seção, faça o download e abra o arquivo_ _**1.7 – Paint with Materials.axm**_ _nos_ _**Conjuntos de dados da Parte 1 do Manual do FormIt**._

## **Criar as paredes de vidro**

1 – Para visualizar a planta que contém as cotas que vamos referenciar, vá para a **paleta Camadas** e ative a camada **Imagem da planta**.

2 – Selecione a **ferramenta Retângulo \(R\)**. Vamos criar um retângulo diretamente na parte superior do grupo do piso existente. Certifique-se de que você não esteja editando o Grupo do piso, e sim desenhando na parte superior do objeto agrupado existente.

![](../../.gitbook/assets/0%20%283%29.png)

3 – Para iniciar o retângulo na área de vidro:

1. Clique no canto posterior do piso existente e mova o mouse ao longo da aresta mais curta.
2. Digite **28’-8"** para definir o comprimento da primeira aresta e clique em **OK**. Esse deve ser o mesmo comprimento da aresta curta existente do piso.
3. Para definir a segunda aresta, comece a mover o mouse ao longo da aresta mais longa existente do piso. Digite **55'-5 ½"** para definir o comprimento da segunda aresta e, em seguida, clique em **OK**.
4. Pressione **ESC** para sair da ferramenta de retângulo. Clique uma vez dentro do novo retângulo para selecionar a face e começar a arrastá-la para cima.

![](../../.gitbook/assets/1%20%283%29.png)

4 – Para definir a altura, mova o mouse para cima ao longo do **Eixo Z**, pressione a tecla **Tab** e insira **11'-2"**.

![](../../.gitbook/assets/2%20%284%29.png)

_**Observação:**_ _Sempre que você estiver usando uma ferramenta na qual possa inserir uma cota, poderá pressionar_ _**Tab**_ _ou apenas começar a digitar os números._

5 – Clique duas vezes e **agrupe \(G\)** a nova geometria.

6 – Clique duas vezes no grupo para editá-lo. Na **paleta Propriedades**, nomeie o grupo como **Paredes de vidro.**

![](../../.gitbook/assets/3%20%283%29.png)

7 – Para definir a espessura da parede de vidro:

1. Clique com o botão direito do mouse na face superior e escolha a **ferramenta Deslocar face \(OF\).**
2. Mova o cursor do mouse para dentro e digite **4".**
3. Clique em **Esc** duas vezes para limpar a ferramenta e a seleção.

![](../../.gitbook/assets/4%20%2817%29.png)

​_**Observação:**_ _A unidade padrão para projetos imperiais é pés, tal como no Revit. Se você inserir um número sem uma unidade especificada, como_ _**4**, obterá_ _**4 pés \(4’\)**_ _e não_ _**4 polegadas \(4"\)**._

8 – Para recortar a área interna, clique uma vez na face superior interna para selecioná-la e, em seguida, clique novamente para iniciar a operação de **arrastar a face**. Empurre a face para baixo até que ela desapareça e clique no espaço para concluir o processo.

![](../../.gitbook/assets/5%20%2812%29.png)

_**Observação:**_ _No FormIt, ao contrário de outros softwares, não é possível empurrar acidentalmente a face que você está tentando excluir “muito longe”, de modo que uma nova extrusão negativa seja formada._

9 – Termine o modo **Editar grupo** clicando duas vezes no espaço ou pressionando **Esc.**

10 – Selecione o grupo **Paredes de vidro** com um único clique e coloque-o na camada **Piso do edifício principal**.

![](../../.gitbook/assets/6%20%2813%29.png)

## **Importar um material da Bibliotecas de materiais da Autodesk**

1 – Edite o grupo **Paredes de vidro** novamente clicando duas vezes nele.

2 – Para importar um novo material para o modelo:

1. Vá para a **paleta Materiais**.
2. Selecione **Amostra de material** no menu suspenso, na parte superior da paleta, para navegar através da **Biblioteca de materiais da Autodesk.** ​
3. Clique na pasta **Vidro+Vidraça** para abri-la.
4. Localize o material **Vidro – Matiz azul** e clique uma vez nele para adicionar esse material à biblioteca de materiais na opção **No esboço**.
5. Observe que você deve estar de volta na biblioteca **No esboço**, que agora inclui o material recém-selecionado.

![](../../.gitbook/assets/7%20%288%29.png)

![](../../.gitbook/assets/8%20%288%29.png)

3 – Após adicionar o material, você deve estar automaticamente na ferramenta **Pincel**. Se não estiver, clique uma vez no material **Vidro – Matiz Azul** novamente. Para pintar todas as paredes, clique duas vezes na geometria com a ferramenta **Pincel**. Isso permitirá aplicar o material selecionado em todo o objeto. ![](../../.gitbook/assets/9%20%281%29.png)​

4 – Clique em **Esc** para sair da ferramenta **Pincel**. Clique em **Esc** novamente ou clique duas vezes no espaço para sair do grupo.

## **Cópia rápida do piso para criar o telhado**

1 – Para criar rapidamente o telhado com base na geometria do piso:

1. Selecione o grupo **Piso** com um único clique.
2. Clique em um dos cantos inferiores para iniciar a ferramenta **Mover**.
3. Comece a mover o piso para cima ao longo do eixo azul \(**Eixo Z**\). Crie uma **cópia rápida** tocando na tecla **Ctrl**. Uma visualização “fantasma” da cópia deve aparecer. ​
4. Ao mover ao longo do eixo azul \(**Eixo Z**\), comece a digitar **12' 2"** e será exibida uma **caixa de diálogo Cota**. Clique em **OK** ou pressione **Enter** para finalizar o posicionamento.

![](../../.gitbook/assets/10%20%281%29.png)

![](../../.gitbook/assets/11%20%281%29.png)

## **Editar o telhado**

1 – Enquanto o grupo copiado ainda estiver selecionado, use o comando **Tornar único \(MU\)** para dissociar esse grupo do grupo do piso.

2 – Clique duas vezes no grupo para editá-lo. Nomeie novamente o grupo como **Telhado** na **paleta Propriedades**. Saia do grupo clicando duas vezes no espaço.

3 – Na **paleta Camadas**, crie uma nova **Camada** chamada **Telhado** e adicione o grupo **Telhado** a essa camada. É possível ativar e desativar a camada para verificar se os elementos corretos estão no telhado. Consulte o **Capítulo 6** para obter mais informações sobre como trabalhar com **Camadas**.

4 – Navegue de volta para a **paleta Materiais** e importe o material **Concreto – Acabamento escovado – Colorido 1** da pasta **Concreto+Asfalto**, na biblioteca de **Amostras de material** **\(Produção\)**. Observe que, ao clicar no material, a geometria selecionada será automaticamente pintada e o novo material será adicionado à biblioteca de materiais **No esboço**.

![](../../.gitbook/assets/12.jpeg)

_**Observação:**_ _Pintar um grupo fora do_ _**Modo de edição de grupos**_ _é uma técnica útil que permite pintar diferentes instâncias do mesmo grupo com diferentes materiais._

## **Criar o terraço inferior**

1 – Com base na **Imagem da planta**, crie o terraço inferior como um **Retângulo \(R\)** que tem **55' 3"** de comprimento e **22'-7 3/4"** de largura e faça a extrusão por 1’. Posicione o novo retângulo de forma que esteja a uma distância de 8 5/8" da aresta sul do edifício principal \(criaremos mais tarde a profundidade das colunas\).

_**Notas:**_

* _Consulte os capítulos anteriores para saber como desenhar e efetuar a extrusão de retângulos._
* _Talvez seja necessário ativar ou desativar a opção __**Snap à grade \(SG\)**__ para clicar no_ canto do terraço.

2 – Para finalizar o terraço inferior:

1. **Agrupe \(G\)** a geometria e nomeie-a como **Piso do terraço inferior**.
2. **Mova** o grupo para cima **2'-2"** do plano do chão.
3. Crie uma nova **Camada** chamada **Terraço inferior** e adicione o grupo à camada.
4. Adicione o **Piso do nível do terraço** ao grupo.

![](../../.gitbook/assets/13%20%281%29.png)

_**Observação:**_ _Essa imagem não representa o processo passo a passo para criar e atribuir a geometria a grupos, níveis e camadas. Para obter mais informações sobre esses processos, consulte os capítulos anteriores deste Manual._

3 – Importe o material **Pedra &gt; Pedra – Travertino**.

4 – Na **paleta Materiais**, localize o material **Travertino** importado e modifique-o:

1. Clique duas vezes na miniatura de visualização para abrir a janela pop-up **Editor de material**.
2. Clique na miniatura de visualização de **Cor** para abrir a janela pop-up **Editor de cores**.
3. Altere o campo **Valor** para **190** para escurecer o matiz do material.

![](../../.gitbook/assets/14%20%282%29.png)

5 – **Pinte** os grupos **Piso** e **Piso do terraço inferior** com o material **Travertino** modificado.

![](../../.gitbook/assets/15.jpeg)

