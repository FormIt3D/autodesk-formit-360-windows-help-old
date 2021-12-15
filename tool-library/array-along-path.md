# Array Along Path

## Fornecido pelo Dynamo

No FormIt 2021 e versões mais recentes, é possível dispor objetos ao longo de um caminho em uma matriz e personalizar rapidamente os resultados no local. A amostra Array Along Path é fornecida pelo Dynamo, o que significa que o corrimão resultante é facilmente configurável para obter os resultados desejados, e a nova execução da lógica atualizará a geometria no local.

![](../.gitbook/assets/array-along-path.gif)

## Iniciar Array Along Path

* Vá para o painel do Dynamo no FormIt para Windows e certifique-se de que você esteja no diretório Dynamo Samples.
* Clique na amostra Array Along Path.
* No lado esquerdo da tela, você verá um prompt para “Select object\(s\) to array”.
   * É possível selecionar qualquer combinação de objetos do FormIt para esta etapa.
   * Depois de selecionar algo, é possível clicar na seta “Avançar” no lado esquerdo da tela ou pressionar Enter.
* Agora você verá um prompt para “Select path for array”.
   * Aqui, você deve selecionar somente uma série de arestas contíguas ou um grupo que contém uma série de arestas contíguas.
   * Depois de selecionar o caminho, clique no botão “finish” ou pressione Enter.
* O painel do Dynamo indicará que está processando as alterações. Ao terminar, você terá uma matriz, gerada pelo Dynamo em um grupo do FormIt, pronta para modificação \(veja abaixo\).

## Iteração no local

Após executar Array Along Path, você verá que seus resultados estão definidos com os valores padrão; por isso, será conveniente modificá-los para atender às suas necessidades.

Quando a amostra Array Along Path é executada, ela cria um novo grupo que contém os resultados, e o FormIt selecionará automaticamente o grupo e mostrará as opções disponíveis para essa instância de Array Along Path.

Você sempre pode retornar às propriedades Array Along Path selecionando o grupo e alternando para o painel Properties ou editando o grupo que mostrará automaticamente Properties.

![](../.gitbook/assets/array-along-path-options.png)

### Select Object\(s\) to Array <a id="run"></a>

Clique nessa opção para voltar ao assistente de seleção e alterar quais objetos estão sendo dispostos em matriz.

### Select Array Path

Clique para voltar ao assistente de seleção para alterar o caminho usado para calcular a matriz.

### Array Type <a id="run"></a>

Isso alterna o tipo de matriz para cálculo: By Distance ou By Number.

**Quando true**, o cálculo será “By Distance”. O número abaixo se refere à distância entre cópias.

**Quando false**, o cálculo será feito por “By Number of Copies”. O número abaixo desse campo se refere ao número de cópias que se ajustam ao longo do caminho.

### Include Original Selection In Results

Quando **true**:

* Os objetos selecionados serão contabilizados como uma das novas cópias.
* O grupo do Dynamo resultante incluirá a seleção original em seus resultados, de modo que as novas cópias efetuarão a luta Z com a seleção original. É possível colocar a seleção original em uma [Camada](layers.md) e desativá-la para ocultá-la.

Quando **false**:

* A matriz resultante **não** incluirá a seleção original, portanto você obterá o número de cópias especificado **além** da seleção original, e os resultados não efetuarão a luta Z.

### Rotate Copies Along Path

Quando **true**, as cópias são rotacionadas para manter a orientação do objeto original com relação ao caminho.

Quando **false**, as cópias não são rotacionadas, somente movidas.

### Use Relative Positioning Along Path

Quando **true**:

* Cada cópia manterá a distância entre o caminho e o objeto original.
* Se o objeto original **não** estiver posicionado em uma das extremidades do caminho, o maior segmento restante do caminho será usado para o cálculo da matriz.

Quando **false**:

* O comprimento inteiro do caminho será usado para calcular a matriz, independentemente de onde o objeto original está em relação ao caminho.
* Isso dissocia a localização do caminho em relação ao objeto e simplesmente usa o caminho inteiro. Isso será útil se o caminho e o objeto não estiverem próximos um do outro.

### Reverse Path Direction

Somente para caminhos fechados. Ao usar Array Along Path com um caminho fechado, a direção da curva pode inesperadamente inverter os resultados esperados da matriz. Alterne para **true** para inverter a direção da matriz se os resultados forem invertidos.

### Run <a id="run"></a>

Após editar as opções, clique no botão “Run” para executar o gráfico subjacente do Dynamo e gerar novos resultados. Esse botão ficará azul quando os parâmetros forem alterados, para que você saiba que ele precisa ser clicado para ver as atualizações na geometria final.‌

### Edit Embedded Graph <a id="edit-embedded-graph"></a>

Clicar nesse botão iniciará o ambiente do editor gráfico do Dynamo, para que você possa visualizar e editar o gráfico subjacente do Dynamo para alterar mais rapidamente os parâmetros e ver as atualizações ao vivo ou para inspecionar/ajustar a lógica.



## Selecting Geometry

Ao selecionar objetos para Array Along Path e outros gráficos do Dynamo com base em seleção:

* Será possível selecionar qualquer combinação de objetos do FormIt: vértices, arestas, faces, sólidos, grupos e malhas.
   * Observe que, dependendo da etapa, alguns desses objetos não devem ser selecionados.
   * Por exemplo, ao selecionar o caminho, você deverá selecionar somente uma série contígua de arestas ou um Grupo que contém uma série contígua de arestas. Qualquer outra coisa causará a falha do gráfico.
* Será possível clicar duas vezes em um objeto para selecionar tudo que está anexado.
* Será possível usar a janela de seleção de área para capturar uma série de objetos.
* Será possível selecionar objetos já selecionados para desfazer a seleção.
* Ao menos um objeto é necessário para continuar com uma etapa com base na seleção.



