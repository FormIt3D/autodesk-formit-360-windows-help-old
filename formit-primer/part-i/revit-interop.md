# 1.15 – Trabalhar com o Revit

_Um dos recursos mais interessantes do FormIt é a capacidade de mover o modelo de um ambiente de modelagem flexível, como o FormIt, para um ambiente paramétrico avançado, como o Revit. Neste capítulo, analisaremos alguns exercícios que movem vários elementos do FormIt para o Revit e do Revit para o FormIt._

_Este capítulo usará famílias de amostra do Revit. Se você ainda não tiver isso, faça o download delas do **Conjunto de dados da Residência Farnsworth.**Se você não tiver seguido todo o tutorial até esse ponto, também será possível fazer o download e abrir o arquivo **1.15 – Working With Revit.axm** nos **Conjuntos de dados da Parte 1 do Manual do FormIt**._

_Nestes exercícios, usaremos o Revit 2022, que melhorou os recursos de interoperabilidade com o FormIt. As versões anteriores do Revit não terão parte ou nenhum dos recursos mostrados neste tutorial e terão uma interface do usuário diferente._

## Do Revit para o FormIt

### Converter famílias do Revit para uso no FormIt

Se você \(ou sua empresa\) tiver um conjunto de famílias do Revit que deseja usar no FormIt, você se interessará por esta seção, que discute como exportar em lote arquivos RFA para o FormIt.

_**Observação:**_ _As etapas abaixo mostram a interface e as etapas necessárias ao usar o Revit 2022, mas as ferramentas_ _**Converter RFA em FormIt**_ _estão disponíveis desde o Revit 2016._

1 – Abra um novo projeto ou família do Revit. Então:

1. Na faixa de opções **Complementos**, localize o painel **Conversor FormIt** e clique no botão **Converter RFA em FormIt**. A caixa de diálogo **Converter famílias do Revit** será exibida.
2. No campo **Caminho para o arquivo da família do Revit**, navegue até o local no computador onde você salvou a seguinte pasta: **Conjunto de dados da Residência Farnsworth &gt; Arquivos de suporte &gt; Revit**.
3. No campo **Caminho para o conteúdo do FormIt**, navegue para **Conjunto de dados da Residência Farnsworth &gt; Arquivos de suporte &gt; FormIt &gt; Conteúdo personalizado do FormIt**. Se você não tiver concluído o capítulo **1.11 – Importar modelos com a biblioteca de conteúdo**, talvez seja necessário criar a pasta **Conteúdo personalizado do FormIt** ou escolher outro destino.
4. Clique em **OK** para iniciar o processo de conversão.

![](../../.gitbook/assets/0%20%2823%29.png)

_**Observações:**_

* _Esse processo levará algum tempo enquanto o Revit abre o_ _**RFA**_ _no primeiro caminho e, em seguida, converte e salva com o formato_ _**AXMF**_ _para o FormIt._
* _Neste exercício, estamos convertendo apenas um único arquivo, mas é possível usar esse processo para converter em lote todos os_ _**RFAs**_ _na pasta selecionada \(incluindo os_ _**RFAs**_ _em pastas aninhadas\)._

2 – Quando o processo for concluído, volte para o FormIt. Nele, você verá o novo conteúdo ser exibido na **paleta Biblioteca de conteúdo**, dentro da pasta **FormIt &gt;** **Conteúdo personalizado do FormIt** que vinculamos anteriormente. Se você salvou os arquivos **AXMF** convertidos em uma localização diferente ou não completou o capítulo **1.11 – Importar modelos com a biblioteca de conteúdo**, talvez seja necessário adicionar essa pasta à biblioteca de conteúdo para ver seu conteúdo. Consulte o capítulo 1.11 para obter instruções sobre como adicionar pastas à biblioteca de conteúdo.

![](../../.gitbook/assets/1%20%2824%29.png)‌

**Observação**: _Nem todas as categorias do Revit são suportadas para exportação. As famílias “independentes” ou “com base no nível” são suportadas, mas as famílias “com base no hospedeiro”, como portas e janelas, não são. Massa, Gabinete, Ambiente, Mobiliário, Sistema de mobiliário, Modelo genérico, Estacionamento, Terreno e Equipamentos especiais são todos suportados. As famílias não suportadas na pasta selecionada serão simplesmente ignoradas._

## Do FormIt para o Revit

_Há duas maneiras diferentes de trazer a geometria do FormIt para o Revit. É possível importar um arquivo_ _**.axm** existente para um projeto do Revit ou para um arquivo da família do Revit, que se comportará de forma similar a um modelo importado ou arquivo CAD. Como alternativa, é possível iniciar o FormIt no Revit e trazer cada grupo do FormIt para o Revit como um elemento individual do Modelo genérico. O segundo método é abordado na **Parte II** do capítulo_ _**2.8**_ – _**Fluxos de trabalho avançados do Revit**._

### Importar a Residência Farnsworth para o Revit

1 – Para importar um arquivo do FormIt \(**.axm**\) para o Revit, inicie um novo projeto do Revit e abra a vista 3D padrão. Então:

1. Vá para a **guia Inserir** e clique no botão **Importar CAD**. A janela **Importar formatos de CAD** será aberta.
2. Certifique-se de que o menu suspenso **Arquivos do tipo** esteja definido como **Arquivos do FormIt \(\*.axm\)**.
3. Navegue até o arquivo Farnsworth **.axm** no qual você está trabalhando e selecione-o. Se você não tiver acompanhado a Parte I do Manual, também poderá abrir o arquivo **1.15 – Working With Revit.axm** na pasta **Conjunto de dados da Residência Farnsworth &gt; Arquivos do capítulo**.
4. Assegure-se de que a opção **Importar níveis do FormIt** esteja marcada.
5. Uma vez definidas as configurações, clique em **Abrir** e a geometria do FormIt será levada para o Revit como um único elemento.

![](../../.gitbook/assets/2%20%2824%29.png)

Importar um arquivo do FormIt usando o botão Importar CAD.

![](../../.gitbook/assets/3%20%2821%29.png)  
Elemento .axm importado. Observe que os níveis do modelo do FormIt também são importados para o Revit.

_De forma semelhante a outros formatos CAD, as camadas no arquivo original são importadas para o Revit. Esse recurso permite definir diferentes configurações de visibilidade para cada camada para manipular facilmente a aparência gráfica do arquivo FormIt em qualquer vista do Revit._

2 – Para ajustar a visibilidade da camada do arquivo .axm importado:

1. Vá para a janela **Visibilidade/Sobreposição de gráficos \(VG ou VV\)**, guia **Categorias importadas**, expanda o arquivo do FormIt importado, desmarque a camada **Vegetação** para desativar a camada na vista atual e clique em **OK**.
2. Altere o **Estilo visual** para **Realista** e você verá que todos os materiais do FormIt foram importados para o Revit.

![](../../.gitbook/assets/4%20%2820%29.png)

3 – Na verdade, os materiais do FormIt importados agora estarão disponíveis neste projeto do Revit, identificados com a classe do **FormIt**. Basta abrir o **Navegador de materiais** e procurar “FormIt” para ver todos eles. Agora, eles podem ser usados no projeto do Revit como qualquer outro material.

![](../../.gitbook/assets/5%20%2819%29.png)

