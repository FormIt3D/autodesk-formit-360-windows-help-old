# 1.5 – Agrupar objetos

_Os grupos no FormIt funcionam de forma semelhante às famílias no Revit e aos componentes no SketchUp. O agrupamento de diferentes objetos impede a união de suas geometrias. As cópias de um grupo atuam como uma instância da geometria original, o que significa que as alterações em uma cópia afetarão todas elas._

_Se você não tiver concluído a última seção, faça o download e abra o arquivo_ _**1.5 – Group Objects.axm**_ _nos_ _**Conjuntos de dados da Parte 1 do Manual do FormIt**._

## **Criar um grupo**

1 – Selecione a massa do terraço superior clicando duas vezes nela.

2 – Clique com o botão direito do mouse e selecione **Grupo \(G\)** ou simplesmente pressione “**G**”.

![](../../.gitbook/assets/0%20%281%29.jpeg)

3 – Observe que, após a criação de um Grupo, você é automaticamente colocado na ferramenta Mover.

## **Mover um grupo**

1 – Para auxiliar no processo de modelagem, ative **Snap à grade \(SG\)**, se estiver desativado.

![](../../.gitbook/assets/1%20%2814%29.png)

2 – Para começar a mover o objeto selecionado, enquanto ainda estiver no comando **Mover \(M\)**, clique uma vez em qualquer canto inferior da massa. Em seguida, mova o cursor para cima e você verá uma linha de eixo azul \(Z\). Essa linha ajudará a mover o objeto diretamente para cima.

3 – Com o eixo azul visível, digite **4'-6"** e uma caixa de diálogo de cota será exibida. Após inserir a cota, clique em **OK** ou pressione **Enter** no teclado. Isso moverá toda a massa para cima do plano de chão ao longo do **eixo Z**.

_**Observação:**_ _Da mesma forma que no Revit, você também pode digitar_ _**4’6**,_ _**4’6”**_ _ou_ _**4.5**. O programa interpretará o valor como 4\(pés\) 6\(polegadas\) ao usar unidades imperiais._

![](../../.gitbook/assets/2%20%282%29.png)

## **Editar um grupo**

1 – Para entrar no **Modo de edição de grupo**, clique duas vezes na massa.

1. Na **paleta Propriedades**, renomeie o grupo **“Massa – Construção principal”**.
2. Para salvar as alterações e sair do **Modo de edição de grupo**, clique no ícone de marca de seleção **Concluir edição de grupo** no canto superior esquerdo da tela ou clique duas vezes fora do espaço.

![](../../.gitbook/assets/3%20%2812%29.png)

_**Notas:**_

* _Para saber mais sobre as opções de_ _**Categoria**_ _, acesse o capítulo_ _**Trabalhar com o Revit**_ _._‌
* _Cada grupo tem seu próprio histórico de desfazer/refazer que é diferente do projeto geral – é possível clicar nas setas_ _**Desfazer**_ _e_ _**Refazer**_ _no_ _**Assistente de edição de grupo**_ _no canto superior esquerdo da tela._

## **Aplicar níveis a um grupo**

_**Observação:**_ _O agrupamento de uma geometria substitui as configurações anteriores que você pode ter aplicado à geometria. Por isso, você precisará reaplicar os níveis do exercício anterior._

1 – Para aplicar níveis a um grupo:

1. Clique uma vez no grupo **Massa** **– Construção principal** para selecioná-lo.
2. Vá para a **paleta Propriedades** e marque **Usar níveis.**
3. Mantenha somente o nível de **Construção principal** desmarcando todos os outros.
4. O campo **Área por nível** exibirá a área bruta dos objetos selecionados no momento. A área de cada **Nível** é exibida na frente do nome de cada **Nível**.
5. Se você não visualizar uma linha de nível azul cruzando o objeto horizontalmente, ative a exibição de nível indo para o **menu Configurações > Estilo visual > Exibir níveis \(DL\).**

_**Observação**: Se não houver nenhuma área reportada para o nível_ _**Construção principal**_ _, a geometria poderá não estar efetuando a interseção com o nível, que deverá estar na altura de 4’-6". Solucione o problema reposicionando a geometria ou a altura do_ _**Nível**_ _para que eles se intersecionem._

![](../../.gitbook/assets/levels-to-groups.png)

2 – Desmarque o Grupo pressionando **Esc** ou clicando uma vez no espaço. Sem nenhum objeto estiver selecionado, a **paleta Propriedades** informará a área bruta geral do esboço, em vez de uma área específica do objeto.

![](../../.gitbook/assets/5%20%2815%29.png)

## **Gerenciar Grupos**

1 – Para visualizar e gerenciar todos os grupos no esboço:

1. Vá para a **paleta Árvore de grupos**. Nela, você verá:
   * Grupo **Terreno** – grupo criado automaticamente quando a **imagem de satélite foi importada**.
   * **Massa – Construção principal** – o grupo de geometria de massa de construção que acabamos de criar.
   * **grupo 2** – grupo sem nome que contém a imagem da planta de piso.
2. Para renomear o **grupo 2** por meio da paleta Árvore de grupos, clique duas vezes no **grupo 2** e digite **Imagem da planta**.

![](../../.gitbook/assets/6%20%284%29.png)

_**Observações:**_

* _Para um modelo organizado, é recomendável manter os nomes de grupo descritivos._
* _Essa é uma forma útil de gerenciar e editar todos os grupos no modelo em um local._

2 – Com o grupo **Imagem da planta** ainda selecionado, navegue para a **paleta Propriedades**. Observe que o nome do grupo também foi atualizado no campo **Grupo**.

![](../../.gitbook/assets/7.png)

## **Ocultar contexto de grupo**

_Essa ferramenta é uma forma rápida de ocultar toda a geometria fora do grupo que você está editando no momento. Ela se torna muito útil sempre que você tem um modelo grande e complexo e outras geometrias atrapalham._

1 – Para isolar um grupo:

1. Clique duas vezes em sua geometria para editar o grupo.
2. Navegue até **Configurações** no **Menu principal** e selecione **Ocultar contexto de grupo** ou simplesmente pressione **H** no teclado. Observe como a **Imagem da planta** desaparece.
3. Conclua a edição do grupo. Observe que o modo **Ocultar contexto de grupo \(H\)** somente estará ativo enquanto estiver dentro do **Assistente de edição de grupo**.
4. Para desativar novamente esse modo, basta pressionar **H**. Essa opção pode ser alternada a qualquer momento, dentro ou fora de um grupo.

![](../../.gitbook/assets/8%20%285%29.png)

