# Modelagem avançada

Em nossos exercícios da Residência Farnsworth, nos concentramos em ferramentas básicas de modelagem, como Desenhar, Arrastar face, Mover, Matriz e Deslocar face. Também abordamos os fluxos de trabalho essenciais que envolvem grupos, camadas, materiais e níveis. Nesta seção, apresentaremos as ferramentas avançadas de modelagem **Varredura** e **Arredondamento**.

Se você não tiver concluído a última seção, faça o download e abra o arquivo **farnsworth05.axm** na [pasta Manual do FormIt](https://autodesk.app.box.com/s/thavswirrbflit27rbqzl26ljj7fu1uv/1/9025446442).

## Varredura

Use a ferramenta Varredura para criar uma cornija ao longo do telhado.

1. Com a ferramenta **Retângulo \(R\)**, crie um perfil de **6" de altura por 4 5/8" **em qualquer canto do telhado.

   ![](../../.gitbook/assets/a7297208-cefe-42e7-95ca-1e8ea122ac38.png)

2. Crie outro perfil de **Retângulo \(R\)** que seja **2" x 2".**

   ![](../../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54.png)

3. **Clique uma vez** para selecionar a linha entre os perfis. Use a tecla **Delete** para remover a linha; isso cria um único contorno.

   ![](../../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_2.png)

4. Selecione a [**ferramenta Varredura \(SW\)**](../../tool-library/cover-sweep-loft.md) no [**menu Modelagem avançada**](../../formit-introduction/tool-bars.md)**.**

   ![](../../.gitbook/assets/8a17017b-b824-48ac-ba24-064a24e7a6ad.png)

5. A barra de ferramentas **Geometria avançada** é exibida no canto superior esquerdo da tela com instruções de texto de ajuda.

   ![](../../.gitbook/assets/e8badff2-acd9-4393-af5f-adae2424ad47.png)

6. **Clique uma vez** para selecionar a face que você acabou de desenhar. Esse será o **perfil** no qual você deseja efetuar a varredura.

   ![](../../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_3.png)

7. A barra de ferramentas **Geometria avançada** muda quando você seleciona uma face. Agora, ela solicita que você selecione um **caminho** para a varredura.

   ![](../../.gitbook/assets/df9fc338-15c0-4953-9ec1-c977117efc4d.png)

8. **Clique uma vez** para selecionar a **face superior do telhado**. A ferramenta infere as arestas da face como caminho. A varredura é criada após selecionar o telhado.

   ![](../../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_4.png)

9. Clique duas vezes para selecionar todo o elemento de cornija. **Agrupe \(G\)** a cornija. Edite o grupo e nomeie-o como **cornija.**

   ![](../../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_5.png)

10. Pinte o grupo de cornija com o material **Concreto &gt; Branco** para coincidir com o telhado. Adicione o **grupo de cornija** à camada **telhado**.

Será necessário ajustar a **altura das colunas** para que termine na cornija. Edite um dos grupos de colunas altos, selecione a face superior e reduza-a para a altura correta. Também pode ser necessário ajustar a localização das colunas para que elas fiquem alinhadas com as lajes. Agora é um bom momento para fazer esses pequenos ajustes.

## Arredondamento

Agora você aprenderá mais sobre a ferramenta Arredondamento e como criar uma aresta arredondada e dar uma aparência mais suave a um móvel.

1. **Desative** a camada do **telhado** para que você possa ver dentro da casa.
2. Crie um **Retângulo \(R\)** de **4’ x 7"** no canto nordeste da casa. Selecione a face e faça a extrusão dela a **1'-6" de altura.**

   ![](../../.gitbook/assets/upperterracesketch_20.png)

3. Selecione a [**ferramenta Arredondamento \(FI\)**](../../tool-library/cover-sweep-loft.md) nas **ferramentas avançadas de modelagem** na [**Barra de ferramentas de ação**](../../formit-introduction/tool-bars.md)**.**

   ![](../../.gitbook/assets/f7e388e3-4ad0-4fef-a701-0d3176adc2c5.png)

4. Altere o valor padrão de **arredondamento** para 1" na caixa de diálogo exibida.
5. **Clique uma vez** na face superior da cama. O arredondamento é criado automaticamente após selecionar a face.

   ![](../../.gitbook/assets/upperterracesketch_21.png)

## Árvore de grupos

Em vez de editar o grupo para nomeá-lo e categorizá-lo, vamos usar a **Árvore de grupos**, que permite conduzir rapidamente várias tarefas de gerenciamento de modelo.

1. **Clique duas vezes** para selecionar a cama inteira. Adicione a cama ao **Grupo \(G\).**
2. Clique no ícone **Árvore de grupos** nas paletas à direita.

   ![](../../.gitbook/assets/groupstree.png)

3. Se você selecionar o grupo de cama na tela, ele será realçado na lista **Árvore de grupos** \(o oposto também será verdadeiro, se você selecionar um grupo na lista, ele será realçado na tela\).
4. É possível **clicar duas vezes** no nome na lista e alterá-lo para **Cama** – todas as instâncias do grupo serão atualizadas – no nosso caso, há apenas uma.
5. Enquanto o **Grupo de cama** está selecionado na lista, é possível definir a categoria como **Mobiliário** na lista suspensa na parte superior da paleta Árvore de grupos.

   ![](../../.gitbook/assets/groupstree_palette.png)

## Mesclar arestas, suavizar arestas e filtragem de seleção

Agora, vamos ocultar as arestas indesejadas em nosso mobiliário, para dar a ele uma aparência mais fluida e mais suave.

1. **Clique duas vezes** para editar o grupo. Selecione a cama inteira com um **clique duplo**. **Clique com o botão direito do mouse** e escolha **Mesclar \(MG\)** no menu de contexto.

   ![](../../.gitbook/assets/upperterracesketch_215.png)

2. Use o **Filtro de seleção** para restringir uma seleção de janela para selecionar somente **Arestas.**

   ![](../../.gitbook/assets/25b2428d-bc93-4ae4-9b8a-d8f3749ddb43.png)

3. **Arraste o mouse** do canto superior esquerdo para o canto inferior direito para executar uma **seleção de janela**. Selecione por janela o arco e a aresta em cada canto da cama. Mantenha pressionada a tecla **Ctrl** ou **Shift** para adicionar ao conjunto de seleção.
4. **Clique com o botão direito do mouse** e escolha **Suavizar arestas \(SE\)**

   ![](../../.gitbook/assets/upperterracesketch_216.png)

5. Para tornar essas arestas visíveis novamente, **clique uma vez** para selecionar a face superior da cama, **clique com o botão direito do mouse** e selecione **Facetas suaves** \(UE\).

   ![](../../.gitbook/assets/upperterracesketch_217.png)

6. Altere o **Filtro de seleção** de volta para incluir faces e grupos novamente. Ative novamente a camada do **telhado**. Seu modelo de Residência Farnsworth está indo bem.

   ![](../../.gitbook/assets/upperterracesketch_22.png)

