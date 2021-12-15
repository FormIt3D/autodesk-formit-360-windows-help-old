# Malhas

A partir da v17.0, o FormIt oferece um novo tipo de geometria: Meshes.

As malhas são representações leves de objetos do FormIt padrão e são ótimas para melhorar o desempenho da geometria de polígonos altos, como mobiliário ou ambientes 3D, como pessoas, árvores, carros e sinalização. As malhas também são ótimas para geometria DWG complexa que, de outra forma, poderia afetar o desempenho do FormIt.

Os objetos podem ser convertidos em malhas e as malhas podem ser convertidas de volta em objetos sem perder nenhum dado. Alguns tipos de arquivo são automaticamente importados como malhas, como OBJ, STL e DWG. Saiba mais sobre a conversão entre tipos e outros benefícios e limitações de malhas abaixo.

### Converter objetos em malhas

Qualquer combinação de vértices, arestas, faces ou corpos sólidos pode ser convertida em malhas.

Basta selecionar Objects e usar o atalho OM \(Objects to Meshes\) ou clicar com o botão direito do mouse e selecionar Objects to Meshes no menu de contexto:

![](../.gitbook/assets/context-menu_object-to-mesh.PNG)

Quando os objetos tiverem sido convertidos em malhas, você verá uma mensagem de confirmação na parte superior da tela:

![](../.gitbook/assets/success_object-to-mesh.PNG)

**Ao converter objetos em malhas:**

* As arestas que foram suavizadas nos objetos permanecerão suavizadas nas malhas resultantes.
* As orientações de material nos objetos permanecerão inalteradas nas malhas resultantes.
* Uma malha será criada para cada material aplicado. Por exemplo, se você converter um único cubo pintado em 6 cores diferentes, você obterá 6 malhas diferentes.
   * Converter de volta em um objeto vedará novamente as malhas individuais de volta em um corpo sólido.
* Selecionar um corpo sólido converterá e substituirá todo o corpo por uma malha, mas selecionar arestas ou vértices individuais pertencentes a um sólido criará uma nova malha sobre a geometria existente, sem afetar o corpo original.
* A conversão de um conjunto de arestas ou vértices criará uma única malha de linhas \(uma malha feita de arestas\) ou uma única malha de ponto \(uma malha feita de pontos\), o que significa que você não será capaz de selecionar arestas ou vértices individuais depois que eles forem combinados em uma única malha. Converta-os de volta em objetos se você desejar ajustar a posição de um único elemento.

**Converter geometria agrupada em malhas:**

* As malhas se tornam ainda mais poderosas quando você pode converter um grupo inteiro e todos os seus grupos aninhados em malhas.
* Os grupos e seu conteúdo aninhado podem ser convertidos em grupos usando um plug-in:
   * Procure o ícone Plugin Manager no lado direito do aplicativo:
      * ![](../.gitbook/assets/plugin-manager_icon.PNG)
   * Localize o plug-in “Mesh + Unmesh All” e clique na caixa de seleção para instalá-lo:
      * ![](../.gitbook/assets/plugin-manager_mesh-unmesh-all.PNG)
   * O plug-in Mesh + Unmesh All será carregado. Basta selecionar um grupo que contenha os objetos que você deseja converter em malhas e clicar em Mesh All.
      * ![](../.gitbook/assets/mesh-unmesh-all-plugin.PNG)
   * Ao converter objetos aninhados ou malhas com esse plug-in, você verá uma mensagem de atualização na parte superior da tela informando quantos grupos e instâncias de grupos foram afetados pela operação:

![](../.gitbook/assets/success_mesh-all.PNG)

### Interação com malhas

**Por causa de sua natureza leve, as malhas têm certas limitações e comportamentos:**

* Não será possível editar faces, arestas ou vértices individuais de uma malha.
   * No entanto, será possível reformatar malhas e mover malhas individuais criadas como resultado de diferentes materiais aplicados às faces \(consulte acima\).
* O snap a malhas será limitado às faces e vértices de malhas. Para fins de desempenho, o snap e a inferência não funcionarão com arestas de malhas.
   * No entanto, os arquivos DWG convertidos em malhas \(um tipo diferente de malha conhecido como malha de linhas\) manterão a capacidade de efetuar inferência e snap a arestas de malha.
* As malhas não poderão ter níveis aplicados.
* As malhas não informarão problemas herméticos ou de face posterior. Converta-os de volta em objetos para ver se eles são herméticos ou não.
   * Os objetos que estavam herméticos antes da conversão em uma malha permanecerão herméticos quando convertidos de volta em um objeto.
* Não é possível usar as malhas em operações avançadas de modelagem, como Unir/Cortar sólido, Casca 3D, Deslocamento 3D, Concordância, Elevação, Varredura ou Cobertura.

Caso contrário, as malhas serão exibidas e se comportarão como qualquer outro objeto do FormIt: colocadas em grupos, atribuídas a camadas, visualizadas em cenas, usadas para análise etc.

**Você saberá que está interagindo com uma malha se a dica de ferramenta relatar “On Mesh” ou se o painel Properties relatar uma malha:**

![](../.gitbook/assets/snap_on-mesh.PNG)

![](../.gitbook/assets/properties-panel_mesh.PNG)

**Alguns tipos de arquivo são automaticamente importados como malhas para melhorar o desempenho:**

* Os arquivos STL e OBJ, que podem conter geometria densa, como nuvens de pontos de outros aplicativos, são automaticamente importados como malhas.
* Os arquivos DWG, que podem conter milhões de pequenos segmentos de aresta em curvas de alta qualidade, são automaticamente importados como malhas.

### Converter malhas de volta em objetos

Basta selecionar Meshes e usar o atalho MO \(Meshes to Objects\) ou clicar com o botão direito do mouse e selecionar Meshes to Objects no menu de contexto:

![](../.gitbook/assets/context-menu_mesh-to-object.PNG)

Quando os objetos tiverem sido convertidos em malhas, você verá uma mensagem de confirmação na parte superior da tela:

![](../.gitbook/assets/success_mesh-to-object.PNG)

**Ao converter malhas de volta em objetos:**

* Quaisquer objetos que anteriormente eram sólidos/herméticos antes de converter em uma malha serão unidos novamente em um sólido hermético ao converter de volta em um objeto.
* Converter uma série de arestas \(por exemplo de um arquivo DWG\) ou uma série de vértices \(por exemplo de uma nuvem de pontos\) em uma malha e convertê-los de volta colocará automaticamente os objetos sem malha em um grupo.
   * Isso impedirá que as novas arestas ou vértices mesclem com outra geometria, o que poderá ter efeitos adversos e afetar o desempenho.
   * Será possível desagrupar simplesmente o grupo resultante para liberar as arestas e/ou vértices.

**Converter malhas agrupadas de volta em objetos:**

* Consulte as instruções acima para usar o plug-in Mesh + Unmesh All para converter grupos e suas malhas aninhadas de volta em objetos.

