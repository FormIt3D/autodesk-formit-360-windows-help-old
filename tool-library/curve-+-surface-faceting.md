# Curva + facetamento de superfície

O FormIt é um sistema de modelagem poliédrico, portanto, objetos como círculos, arcos e splines são representados por uma série de arestas retas. De forma similar, uma superfície curva como a parede de um cilindro ou um domo é composta de uma série de faces planas com arestas de borda ocultas.

Por padrão, o FormIt usa 40 arestas ou facetas para representar um círculo e 24 facetas para representar um objeto curvado 3D como um cilindro. Para superfícies mais complexas, como um domo, um valor de 24 define a contagem de facetamento do perímetro e também afeta a intensidade da densidade com que o restante da forma é facetado.

No FormIt para Windows v18 e versões mais recentes, os valores de facetamento de curva e superfície são personalizáveis:

![](../.gitbook/assets/faceting\_planter.gif)

![](<../.gitbook/assets/faceting (1).png>)

**Curve Faceting Quality**

Alterar Curve Faceting Quality afetará o número de facetas usadas ao desenhar novos círculos e arcos no FormIt, bem como ao inserir formas primitivas. Por exemplo, defini-la como 64 criaria um círculo completo de 64 lados ou um arco de um quarto de círculo com 16 facetas.

Esse valor também afetará a qualidade de círculos e arcos importados de arquivos SAT, bem como ao consolidar a geometria do Dynamo. É possível definir esse valor para novos esboços ou apenas para o esboço atual.

Para curvas existentes, também é possível usar o plug-in Rebuild Curve para reconstruir retroativamente um arco ou círculo **existente** com uma nova contagem de facetamento:

![](../.gitbook/assets/screen-shot-2020-01-10-at-1.20.53-pm.png)

![](../.gitbook/assets/faceting\_rebuild-curve.gif)

**Surface Faceting Quality**

Alterar essa configuração global afetará a qualidade das superfícies curvas 3D importadas de arquivos SAT e quando consolidadas do Dynamo.

Por exemplo, defini-la como 64 e, em seguida, consolidar uma esfera do Dynamo usará 64 faces em torno do equador da esfera, mais 64 facetas em cada um dos anéis que vão para os polos da esfera, o que aumenta rapidamente. Use valores maiores com cautela, pois, em alguns casos, isso pode afetar o desempenho do FormIt. Quando você tiver um resultado de alta qualidade, será possível [convertê-lo em uma malha](meshes.md) para aprimorar o desempenho.

Ao trabalhar com o Dynamo, é possível modificar a qualidade de facetamento e clicar em “Run Graph” no painel Properties sem alterar nenhum parâmetro para aproveitar as novas contagens de facetamento:

![](../.gitbook/assets/faceting\_column.gif)

Como ocorre com as curvas, é possível definir a qualidade de facetamento da superfície para novos esboços ou somente para o esboço atual.

Observe que os valores de facetamento estão limitados atualmente a múltiplos de 4, portanto, ao inserir números manualmente, o FormIt será arredondado para o múltiplo mais próximo. É possível usar os controles deslizantes e as setas para percorrer os valores aceitos.

![](../.gitbook/assets/units-+-precision.png)
