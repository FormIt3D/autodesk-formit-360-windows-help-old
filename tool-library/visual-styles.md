# Estilos visuais

Personalize a aparência visual do modelo, incluindo iluminação geral, estilos de aresta e efeitos ambientais. O painel Estilos visuais pode ser encontrado clicando no ícone de óculos escuros na barra de paletas:

![](../.gitbook/assets/20200307-visual-styles-icon.png)

Os estilos visuais [podem ser definidos por cena](https://windows.help.formit.autodesk.com/building-the-farnsworth-house/visual-settings), para que você possa salvar as configurações de estilo favoritas e aplicá-las a outras cenas.

## Superfícies

Gerencie a maneira como as superfícies são exibidas e sombreadas.

![](../.gitbook/assets/visual_styles%20%281%29.png)

**Brilho do ambiente** controla o brilho geral de todos os materiais na cena. Um valor de 100 significa que os materiais expostos à luz serão exibidos com todo o brilho, conforme definido na cor ou textura do material. Valores acima de 100 expõem materiais em excesso, mas podem ser úteis para modelos do SketchUp que ainda parecem escuros no FormIt. O valor padrão é 100.

**Contraste de ambiente** controla o quanto as faces mais escuras na sombra são exibidas, quando comparadas com as faces expostas à luz solar direta. Um valor de 0 significa que a iluminação não tem efeito \(todos os materiais serão exibidos com seu brilho completo, independentemente da orientação\), enquanto valores maiores farão com que as faces na sombra pareçam cada vez mais escuras. O valor padrão é 25.

Ative/desative as **Sombras** para ver como o projeto seria [sombreado na hora atual do dia](https://windows.help.formit.autodesk.com/tool-library/shadows).

**Intensidade da sombra** controla como as sombras escuras são desenhadas no plano de chão e em outras faces. Um valor de 0 tornará as sombras efetivamente invisíveis e um valor de 100 tornará as sombras pretas. O valor padrão é 20.

**Sombras de ambiente** adiciona um toque de sombreamento aos cantos para adicionar realismo ao modelo do FormIt.

**Superfícies monotônicas** desativa a cor e a textura de todos os materiais e tornam branco o ambiente ao redor. Útil para estudos de sombra ou sombreamento.

A seção Cores de superfície define as cores padrão das faces quando nenhum material é aplicado.

**Faces** é a cor padrão de todas as faces frontais do FormIt \(ou de ambos os lados, se a opção Faces posteriores estiver desmarcada\) quando nenhum material está aplicado.

A opção **Faces posteriores** é usada para exibir diferentes materiais em qualquer lado de uma única face, para modelos do SketchUp que são importados no FormIt e requerem isso. Essa opção está desmarcada por padrão, mas é marcada quando os modelos do SketchUp estão abertos ou importados. Em geometria que não seja do SketchUp, a cor especificada da Face posterior será exibida nos lados posteriores das faces.

Use as seções Efeitos de corte de seção e Efeitos de poché de efeitos para gerenciar as cores padrão de faces, linhas e o efeito poché quando a ferramenta [Plano de corte](section-planes.md) é usada.

## Planos de chão

Quando o Plano de chão é desativado no Modo de edição de grupo, a grade azul do Plano de trabalho também é desativada.

A cor do plano de trabalho também pode ser personalizada no painel Estilos visuais.

![](../.gitbook/assets/screen-shot-2020-03-30-at-1.30.16-pm.png)

## Arestas

Gerencie o estilo de exibição de todas as arestas no modelo.

![](../.gitbook/assets/edges.PNG)

**Contraste** afeta a visibilidade de todas as arestas. Um valor de 0 tornaria as arestas efetivamente invisíveis. O valor padrão é 60.

**Cor** afeta a cor de todas as arestas no modelo. O padrão é preto.

**Arestas grossas** torna todas as arestas mais grossas, incluindo as arestas de silhueta.

**Arestas de esboço** adiciona um efeito de esboço a todas as arestas para simular um efeito de desenho à mão.

**Arestas ocultas** exibe arestas ocluídas por superfícies, por outros motivos.

**Arestas estendidas** adiciona uma extensão a algumas arestas para simular um efeito desenhado à mão.

## Ambiente

Alternar a exibição de efeitos ambientais e objetos de ajuda.

![](../.gitbook/assets/environment.PNG)

**Grade** controla a exibição da grade no plano de chão, bem como a grade mostrada ao editar um Grupo. A opção “Snap à grade” será desativada quando a grade estiver desativada.

**Eixos** controla a exibição dos eixos XYZ que aparecerão na origem universal ou na origem do grupo se um grupo for editado.

**Níveis** controla a exibição de [**Níveis**](levels-and-area.md) ****definido no Painel de níveis.

**Névoa** controla a exibição da névoa que é desenhada para fazer com que a transição entre o plano de chão e o céu pareça perfeita. Desativar a Névoa resultará em uma linha de horizonte sólida em que o plano de chão \(se ativado\) encontra o céu.

**Seta de norte** controla a exibição de um pequeno widget gráfico que indica a direção do norte do projeto \(como determinado pela localização e imagens de satélite\).

Cores ambientais como céu, plano de fundo e plano de chão também podem ser personalizadas.

O céu é composto de um gradiente de cores **Inferior/plano de fundo**, **Médio** e **Superior**.

Se a opção **Céu** estiver desmarcada, somente a cor **Inferior/plano de fundo** estará visível.

## Diagnóstico

Ative/desative a exibição de ferramentas de diagnóstico.

![](../.gitbook/assets/diagnostics.PNG)

**Problemas herméticos** realça em vermelho todas as arestas que não fazem parte de um objeto sólido hermético.

**Faces posteriores** realça em vermelho todas as faces que estão voltadas para a direção errada \(todos os objetos sólidos devem ter as faces posteriores voltadas para o interior da forma sólida\).

[Saiba mais sobre como usar o diagnóstico de Vedação e faces posteriores para identificar e corrigir problemas com modelos sólidos](https://formit.autodesk.com/blog/post/repairing-solid-models).

