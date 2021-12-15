# 1.6 – Controlar a visibilidade com camadas

_Assim como o AutoCAD e o Photoshop, as camadas no FormIt permitem gerenciar a visibilidade dos objetos no modelo. Neste capítulo, vamos criar uma camada para salvar e ocultar a massa da construção para análise futura._

_Se você não tiver concluído a última seção, faça o download e abra o arquivo_ _**1.6 – Control Visibility with Layers.axm**_ _nos_ _**Conjuntos de dados da Parte 1 do Manual do FormIt**._

## **Criar camadas**

1 – Para criar as novas camadas:

1. Vá para a **paleta Camadas** e clique no sinal **+** três vezes para criar três camadas.
2. Clique duas vezes nos nomes das camadas para renomeá-los como **Massa**, **Piso principal de construção** e **Imagem da planta.**

![](../../.gitbook/assets/0%20%2820%29.png)

_**Observação:**_ _É possível clicar em um nome de camada e arrastá-lo para cima ou para baixo para reordenar as camadas._

2 – Para atribuir o grupo **Massa – Construção principal** à camada **Massa**:

1. Na tela, selecione o grupo **Massa – Construção principal**.
2. Na **paleta Camadas**, selecione a camada **Massa** no menu suspenso “**Seleção ativada:**”. De forma similar, atribua o grupo **Imagem da planta** à camada **Imagem da planta**.

![](../../.gitbook/assets/1%20%2813%29.png)

## **Duplicar grupo**

_Agora, iniciaremos o processo de modelagem da construção em mais detalhes. A primeira etapa é criar a geometria do piso com base na massa da construção que já temos._

1 – Selecione o grupo **Massa – Construção principal** novamente. Pressione **Ctrl + C \(Copiar\)** para copiar e, em seguida, **Ctrl + Shift + V \(Colar no local\)** para colar a massa no mesmo lugar.

2 – Para desassociar a nova geometria de grupo do grupo original: clique com o botão direito do mouse para acessar o **menu de contexto** e selecione a opção **Tornar exclusivo \(MU\)**.

![](../../.gitbook/assets/2%20%2818%29.png)

_**Observação**: O novo grupo não está mais associado ao original. As alterações no novo grupo não alterarão o grupo original._

## **Criar a geometria do piso**

1 – Reatribuir a camada do grupo:

1. Clique uma vez para selecionar um dos grupos **Massa – Construção principal**.
2. Coloque o grupo na camada **Piso de construção principal** usando o menu suspenso “**Seleção ativada:**” na **paleta Camadas**.
3. Desmarque a camada **Massa** para ocultar sua geometria e mantê-la segura de quaisquer edições acidentais.

![](../../.gitbook/assets/3%20%2818%29.png)

2 – Clique duas vezes no grupo visível **Massa – Construção principal** para editá-lo. Nomeie novamente o grupo **Piso** na **paleta Propriedades**.

![](../../.gitbook/assets/4%20%2812%29.png)

3 – **Clique uma vez** na **face superior** da geometria para selecioná-la. Clique novamente e comece a arrastar a face para baixo. Quando você arrasta a face para baixo, digite **11’-2"** e a **caixa de diálogo Cota** será exibida. Clique em **OK** após inserir o valor. O piso resultante deve ter 1’ de espessura. Clique duas vezes no espaço para sair do grupo.

![](../../.gitbook/assets/5%20%2810%29.png)

