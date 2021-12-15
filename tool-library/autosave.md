# Salvar automático

A partir da v17.3, o FormIt para Windows inclui o recurso Salvar automático, que faz uma cópia de backup do modelo do FormIt enquanto você trabalha. Esse arquivo de backup poderá ser usado para recuperar dados se o FormIt for fechado com alterações não salvas.

### Ativar/desativar Salvar automático

Encontre as opções de configuração para Salvar automático em Editar &gt; Preferências &gt; Salvar automático.

![](../.gitbook/assets/20190613-autosave.png)

O recurso Salvar automático é ativado por padrão, mas pode ser desativado completamente simplesmente ao desmarcar a caixa.

Defina o intervalo \(em minutos\) no qual Salvar automático fará uma cópia de backup inserindo um valor na caixa de número “Intervalo do salvamento automático”.

Observe que essas preferências estão no nível do aplicativo e não serão alteradas ao abrir arquivos diferentes.

### Como o recurso Salvar automático funciona

Quando Salvar automático está ativado, ele determina se o arquivo do FormIt atual tem alterações não salvas. Se houver alterações não salvas, o recurso Salvar automático criará uma cópia de backup do arquivo no intervalo especificado.

Os arquivos de backup são armazenados junto ao arquivo original e têm uma extensão de `.axmb`.

Por exemplo, se o arquivo FormIt original estiver armazenado em `C:/Users/<user>/FormIt/MyProject.axm`, o arquivo de backup poderá ser encontrado em `C:/Users/<user>/FormIt/MyProject.axmb`.

Se você iniciar uma nova sessão do FormIt sem abrir um arquivo existente, as alterações não salvas poderão ser encontradas em `C:/Users/<user>/Documents/Untitled.axmb`. Depois de salvar o novo modelo em uma localização diferente, o backup começará a adicionar alterações não salvas ao lado da nova localização, como indicado acima.

Quando você salva as alterações no arquivo original, Salvar automático exclui automaticamente o arquivo de backup, já que o backup agora é mais antigo do que o arquivo original. No entanto, se você fizer alterações subsequentes ao arquivo salvo, Salvar automático iniciará novamente o backup no intervalo especificado.

Se o arquivo de trabalho tiver alterações não salvas e você optar por fechar o FormIt e descartar as alterações, o backup de Salvar automático será excluído. No entanto, se o FormIt for forçado a fechar, por um desligamento do computador ou um erro fatal do aplicativo, o arquivo de backup de Salvar automático será mantido e poderá ser usado posteriormente para recuperar os dados.

### Trabalhar com Salvar automático ativado

O FormIt minimiza o impacto potencial do recurso Salvar automático no desempenho executando o backup em um processo separado. Com arquivos de tamanho pequeno a médio, você não deve perceber quando Salvar automático faz backup. Com arquivos muito grandes \(~400 MB ou mais\), você pode observar apenas uma pausa momentânea enquanto o FormIt copia todo o modelo e começa a fazer backup em um processo separado.

Se estiver se perguntando se Salvar automático está fazendo backup no momento, você poderá observar a barra de status na parte inferior esquerda do aplicativo para ver uma breve mensagem “Salvando automaticamente...”:

![](../.gitbook/assets/20190613-autosave-status-bar.png)

Se a barra de status estiver desativada, será possível ativá-la em Janela &gt; Barra de status ou por meio do atalho HS.

### Recuperar dados com Salvar automático

Quando você abre um arquivo FormIt com um backup disponível, o FormIt alertará que o arquivo de backup existe. Como mencionado acima, isso pode ser simplesmente devido ao fechamento do FormIt sem escolher salvar as alterações feitas nesse projeto na última vez em que ele foi editado ou devido ao fechamento inesperado do FormIt.

![](../.gitbook/assets/20190613-autosave-notification.png)

Clicar no link “Abrir?” carregará o arquivo de backup `.axmb`.

De forma similar, é possível usar Arquivo &gt; Abrir e selecionar manualmente o arquivo `.axmb` no gerenciador de arquivos para abrir um backup.

Quando o arquivo de backup estiver aberto, na próxima vez que você salvar, o FormIt exigirá que você selecione um arquivo do FormIt diferente \(`.axm`\) para substituir. Não é possível substituir os arquivos de backup do FormIt \(`.axmb`\).



