# Plug-ins

Use o Gerenciador de plug-ins para instalar plug-ins úteis da equipe do FormIt ou saiba como [**criar seus próprios plug-ins do FormIt**](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html)**.**

#### O Gerenciador de plug-ins do FormIt

O Gerenciador de plug-ins do FormIt funciona como um hub para descobrir e gerenciar plug-ins do FormIt.

O Gerenciador de plug-ins é carregado automaticamente quando o FormIt é iniciado, desde que o FormIt tenha acesso à Internet.

É possível acessar o Gerenciador de plug-ins clicando no ícone da guia no lado direito da janela do aplicativo:

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/PluginManagerTab.PNG)

#### O Gerenciador de plug-ins categoriza diferentes tipos de plug-ins:

* **Plug-ins instalados**
* **Plug-ins recomendados**
   * Plug-ins que a equipe do FormIt recomenda para expandir a funcionalidade básica do FormIt e desbloquear novos fluxos de trabalho.
   * Os plug-ins desenvolvidos pela comunidade serão exibidos aqui após serem aprovados pela equipe do FormIt. Mais detalhes sobre esse assunto serão fornecidos no futuro.
* **Plug-ins públicos**
   * Plug-ins criados pela comunidade, mas que não foram revisados ou aprovados pela equipe do FormIt.

#### O Gerenciador de plug-ins foi projetado usando uma série de interfaces expansíveis e recolhíveis, o que facilita o gerenciamento de plug-ins e seus repositórios:

* **Gerenciar plug-ins:**
   * Clique no nome de um plug-in para ver sua descrição.
   * Alterne a opção para instalá-los ou desinstalá-los.
      * O plug-in se manifestará como uma barra de ferramentas na parte superior do aplicativo, um painel no lado direito ou uma caixa de diálogo no meio, dependendo do tipo de plug-in.
* Se você estiver [desenvolvendo seu próprio plug-in](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html), poderá adicionar sua URL privada ao campo na parte inferior e pressionar \(+\):

![Gerenciador de plug-ins do FormIt](https://formit3d.github.io/FormItExamplePlugins/docs/images/addNew.png)

#### Como os plug-ins funcionam

* Os plug-ins são baseados na Web e estão disponíveis no FormIt para Windows e no FormIt para Web.
* Os plug-ins são compostos de uma série de arquivos e pastas hospedados no GitHub ou em um servidor local ao criar seu próprio.
* Plug-ins externos \(plug-ins não hospedados localmente\) requerem uma conexão com a Internet para serem carregados inicialmente, o que significa que:
   * Os plug-ins externos não serão carregados se nenhuma conexão com a Internet for detectada quando o FormIt for iniciado.
   * Depois de carregados, alguns plug-ins externos podem continuar a trabalhar no modo off-line para essa sessão, mas outros podem ser interrompidos até que a conectividade seja restaurada.
   * Os plug-ins externos carregam o código mais recente no servidor em cada execução; portanto, sua funcionalidade será atualizada sempre que o autor enviar uma alteração.
* Os plug-ins são carregados de forma assíncrona, o que significa que a ordem dos plug-ins na interface do FormIt pode mudar em cada nova sessão.
* O Gerenciador de plug-ins usa chaves de registro no Windows para armazenar os repositórios e plug-ins instalados.
   * Se for necessário redefinir o Gerenciador de plug-ins para seus padrões, exclua a seguinte chave do registro:
      * Computer\HKEY\_CURRENT\_USER\Software\Autodesk\FormIt 360\Plugins
      * Observe que isso desinstalará todos os repositórios e plug-ins adicionados pelo usuário, redefinindo o Gerenciador de plug-ins para incluir somente os repositórios e plug-ins internos.

