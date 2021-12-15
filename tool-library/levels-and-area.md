# Níveis e área

Após criar a geometria no FormIt, é possível aplicar Níveis para indicar onde as elevações do piso estão e para gerar cálculos de área.

Confira o [Manual do FormIt](../formit-primer/part-i/adding-floors-with-levels.md) para ver os níveis em ação.

## Criar e configurar níveis

Você encontrará o painel Níveis no lado direito do FormIt para Windows:

![](../.gitbook/assets/20191217-levels-panel-1.png)

#### Criar e excluir níveis

* Crie um novo nível clicando no botão “+”.
* Crie uma série de níveis clicando no botão “++”.
   * Isso permitirá especificar quantos níveis serão criados e a distância vertical entre eles.
* Selecione um ou mais níveis e clique em “-” para excluí-los.

#### Renomear, definir elevações e renumerar níveis

* Renomeie um nível clicando duas vezes no nome ou clicando com o botão direito do mouse e escolhendo “Editar nome”.
* Ajuste a elevação de um nível clicando duas vezes no número ou clicando com o botão direito do mouse e escolhendo “Editar elevação”.
* Clique no ícone Atualizar na parte superior para renumerar níveis.
   * Isso será útil se você tiver adicionado ou removido níveis e se o esquema de nomenclatura padrão não estiver sincronizado \(ou seja, Nível 1, Nível 2, Nível 5\).
   * Esse botão ignorará quaisquer níveis com nomes personalizados, mas renumerará quaisquer níveis com o nome que segue a sintaxe “Nível 1”.

## Aplicar níveis

Para aplicar níveis a um objeto, você precisará selecionar o objeto e passar para o painel Propriedades.

Observe que para aplicar níveis a um objeto, o objeto deve ser sólido, sem problemas de face posterior ou impermeável. [Saiba como verificar o modelo quanto a problemas de vedação e face posterior](https://formit.autodesk.com/blog/post/repairing-solid-models).

Com um objeto sólido selecionado na tela \(neste exemplo, uma casca de construção simples\), o painel Propriedades mostrará uma caixa de seleção “Usar níveis”.

* Se o esboço do FormIt já tiver níveis definidos \(veja acima\), marcar essa caixa usará todos os níveis que farão interseção com essa forma \(ignorando todos os que sejam muito altos ou muito baixos\).
* Se o esboço do FormIt ainda não tiver níveis, marcar essa caixa criará níveis padrão suficientes.\(Altura de 12' piso a piso\) para efetuar a interseção com toda a forma e para aplicar automaticamente esses níveis a esse objeto.

![](../.gitbook/assets/20191217-properties-panel.png)

## Níveis + Revit

Quando os níveis são aplicados à geometria do FormIt, esses níveis serão enviados para o Revit ao usar o [complemento do FormIt](https://formit.autodesk.com/page/formit-revit).

No Revit, é possível usar os níveis do FormIt para criar pisos de massa, piso por face e plantas de piso associadas aos níveis do FormIt.



