# 1.12 – Estilos visuais

_A modelagem de massas conceituais é apenas metade do que o FormIt tem a oferecer. A outra metade são gráficos bonitos que ajudam a contar uma história a um cliente ou membro da equipe. Neste capítulo, abordaremos formas de configurar os_ _**estilos visuais gráficos**_ _e criar animações._

_Se você não tiver concluído a última seção, faça o download e abra o arquivo_ _**1.12 – Visual Styles.axm**_ _nos_ _**Conjuntos de dados da Parte 1 do Manual do FormIt**._

## **Criação de uma animação**

_Nestas próximas etapas, aprenderemos a usar_ _**Cenas**_ _para criar uma animação._

1 – Para criar a primeira **Cena**:

1. Ative todas as camadas, exceto **Terreno**, **Imagem da planta** e **Massa**.
2. Certifique-se de que o modo de câmera esteja definido como **Perspectiva \(VP\)** e posicione a câmera de forma que ela esteja olhando para toda a casa ligeiramente de cima, similar à imagem abaixo.
3. Abra a **paleta Cenas**.
4. Clique no ícone **+** para criar uma nova cena com base em nossa vista atual.
5. Renomeie-a como **Vista aérea 1** e faça corresponder as outras **Propriedades da cena** ao que é mostrado na imagem abaixo.

![](../../.gitbook/assets/0%20%2817%29.png)

2 – Para criar a segunda **Cena** e, em seguida, fazer a animação entre elas:

1. Ajuste a câmera para uma nova posição para que você esteja olhando para a casa de um ângulo diferente. Crie uma nova **Cena** denominada **Vista aérea 2** usando o mesmo processo que seguimos na etapa anterior.
2. Clique no botão **Play**. Após o **Tempo de pausa** definido como **2 segundos**, a animação começará lentamente a se mover para frente e para trás entre as duas cenas. Isso continuará até que você clique no botão **Parar** para parar a animação.

![](../../.gitbook/assets/1%20%2812%29.png)

_**Observação:**_ _É possível ajustar o_ _**Tempo de pausa**, o_ _**Tempo de transição** e a_ _**Velocidade da câmera**_ _usando as configurações na parte inferior das_ _**Propriedades da cena**. Tente adicionar mais cenas e reproduzir com essas configurações para personalizar a animação._

## **Personalizar os estilos visuais**

_Agora, vamos criar outra cena com algumas configurações personalizadas de **Estilos visuais**._

1 - Primeiro, abra a **paleta Estilos visuais**. Observe que há quatro guias \(4\) na parte superior, cada uma contendo diferentes configurações visuais: **Superfícies**, **Arestas**, **Ambiente** e **Diagnósticos do modelo**. Para saber mais sobre cada guia, consulte o capítulo **Estilos visuais** na seção **Biblioteca de ferramentas**.

2 – Para personalizar algumas configurações na **guia Superfície**:

1. Ative **Sombras \(DS\)**.
2. Ative **Sombras de ambiente \(DA\)**.
3. Ative **Superfícies monotônicas \(DM\)**. Isso cria uma imagem em preto e branco abstrata sem nenhum material.

![](../../.gitbook/assets/2%20%2820%29.png)

3 – Para personalizar algumas configurações na **guia Aresta**:

* 
   1. Ajuste os controles deslizantes para clarear o contraste de **Arestas** para cerca de **30%**.
   2. Ative **Estender arestas \(DX\).**
   3. Ajuste os controles deslizantes para clarear o contraste de **Silhuetas** para **30%**.

![](../../.gitbook/assets/3%20%2811%29.png)

4 – Para personalizar algumas configurações na **guia Ambiente**:

1. Desative **Eixos**.
2. Desative **Níveis**, se estiver ativado.

![](../../.gitbook/assets/4%20%288%29.png)

5 – Crie uma nova cena chamada **Cena personalizada** para salvar essas configurações. Agora é possível alternar entre as **Cenas** para redefinir as configurações gráficas.

![](../../.gitbook/assets/5%20%286%29.png)

_**Observação**: Se você desmarcar a propriedade_ _**Câmera**_ _da nova cena, será possível usá-la para alternar somente as configurações visuais que acabamos de criar sem mover a posição da câmera. Experimente acessar uma das cenas aéreas anteriores e, em seguida, clicar duas vezes na_ _**Cena personalizada**_ _e observar o que acontece._

_**Observação:**_ _Para saber mais sobre o_ _**Diagnóstico de estilos visuais**_ _e os aplicativos avançados para_ _**Cenas**, confira a_ _**Parte II do Manual**._

