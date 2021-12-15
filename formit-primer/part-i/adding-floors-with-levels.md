# 1.4 – Adicionar pisos com níveis

_Os níveis permitem dividir massas com dados de piso individuais e calcular a área bruta por massa de construção. Os níveis do FormIt e seus nomes personalizados serão convertidos em níveis do Revit quando o arquivo for convertido para o Revit._

_Se você não completou a última seção, faça o download e abra o arquivo **1.4 – Add Floors with Levels.axm** nos **Conjuntos de dados da Parte 1 do Manual do FormIt**._

## **Criar e personalizar níveis**

1 – Para criar níveis:

1. Vá para a **paleta Níveis** na **Barra de paletas**.
2. Clique em **+** \(**Adicionar nível**\) quatro vezes para criar quatro níveis.
3. Clique duas vezes na elevação atual de cada nível para modificá-los para: **0’-0", 2’-2", 4’-6"** e **17’-8"**.
4. Clique duas vezes no nome atual de cada nível e renomeie-os: **Solo, Terraço, Construção principal** e **Topo do telhado.**

![](../../.gitbook/assets/0%20%2816%29.png)

_**Observação**: É possível clicar no ícone __**++**__ para criar vários níveis, com uma distância especificada e uniforme separada. Isso é útil para construções com vários andares_.

## **Aplicar níveis à geometria**

_Nas etapas anteriores, só criamos níveis. Agora estamos prontos para aplicar esses níveis à geometria que criamos._

1 – Para aplicar níveis à geometria existente:

1. Selecione toda a massa do terraço superior clicando duas vezes nela.
2. Na **paleta Propriedades**, clique em **Usar níveis**. Esse passo pré-selecionará todos os níveis que atualmente efetuam a interseção com a geometria selecionada.
3. Agora a geometria atualmente selecionada tem três níveis aplicados \(**Construção principal, Terraço **e **Solo**\), mas para este exercício, queremos aplicar somente **Solo**. Desmarque **Construção principal** e **Terraço**.
4. Esse processo assegura que somente a área intersecionada pelo **Solo** seja considerada para o cálculo da área bruta, que pode ser vista no campo **Área por nível**.

![](../../.gitbook/assets/1%20%284%29.png)

_**Observação**: Se você não visualizar linhas de nível azuis na massa, digite_ _**DL**_ _para_ _**Exibir níveis**._

![](../../.gitbook/assets/2%20%283%29.png)

