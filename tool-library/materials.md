# Materiais

Faça com que os modelos do FormIt sejam exibidos com materiais que suportam reflexão, brilho e mapas de saliência.

## Painel Materiais

![](<../.gitbook/assets/materials-sample-category (2).png>)

No painel de materiais, é possível escolher entre uma grande variedade de amostras de material, navegar entre bibliotecas de materiais vinculadas e, a partir do FormIt 2021, acessar e usar o conteúdo de materiais de outros arquivos do FormIt (.AXM).

### Fontes da biblioteca de materiais

No FormIt 2021 e versões mais recentes, o painel Materiais tem uma interface de menu suspenso para escolher entre as fontes disponíveis na Biblioteca de materiais: No esboço, Amostras de material e [bibliotecas vinculadas](https://windows.help.formit.autodesk.com/tool-library/materials#linking-material-libraries).

![](<../.gitbook/assets/materials-directory-picker (1).png>)

#### No esboço

Exibe os materiais salvos no esboço atual do FormIt.

#### Amostras de material

Exibe uma lista de materiais de amostra disponíveis. Essas ofertas são armazenadas em um servidor baseado na nuvem; por isso, observe o seguinte:

* Uma conexão com a Internet é necessária ao acessar as categorias de amostras de material pela primeira vez.
* Ao acessar uma categoria pela primeira vez, ela será transferida por download e armazenada em cache no computador, para que em sessões futuras não seja necessário fazer o download.
* Ocasionalmente, a equipe do FormIt pode atualizar as ofertas na opção Amostras de material. Quando isso ocorrer, o FormIt excluirá automaticamente os itens antigos e fará o download novamente para obter as versões mais recentes.

![](../.gitbook/assets/materials-samples\_original.png)

**Bibliotecas vinculadas**

Outros diretórios e localizações aparecerão após [vincular as bibliotecas de materiais](https://windows.help.formit.autodesk.com/tool-library/materials#linking-material-libraries).

### Criar, excluir e conta-gotas

![](../.gitbook/assets/materials\_add.PNG) **Crie um novo material** definindo as configurações de cor, textura, mapa de saliência, mapa de corte, transparência e reflexão/brilho.

![](<../.gitbook/assets/materials\_delete (1) (1).PNG>) **Excluir** materiais selecionados.

![](../.gitbook/assets/materials\_eyedropper.PNG) Use a ferramenta **Conta-gotas** em um material pintado na cena e imediatamente comece a pintar com ele.

* Clique na ferramenta Conta-gotas e, em seguida, clique em uma face pintada com um material
* O material encontrado na face será realçado no painel e a ferramenta Pincel ficará ativa com o material carregado.

### Atualizar, vincular bibliotecas e eliminar itens não usados

\*\*\*\*![](../.gitbook/assets/materials-link.png)**Vincule bibliotecas de materiais** de diretórios locais. Os diretórios com arquivos JPG, PNG ou AXM (FormIt) exibirão conteúdos. Consulte [Vincular bibliotecas de materiais](https://windows.help.formit.autodesk.com/tool-library/materials#linking-material-libraries) para obter mais informações.

![](../.gitbook/assets/materials-refresh.png) **Atualize** o diretório atual. Somente ativado ao visualizar um diretório vinculado localmente (e não em esboço ou amostras de material).

![](../.gitbook/assets/materials-purge.png) Os **materiais não usados são eliminados** do esboço atual do FormIt.

Os materiais não usados podem se acumular naturalmente através do processo de iteração, mas poderão provocar um acréscimo significativo no tamanho do arquivo se usarem texturas de alta qualidade.

Os materiais não usados aparecem com um nome em cinza na lista No esboço.

Clique na ferramenta Eliminar itens não utilizados para excluir todos os materiais não usados. Você verá um aviso primeiro, para que possa cancelar se mudar de ideia. Esse botão somente está ativado na lista No esboço.

### Vincular bibliotecas de materiais

O FormIt 2021 e as versões mais recentes oferecem a capacidade de vincular o painel Materiais a diretórios locais (bibliotecas) que contêm conteúdo de materiais, incluindo pastas de JPGs, PNGs e/ou arquivos do FormIt:

![](../.gitbook/assets/materials-axms.png)

![Visualize materiais individuais de um arquivo do FormIt ou arquivos JPG/PNG em um diretório.](../.gitbook/assets/materials-axm-content.png)

* Os **arquivos JPG/PNG** serão exibidos como materiais, que podem ser pintados diretamente no esboço atual do FormIt.
   * Ao clicar em uma miniatura, o arquivo de imagem é convertido em um material do FormIt em tempo real e copiado para o esboço atual.
   * O FormIt retornará ao diretório “No esboço” para ver o material que você acabou de copiar para o esboço.
* **Os arquivos do FormIt (\*.axm)** serão exibidos como pastas com um ícone do FormIt.
   * Ao clicar nas pastas de arquivos do FormIt, serão exibidos todos os materiais do FormIt salvos no arquivo.
   * Observe que o FormIt deve carregar parte do arquivo para obter o conteúdo dos materiais; portanto, arquivos maiores podem levar mais tempo para exibir os materiais no painel.

### Interações de materiais

**Pinte um material** clicando uma vez na miniatura. Você será direcionado para a ferramenta Pincel, onde pode passar o cursor do mouse sobre a geometria na tela do FormIt e clicar em faces ou grupos para pintá-los.

Quando estiver na ferramenta Pincel:

* Pinte faces e grupos clicando uma vez.
   * Ao pintar grupos, o Material será colocado em cascata na geometria aninhada e cobrirá qualquer superfície ou grupo pintado com o Material padrão.
* Pinte sólidos inteiros clicando duas vezes em uma face para selecionar tudo o que estiver anexado.

Também é possível selecionar primeiro faces e grupos e, em seguida, clicar uma vez em uma miniatura de material para pintar a seleção com esse material.

**Edite um material** clicando duas vezes na miniatura, que abrirá o Editor de material (veja abaixo).

**Renomeie um material** clicando duas vezes no nome.

**Identifique um material** pintado na geometria ao selecioná-lo e procurar o realce e o ícone que indicam quais materiais foram pintados na geometria selecionada.

![](../.gitbook/assets/material\_selected.png)

O **material padrão** pode ser usado para “limpar” com eficácia uma face ou um grupo de qualquer material. Qualquer geometria não pintada com um material é pintada implicitamente com o material padrão.

### Gerenciamento de listas

Ajuste o tamanho das miniaturas ajustando a largura da coluna (clique e arraste a linha vertical para a direita de “Material”).

Filtre materiais específicos digitando na barra “Filtro...”.

Os materiais com nomes que são exibidos em cinza correspondem a materiais que não são usados no esboço atual.

## Criar e editar materiais

![](<../.gitbook/assets/materials-editor (1).png>)

Quando você cria ou edita um material, verá a caixa de diálogo Editor de material, onde é possível personalizar:

* **Cor**
* **Mapas de imagem**
   * Clique na miniatura para selecionar um novo mapa.
   * Clique no ícone Salvar para salvar o mapa para edição em outro aplicativo.
   * Clique no ícone Excluir para excluir o mapa desse material.
      * **Textura de um arquivo de imagem**
         * JPG ou PNG
      * **Mapa de saliência de um arquivo de imagem**
         * JPG recomendado
         * Ótimo para adicionar efeitos de profundidade aos materiais.
         * É possível usar freeware, como o ShaderMap, para gerar mapas de saliência com uma determinada textura.
      * **Mapa de corte de um arquivo de imagem**
         * PNG
         * Ótimo para materiais que têm transparência seletiva, como cercas de chainlink ou painéis perfurados.
* **Nome**
* **Escala horizontal e vertical**
   * Quando essa opção está ativada, o botão Bloquear aspecto garante que as escalas horizontal e vertical respeitem a relação de aspecto da textura.
   * Estique um material ajustando a escala horizontal independentemente da escala vertical.
   * É possível substituir as escalas horizontal e vertical por face, usando a ferramenta Ajustar colocação do material (veja abaixo).
* **Transparência**, **Reflexão** e **Brilho**

## Ajustar a colocação do material

Ao pintar um material em uma face, o FormIt faz a melhor estimativa sobre a melhor orientação:

* As faces verticais serão orientadas com a parte superior da textura orientada ao longo do eixo Z.
* As faces horizontais serão orientadas com a textura no sentido do comprimento do lado mais longo da face.

Use a ferramenta **Ajustar colocação do material** para substituir o posicionamento padrão do material, bem como a escala do material em faces específicas:

* Selecione uma face ou faces pintadas com um material
   * Se a face herdar material de seu grupo principal, será necessário pintar a face diretamente em primeiro lugar.
* Acesse a ferramenta Ajustar colocação do material através do atalho MP ou no menu de contexto do botão direito do mouse:

![](../.gitbook/assets/adjust-material-placement.PNG)

Use os controles na tela para mover, rotacionar e dimensionar de forma interativa as texturas de material diretamente na face:

![](../.gitbook/assets/materialplacement.gif)

![](../.gitbook/assets/adjust-material-placement.gif)

Para redefinir qualquer uma das alterações na colocação do material, basta pintar a face novamente com o material original, no painel Materiais.

## Conversão de material para o Revit

Os materiais serão transferidos para o Revit ao usar o [complemento do FormIt](https://formit.autodesk.com/page/formit-revit) para o Revit 2018 ou versões mais recentes.
