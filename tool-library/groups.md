# Grupos

Uma das técnicas mais básicas, porém importantes, nos fluxos de trabalho do FormIt envolve o agrupamento. Os grupos permitem que você impeça que a geometria fique unida e possibilitam configurar as relações pai/filho entre os elementos copiados para que, se você atualizar um elemento, ambos os elementos sejam atualizados. Saiba mais sobre os grupos [aqui](../formit-primer/part-i/grouping-objects.md).

É possível criar e editar os grupos de duas maneiras: no menu de contexto de um grupo selecionado ou na barra de ferramentas principal.

## Interações de grupos

Para **criar um grupo**, selecione os elementos que você deseja agrupar (isso pode incluir arestas, faces, sólidos ou outros grupos) e clique com o botão direito do mouse. Selecione a ferramenta **Grupo \(G\)** no menu de contexto. Não é possível agrupar imagens importadas e imagens de satélite.

Para **selecionar um grupo**, clique uma vez no grupo. Observe as linhas tracejadas que são exibidas ao selecionar um grupo; elas indicam o tamanho total do grupo.

Para **editar um grupo**, clique duas vezes no grupo. Isso inicia um modo de edição no qual você só pode visualizar e efetuar o snap para elementos fora do grupo atual, mas não pode selecioná-los. Também é possível ocultar os elementos fora do grupo atual usando o atalho de teclado **H**.

É possível criar **grupos dentro de grupos:** eles são chamados de **grupos aninhados** e podem ser criados dentro do modo de edição de grupo. Para mover um nível acima em grupos aninhados, clique em qualquer lugar fora dos grupos.

Para **sair do modo de edição de grupo**, clique duas vezes em qualquer lugar fora do grupo.

É possível **copiar um grupo** para criar uma relação entre o grupo original e sua cópia: se você editar qualquer grupo copiado, as mesmas alterações afetarão todos os grupos relacionados.

Para **remover a relação entre grupos copiados**, selecione o grupo ou os grupos que você deseja separar, clique com o botão direito do mouse e selecione **Tornar exclusivo** no menu de contexto. Também é possível selecionar Tornar exclusivo na barra de ferramentas Grupos.

Para **selecionar todos os grupos relacionados**, passe o cursor sobre um grupo e pressione a tecla Tab. Quando todos os grupos relacionados estiverem realçados, clique nos grupos para selecioná-los. É possível executar uma ação em todos os grupos de uma vez.

A [**Árvore de grupos**](groups-tree.md) fornece um único local para visualizar e gerenciar todos os grupos em um projeto.

## Menu de contexto Grupos e acesso à barra de ferramentas

## ![](../.gitbook/assets/grouptoolbar.png)

**Agrupar elementos**

Para criar um grupo com base no item da barra de ferramentas Grupos, selecione um ou mais elementos, selecione o ícone **Criar grupo** e, em seguida, selecione o ícone **Concluir**. Como alternativa, é possível selecionar **Criar grupo** no item da barra de ferramentas Grupos, selecionar os elementos que você deseja agrupar e selecionar o ícone **Concluir**.

Para **editar um grupo no item da barra de ferramentas Grupos**, selecione o ícone **Editar grupo** e clique no grupo que você deseja editar. Quando tiver terminado de fazer edições, selecione o ícone **Concluir**. Essa ferramenta permite selecionar o grupo específico que você deseja editar, mesmo que ele esteja profundamente aninhado.

**Para tornar um grupo exclusivo na barra de ferramentas,** selecione o ícone **Tornar exclusivo** no item da barra de ferramentas Grupos. Além disso, é possível selecionar **Tornar exclusivo** no item da barra de ferramentas Grupos, selecionar o grupo que você deseja tornar exclusivo e clicar no ícone **Concluir**.

**Para desagrupar um grupo do item da barra de ferramentas Grupos,** selecione o grupo que você deseja alterar e escolha o ícone **Desagrupar** no menu da barra de ferramentas Grupos. Isso desagrupa a seleção atual, mas não desagrupa nenhum grupo aninhado. Como alternativa, é possível selecionar **Desagrupar** na barra de ferramentas, selecionar o grupo que você deseja alterar e, em seguida, selecionar o ícone **Concluir**.

**Para desagrupar todos os grupos aninhados abaixo do grupo atualmente selecionado,** selecione um grupo com grupos aninhados e selecione **Desagrupar todos aninhados** na barra de ferramentas Grupos.

**Para desagrupar todos os grupos no modelo,** selecione a ferramenta **Desagrupar tudo** na barra de ferramentas Grupos.

## Grupos e Revit

Se você está familiarizado com as **famílias** do Revit, também está familiarizado com o conceito de grupos no FormIt. Os grupos do FormIt têm recursos que você pode usar para transferi-los de forma inteligente para o Revit.

**Categorias de grupos do FormIt**

É possível especificar as **categorias** para grupos no FormIt para que os grupos do FormIt se tornem famílias das mesmas categorias ao importá-las para o Revit. É possível atribuir categorias aos grupos do FormIt selecionando um grupo, entrando no modo **Edição de grupo** e usando o painel **Propriedades** para escolher categorias. Também é possível atribuir categorias no painel **Árvore de grupos**.

**Nomes de grupos do FormIt**

Também é possível usar o painel **Propriedades** para especificar um nome para o grupo do FormIt. Isso pode ser útil para navegar em seu próprio modelo e, ao importar o modelo para o Revit, será possível filtrar facilmente os elementos usando o nome do grupo.

Observe que os **grupos aninhados no FormIt não são importados para o Revit como grupos aninhados**. Isso impede famílias do Revit profundamente aninhadas.

