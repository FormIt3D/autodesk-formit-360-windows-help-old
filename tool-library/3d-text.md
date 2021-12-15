# 3D Text

## Fornecido pelo Dynamo

No FormIt 2021 e versões mais recentes, é possível gerar e modificar objetos de texto 3D, fornecidos pelo Dynamo. O Dynamo permite editar a fonte, o tamanho e outras propriedades do texto no local, sem a necessidade de gerar novamente e reposicionar o texto quando as edições são necessárias.

![](../.gitbook/assets/3d-text.gif)

## Inserção de texto 3D

![](../.gitbook/assets/3d-text-placement.gif)

* Vá para o painel do Dynamo no FormIt para Windows e certifique-se de que você esteja no diretório Dynamo Samples.
* Clique na amostra 3D Text.
* Mova o cursor para a tela e você verá o texto 3D ser exibido no cursor.
   * Antes de inserir, é possível passar o cursor sobre a geometria para orientar o texto 3D de forma diferente; por exemplo, em uma superfície vertical para fazer o texto se alinhar verticalmente. Também é possível pressionar Tab para alternar entre orientações.
* Clique para inserir o texto 3D, que será gerado em um grupo do FormIt.
* Após inserir, o painel Properties será exibido para revelar as opções disponíveis para 3D Text.

## Iteração no local

A maior vantagem de usar o Dynamo para gerar texto 3D é que editá-lo é fácil, e ele mantém o texto em sua posição atual, para rápida iteração.

As opções 3D Text estão disponíveis no painel Properties quando o 3D Text Group é selecionado ou ao editar o grupo.

Após colocar o texto 3D inicialmente, o painel Properties será exibido automaticamente. Também é possível selecionar o Group e alternar para Properties ou clicar duas vezes em Group para alternar automaticamente para o painel Properties.

![](../.gitbook/assets/3d-text-options.png)

### Text

Insira o texto que você deseja que a geometria 3D Text exiba. Esse campo também oferece a visualização da fonte e da justificação selecionadas. Pressione Enter/Return para várias linhas.

### Font

Selecione a fonte para 3D Text. Essa lista exibirá as fontes disponíveis no computador. Selecionar uma nova fonte atualizará o campo Text.

Observe que algumas fontes têm geometria mais complexa, e mais tempo pode ser necessário para gerá-las usando o Dynamo.

### Justification

Isso moverá o texto para alinhamento em relação à origem Group's Local Coordinate System.

* Esquerda garantirá que o texto comece na origem do grupo e se expanda para a direita.
* Centralizado garantirá que o texto esteja sempre centralizado em relação à origem do grupo.
* Direita garantirá que o texto termine na origem do grupo.

![](../.gitbook/assets/3d-text-justification-combined.png)

### Text Size

![](../.gitbook/assets/3d-text-text-size.png)

A altura do texto, nas unidades atuais do FormIt.

### Extrusion Depth

A quantidade de extrusão 3D do texto, nas unidades atuais do FormIt. O texto 3D foi projetado para ser sólido; portanto, esse valor não pode ser zero. No entanto, você pode torná-lo muito próximo de 0, para que seja menos óbvio que foi feita a extrusão.

### Tracking

![](../.gitbook/assets/3d-text-tracking.png)

O rastreamento é útil para ajustar o espaçamento padrão entre letras de uma fonte específica. Usa as unidades atuais do FormIt e pode ser positivo ou negativo. Por exemplo, em pés, 0,25 adicionará 3" de espaçamento entre cada letra. Por outro lado, -0,25 aproximará todas as letras em 3".

### Multi-Line Spacing

![](../.gitbook/assets/3d-text-multi-line.png)

Se você tiver várias linhas no campo Text, esse valor controlará o espaço entre cada linha de texto. Usa as unidades atuais do FormIt.

### Invert Text

![](../.gitbook/assets/3d-text-inverted.png)

Quando True, essa opção criará um sólido em torno do texto e removerá o texto dele, fornecendo o resultado de texto “invertido” – como se o texto tivesse sido cortado de um material.

### Inverted Text Border

![](../.gitbook/assets/3d-text-inverted-border.png)

Somente se aplica quando Invert Text é true. Especifica a quantidade de borda em torno do texto a ser usada para o sólido do qual o texto é removido. Usa as unidades atuais do FormIt.

### Curve Faceting Quality

As curvas das fontes são convertidas em segmentos de linha usando 3D Text; portanto, esse valor controla a precisão com que as curvas são facetadas.

Números menores resultarão em facetas mais grosseiras \(segmentos mais longos\) e números maiores resultarão em facetas mais finas \(segmentos mais curtos\). Esse valor substitui as configurações de facetamento Curve and Surface do FormIt em Preferences.

### Run

Após editar as opções, clique no botão “Run” para executar o gráfico subjacente do Dynamo e gerar novos resultados. Esse botão ficará azul quando os parâmetros forem alterados, para que você saiba que “Run” precisa ser clicado para ver as atualizações na geometria final.‌

### Edit Embedded Graph

Clicar nesse botão iniciará o ambiente do editor gráfico do Dynamo, para que você possa visualizar e editar o gráfico subjacente do Dynamo para alterar rapidamente os parâmetros e ver as atualizações ao vivo ou para inspecionar/ajustar a lógica. Isso não é necessário, mas pode ser útil para solução de problemas ou para edição mais rápida. Veja abaixo para obter mais informações.

## Iterate Faster in Dynamo

Se você estiver iterando em opções 3D Text, poderá ser mais rápido iniciar o editor gráfico do Dynamo, que permitirá ajustar os parâmetros e ver as alterações em tempo real. Isso também permite inspecionar a lógica por trás do gráfico, caso haja problemas.

![](../.gitbook/assets/3d-text-edit-embedded.png)

É possível clicar no botão “Edit Embedded Graph” no painel Properties para iniciar o editor gráfico do Dynamo.

![](../.gitbook/assets/3d-text-edit-embedded-windows.png)

## Solução de problemas

O texto 3D usa o Dynamo nos bastidores e o Dynamo usa um kernel de modelagem chamado ASM para gerar sua geometria, que é passada de volta para o FormIt.

Algumas fontes podem criar “curvas com autointerseção” ou outra geometria problemática, que causam erros no ASM.

Se você receber um erro ao tentar executar 3D Text ou se as letras desaparecerem, será recomendável clicar em “Edit Embedded Graph” para ver o que está errado com o gráfico e onde pode estar acontecendo a falha.

Algumas fontes também têm problemas conhecidos que impedem que elas sejam transformadas na geometria adequada. Bahnschrift é um exemplo disso. Se você encontrar outra fonte problemática, [nos informe nos fóruns](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=pt-br). Faremos o que for possível para corrigir problemas com fontes específicas.





