# Railing Along Path

## Fornecido pelo Dynamo

No FormIt 2021 e versões mais recentes, é possível gerar um corrimão ao longo de um caminho e personalizar rapidamente os resultados no local. A amostra Railing Along Path é fornecida pelo Dynamo, o que significa que o corrimão resultante é facilmente configurável para obter os resultados desejados, e a nova execução da lógica atualizará a geometria no local.

![](../.gitbook/assets/railing-along-path.gif)

## Iniciar Railing Along Path

* Vá para o painel do Dynamo no FormIt para Windows e certifique-se de que você esteja no diretório Dynamo Samples.
* Clique na amostra Railing Along Path.
* No lado esquerdo da tela, você verá um prompt para “Select path for railing”.
   * Você deve selecionar somente uma série de arestas contíguas ou um grupo que contenha somente uma série de arestas.
   * Depois de selecionar o caminho, clique no botão “finish” ou pressione Enter/Return.
* O painel do Dynamo indicará que está processando as alterações. Ao terminar, você terá um corrimão, gerado pelo Dynamo em um grupo do FormIt, pronto para modificação \(veja abaixo\).

## Iteração no local

Após executar Railing Along Path, você observará que seus resultados estão definidos com os valores padrão. Talvez isso funcione para você, mas você pode personalizar muito o corrimão para se adequar às suas necessidades.

Quando Railing Along Path é executado, ele cria um novo grupo que contém os resultados, e o FormIt selecionará automaticamente o grupo e mostrará as opções disponíveis para essa instância de Railing Along Path.

Você sempre pode retornar às propriedades Railing Along Path selecionando o grupo e alternando para o painel Properties ou editando o grupo que mostrará automaticamente Properties.

![](../.gitbook/assets/railing-along-path-options.png)

### Railing Height

A altura total do corrimão. Usa as unidades atuais do FormIt.

### Post Spacing

O espaçamento entre os pilares verticais principais. Usa as unidades atuais do FormIt.

### Add Posts at Path Vertices

Quando **true**, os pilares serão adicionados a cada vértice do caminho selecionado e o cálculo para o próximo posicionamento do pilar será redefinido nesse ponto.

Por exemplo, se você tiver selecionado uma série de três arestas, será exibido um pilar em cada um dos dois pontos internos. Isto será útil se os vértices indicarem uma alteração de direção \(como subir escadas ou dobrar cantos\) onde um pilar naturalmente ocorreria.

Quando **false**, os pilares somente serão adicionados ao longo do caminho começando em uma extremidade e medindo a distância ao longo do caminho, ignorando os vértices ao longo do caminho. Isso será útil se você tiver selecionado um arco, spline ou círculo, nos quais os vértices não são importantes e você deseja que o espaçamento dos pilares os ignore.

### Reverse Path Direction

Ao calcular o posicionamento dos pilares, a direção do caminho escolhido determinará qual extremidade do caminho iniciará a medição de espaçamento dos pilares.

Nos casos em que o espaçamento dos pilares resulta em espaço de sobra em uma extremidade não desejada do caminho, será possível alterar esse valor para **true** para inverter a curva e iniciar a medida de espaçamento dos pilares na extremidade oposta.

### Post Width + Depth

O tamanho \(na planta\) dos perfis retangulares do pilar vertical. Usa as unidades atuais do FormIt.

### Handrail Width + Height

O tamanho \(na seção\) do perfil do corrimão retangular. Usa as unidades atuais do FormIt.

### Baluster Orientation

Quando true, os balaústres serão orientados na horizontal, como os cabos. Quando false, os balaústres serão orientados verticalmente, para obter uma estética mais tradicional.

### Baluster width + Depth

O tamanho do perfil retangular do balaústre. Usa as unidades atuais do FormIt.

### Baluster Spacing

A quantidade de espaço entre cada balaústre. Usa as unidades atuais do FormIt.

### Bottom Rail Start Height

A distância entre a parte inferior do corrimão e o corrimão inferior que suporta os balaústres. Usa as unidades atuais do FormIt.

### Run

Após editar as opções, clique no botão “Run” para executar o gráfico subjacente do Dynamo e gerar novos resultados. Esse botão ficará azul quando os parâmetros forem alterados, para que você saiba que ele precisa ser clicado para ver as atualizações na geometria final.‌

### Edit Embedded Graph

Clicar nesse botão iniciará o ambiente do editor gráfico do Dynamo, para que você possa visualizar e editar o gráfico subjacente do Dynamo para alterar mais rapidamente os parâmetros e ver as atualizações ao vivo ou para inspecionar/ajustar a lógica.

