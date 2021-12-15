# Análise solar e de energia

Agora que o modelo foi criado, podemos usá-lo para estudar o **impacto solar e energético** de nosso projeto. Esses recursos são incorporados ao FormIt para que seus primeiros estudos possam ser compreendidos de uma perspectiva de desempenho da construção. Esses recursos são somente do **FormIt Pro**, se você estiver seguindo no aplicativo da Web, talvez não tenha acesso.

Se você não tiver concluído a última seção, clique em Arquivo &gt; Abrir e selecione **farnsworth08.axm** na pasta Manual do FormIt.

## Sombras

Antes que qualquer uma dessas ferramentas de análise possa ser usada, é preciso [definir a localização](). Isso fornece ao FormIt acesso a dados precisos de sol, sombras e clima

1. Clique no ícone do sol na [**Barra de ferramentas de ação**](../../formit-introduction/tool-bars.md) e marque **Sombras \(DS\)**

   ![](../../.gitbook/assets/3bdf0e2a-0ad4-4aac-b6fc-5e789643b0d6.png)

2. Ajuste os controles deslizantes **Dia** e **Hora** para ver como as sombras mudam

   ![](../../.gitbook/assets/upperterracesketch_32.png)

3. Observe como o terraço coberto é sombreado durante as horas mais quentes dos meses de verão – certamente não é um acidente, mas uma questão de projeto.

**Observação**: As sombras podem causar uma diminuição no desempenho do aplicativo. Duas sugestões para mitigar isso: desative as sombras se você observar lentidão na navegação ou desative as camadas como **mobiliário** se elas não forem necessárias para estudar as sombras.

## Análise de luz solar

Como são pessoas visuais, os projetistas podem aprender e comunicar uma quantidade incrível de informações de diagramas de mapa de calor como o que estamos prestes a criar

1. Na parte inferior do [**menu Sol**](../../formit-introduction/tool-bars.md), clique no botão **Análise solar**
2. Você é colocado num modo especial em que **sombras**, **atalhos de teclado** e outras **barras de ferramentas** estão desativados
3. O comportamento de seleção é modificado no modo **Análise solar**. Você pode selecionar **por meio de grupos**, não precisa manter pressionada a tecla **Ctrl** ou **Shift** para adicionar ao seu conjunto de seleção e pode desmarcar itens clicando neles novamente. Você pode **clicar uma vez**, **clicar duas vezes** ou **selecionar em uma janela** geometria
4. Selecione as faces que você deseja estudar. **Clique uma vez** na parte superior do **telhado** e na parte superior dos **pisos**. Evite selecionar elementos pequenos, como mobiliário

   ![](../../.gitbook/assets/upperterracesketch_33.png)

5. No canto superior esquerdo da tela, localize a barra de ferramentas **Análise solar**. Clique em **Analisar**. O FormIt calculará e renderizará as superfícies. As configurações aqui podem ser ajustadas antes **e** depois da conclusão da análise

   ![](../../.gitbook/assets/solaranalysis.png)

6. A configuração **Pico do mês** mostra os valores de **pico** \(em BTU/pés²\) para o mês especificado. Isso se destina a **estudos de sombreamento**. É possível alterar a configuração do mês. Os gráficos serão atualizados instantaneamente. **Passe o cursor** sobre uma superfície analisada para obter um valor **específico**

   ![](../../.gitbook/assets/460060a0-ea3b-4095-af45-40045811be22.png)

7. A configuração **Acumulado do ano** mostra a energia **cumulativa** para o ano inteiro \(em KwH/m²\). Isso se destina a **estudos de potencial do PV**

   ![](../../.gitbook/assets/a9f61dfb-dfc9-4751-b145-b131a69c53cf.png)

8. Esses estudos de **Análise solar** podem ser exportados clicando em **Arquivo &gt; Exportar \(Ctrl + E\)** e escolhendo **Imagem** na lista à esquerda

## Análise de energia com o Insight

O FormIt integrou as mesmas ferramentas de análise do Desempenho da construção que o Revit usa. O **Insight** fornece um painel de parâmetros do sistema de construção que pode ser ajustado para refletir possíveis cenários sem exigir que você **analise novamente** a geometria do modelo. O Insight funciona melhor com a geometria de **massa** do FormIt

1. Verifique se você está conectado à Autodesk Account. Desative **todas** as camadas, **exceto** a camada de **massa**. A geometria deve ter ao menos um **Nível** aplicado
2. O FormIt só enviará a geometria **visível** para o Insight. Observe que mesmo uma **massa** simples gerará um volume de dados do **Insight**

   ![](../../.gitbook/assets/energymassing.png)

3. Clique no botão **Insight &gt; Gerar Insight**. A análise será executada na nuvem, para que você possa continuar a modelar durante o cálculo

   ![](../../.gitbook/assets/energymenu.png)

4. Quando a análise estiver concluída, clique no botão **Visualizar Insight** para ver o **Modelo de energia** e os **Fatores de desempenho** \(opcionalmente, você pode visitar o site diretamente em [**http://insight.autodesk.com**](http://insight.autodesk.com/)\)

   ![](../../.gitbook/assets/energydashboard.png)

5. No painel do Insight, é possível definir um valor \(ou um intervalo de valores\) para cada widget **Fator de desempenho** clicando no fator e arrastando os pontos azuis. A faixa será útil se você ainda não souber o sistema específico que a construção usará
6. Com cada alteração em um **Fator**, a **Faixa de custo de energia** geral (medida em USD/m²/ano\) é atualizada. É possível ver o desempenho do projeto em comparação com os benchmarks, como o **Ashrae 90.1** e o desafio do **Architecture 2030**
7. Se o projeto for alterado drasticamente, será possível reenviar a massa atualizada para o mesmo painel. Se você desejar criar um **novo** painel para o projeto atualizado, será necessário **Salvar como** no FormIt primeiro
8. Se a análise de energia não for bem-sucedida – talvez você tenha **Problemas herméticos \(DW\)** baseados na geometria, eles poderão ser revisados e corrigidos no FormIt
9. Desative a camada de **massa** e ative novamente todas as outras camadas

