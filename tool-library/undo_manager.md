# Gerenciador de desfazer

O FormIt apresenta um sistema único de Desfazer/Refazer, que pode ser usado de duas maneiras diferentes para desfazer por grupo ou cronologicamente e globalmente:

* Desfazer/Refazer ao editar um grupo aninhado somente afetará as alterações dentro desse grupo.
   * Isso significa que você pode fazer uma alteração nesse grupo, fazer muitas alterações em outros grupos e retornar ao grupo original e ter a opção de Desfazer a última alteração feita nesse grupo sem afetar as alterações feitas mais recentemente, em outros lugares.
* Desfazer/Refazer no esboço principal \(não ao editar um grupo\) age como os sistemas tradicionais Desfazer/Refazer: a última alteração feita em **qualquer** grupo será desfeita, com base na ordem cronológica.

O Gerenciador de desfazer registra todas as alterações dentro de cada grupo no modelo FormIt, incluindo as alterações feitas no esboço principal. Isso é útil para entender visualmente quais operações foram desfeitas em qualquer grupo no modelo.

![](../.gitbook/assets/undo-manager.png)

O Gerenciador de desfazer indicará em **negrito** o estado atual, bem como todas as operações antes desse estado e todas as operações que existissem antes, mas que tenham sido desfeitas desde então.

É possível clicar com o botão direito do mouse em um estado e selecionar “Rolar para” para efetivamente desfazer ou refazer, conforme necessário, para retornar para o estado do modelo.

Os grupos que foram explicitamente excluídos ou que não existem mais devido a uma ação Desfazer ou Refazer são mostrados como \*Inativos\*. Eles podem ser restaurados ao desfazer ou refazer dentro de seu grupo pai até que eles voltem a existir.

