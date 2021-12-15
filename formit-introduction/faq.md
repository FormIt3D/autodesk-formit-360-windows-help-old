# Perguntas frequentes

## Sobre o FormIt

**O que é o FormIt e o FormIt Pro?**

O FormIt é um ambiente de computação, análise, visualização e modelagem 3D para projetos arquitetônicos.

Recursos do FormIt:

* Um mecanismo robusto de modelagem de sólidos, com ferramentas e fluxos de trabalho avançados e otimizados para projetos de construção
* Visualização aprimorada do ambiente para ilustrar as opções de projeto, incluindo os estados do modelo salvos com a ferramenta Cenas
* Localização, imagens de satélite e terreno 3D usando o Bing Maps
* Materiais da Biblioteca de materiais da Autodesk
* Ferramentas de visibilidade e organização de modelos, como Grupos, Camadas e Cenas
* Ferramentas de análise, incluindo:
   * Vedação e validação de faces posteriores para diagnóstico e reparação de modelos sólidos
   * Sol e sombras
   * Análise de luz solar
   * Análise de energia
* Integrações de produtos da Autodesk:
   * BIM 360 Docs
   * Insight \(Análise de energia\)
   * [Dynamo](https://formit.autodesk.com/page/formit-dynamo)
   * [Revit](https://formit.autodesk.com/page/formit-revit)
* Suporte de formatos de arquivo:
   * Abrir/Importar
      * AXM, DWG, FBX, SAT, STL, OBJ, WSM, SketchUp, Imagem
   * Exportar
      * AXM, FBX, OBJ, STL, SAT, DAE, DXF

O FormIt está disponível gratuitamente para [iOS](https://itunes.apple.com/us/app/autodesk-formit-360/id575282599?mt=8) e [na Web, com o seu navegador](https://app.formit.autodesk.com/). Uma assinatura do **FormIt Pro** é necessária para usar o [FormIt para Windows](https://formit.autodesk.com/page/download), a versão mais avançada do FormIt e repleta de recursos. A assinatura do **FormIt Pro** também oferece recursos adicionais para iOS e na Web, como análise solar e análise de energia. O **FormIt Pro** está incluído na [Autodesk AEC Collection](https://www.autodesk.com.br/collections/architecture-engineering-construction/overview).

**O que aconteceu com o FormIt para Android?**

Em um esforço para simplificar a oferta do produto FormIt, tivemos que tomar a difícil decisão de descontinuar o aplicativo para Android. Se você tiver o aplicativo instalado, ele continuará a ser executado, mas não estará mais disponível na Play Store.

**Como posso obter o FormIt?**

Para executar a versão do Windows, você deve ter acesso ao **FormIt Pro**, que faz parte da assinatura da [AEC Industry Collection](https://www.autodesk.com.br/collections/architecture-engineering-construction/overview). Portanto, se seu escritório tiver o Revit, existe uma grande chance de que você já tenha acesso ao FormIt. É possível [fazer o download do FormIt para Windows diretamente do nosso site ](https://formit.autodesk.com/page/download) ou do aplicativo para desktop da Autodesk.

Além disso, a versão da Web pode ser executada diretamente e de forma gratuita no nosso site: [http://formit.autodesk.com](http://formit.autodesk.com)

É possível fazer o download gratuito da versão para iOS na Apple App Store \(somente para iPad\).

**Se eu for estudante ou educador, poderei acessar o FormIt Pro sem custos?**

Sim! Você pode acessar a assinatura do FormIt Pro através do [portal do Autodesk Education](https://www.autodesk.com.br/education/edu-software/overview?sorting=featured&page=1).

**Como posso saber mais sobre o FormIt?**

O melhor local para iniciar é no [tutorial do Manual do FormIt](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Building-the-Farnsworth-House.html).

Existem várias seções do Manual, que variam desde níveis iniciantes \(como criar uma casa moderna completa\) a mais avançados \(como trabalhar com o Revit e o Dynamo de formas mais avançadas\).

Também temos mais de 20 vídeos em nossa série de webinars FormIt Friday. Eles podem ser encontrados no nosso [canal do YouTube](https://www.youtube.com/playlist?list=PLqumTDi1CVHM7rCHJs83Yb2FyadmuQsiH).

## Trabalhar com o Revit

**Como o FormIt funciona com o Revit?**

O FormIt é um aplicativo de projeto e esboço 3D separado, mas cria dados que podem ser convertidos facilmente para o Revit, [através do complemento do FormIt para o Revit](https://formit.autodesk.com/page/formit-revit).

**O que acontece quando faço importações para o Revit?**

A partir de 2016, o Revit é fornecido com um complemento para trabalhar com dados do FormIt. Quando você importa um arquivo AXM do FormIt para o Revit, esse complemento examina cada objeto no arquivo e recria-os no Revit usando a API. Por padrão, tudo no FormIt é categorizado como Massa.

O Conversor FormIt usa cada objeto de massa e cria uma família de massa no Revit com a [API de forma direta](https://knowledge.autodesk.com/search-result/caas/CloudHelp/cloudhelp/2016/PTB/Revit-API/files/GUID-DF7B9D4A-5A8A-4E39-8721-B7782CBD7730-htm.html).

A Forma direta é um objeto não editável usado em fluxos de trabalho IFC. Embora não seja editável, tem a vantagem específica de transferir texturas completas de material entre o FormIt e o Revit. [Confira a seguir um tutorial ](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Revit-Interop.html) que explica o fluxo de trabalho do FormIt para o Revit com mais detalhes.

**O FormIt pode criar paredes, pisos e outras famílias do sistema Revit?**

Não diretamente. Como indicado acima, por padrão, cada objeto é identificado com a categoria de Massa. Para criar paredes, pisos etc., é necessário importar o modelo para o Revit através do complemento de conversão e usar as ferramentas nativas do Revit para criar famílias do sistema com base no modelo de massa subjacente.

**O Revit pode enviar dados de volta para o FormIt?**

Sim. Para importar dados de volta para o FormIt, exporte todos ou, de preferência, _parte_ do arquivo do Revit para o formato de arquivo SAT. Normalmente, não é necessário enviar TODOS os dados do Revit para o FormIt. Em vez disso, crie uma vista filtrada no Revit que inclua somente o mínimo de dados \(por exemplo, pisos e paredes\) antes de salvar como SAT.

## Trabalhar com outros aplicativos

**Por que o formato de arquivo padrão é “.AXM”?**

O nome de código interno antes do FormIt ter sido oficialmente nomeado era XModeler; portanto, o formato de arquivo que criamos era Autodesk X Modeler (ou AXM para encurtar).

**Quais tipos de formatos 3D o FormIt pode importar?**

* Windows: AXM, DWG, FBX, OBJ, SAT, SKP, STL
* Web: OBJ, STL
* iOS: OBJ, STL, SAT

**Quais tipos de formatos o FormIt pode exportar?**

* Windows: FBX, OBJ, SAT, STL, DAE, DXF
* Web: OBJ, SAT, STL
* iOS: OBJ

**Como o FormIt funciona com o Dynamo?**

[Saiba como o FormIt e o Dynamo trabalham juntos](https://formit.autodesk.com/page/formit-dynamo) para criar fluxos de trabalho de projeto computacional.

**Como o FormIt pode ser comparado ao SketchUp?**

* Melhor [**interoperabilidade com o Revit**](../tool-library/revit.md) ***
* [**Integração do Dynamo**](../tool-library/dynamo.md) para projetos computacionais
* Ferramentas nativas para [**análise solar**](../tool-library/solar-analysis.md) e [**análise de energia realizada**](../tool-library/energy-analysis.md) pelo Autodesk Insight
* Um kernel de modelagem de sólidos mais robusto que permite operações avançadas de modelagem
* Ferramentas nativas e avançadas de modelagem, como [**Varredura, Cobertura, Elevação**](../tool-library/cover-sweep-loft.md), Sólido de deslocamento/casca e Mesclagem/Arredondamento 3D, além de [**Aplainar faces**](../tool-library/flatten-face.md)
* Vários [**planos de corte**](../tool-library/section-planes.md) visíveis
* Ferramentas de diagnóstico, como [**Exibir problemas herméticos e Exibir faces posteriores**](../tool-library/visual-styles.md)
* [**Exportação de partes do modelo**](../tool-library/export-data.md) com base no que está selecionado e/ou visível
* Exportação nativa OBJ, SAT e STL

**Posso usar os atalhos de teclado do SketchUp?**

Sim! O FormIt para Windows tem um mapa de teclado totalmente editável. Muitos atalhos comuns do SketchUp já estão incluídos por padrão, mas você pode editá-los no menu Editar &gt; Preferências.

**Posso usar meus arquivos DWG?**

Sim! O FormIt importa arquivos DWG 2D e 3D.

## Perguntas comuns de suporte

**Como posso obter suporte?**

Você pode começar com o revendedor Autodesk ou entrando em contato conosco no [Fórum do FormIt](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=pt-br). Em primeiro lugar, é melhor pesquisar se a sua pergunta já foi respondida; caso contrário, publique um novo tópico e a equipe do FormIt responderá.

**O que fazer se não conseguir efetuar login?**

* Esta [ postagem do fórum ](https://forums.autodesk.com/t5/formit-forum/having-trouble-logging-into-formit-for-windows-try-these-steps/td-p/7179572?profile.language=pt-br) aborda os problemas comuns de login
* Se você tiver um PC com um processador gráfico comutável \(GPU\), é importante garantir que o FormIt sempre use o GPU de maior desempenho. Consulte a seguir instruções para [AMD](https://community.amd.com/docs/DOC-1581#jive_content_id_Assigning_Applications_to_GPUs) e [NVIDIA](http://nvidia.custhelp.com/app/answers/detail/a_id/2615/kw/manage%203d%20settings/related/1)

**O que fazer se ocorrer uma falha na análise de energia do Insight?**

Se a análise de energia do Insight reportar um erro ou não retornar nenhum resultado, [consulte a nossa página de Análise de energia do Insight](https://formit.autodesk.com/page/formit-insight) para saber sobre dicas comuns de solução de problemas.

