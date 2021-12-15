# Gestionnaire d’annulation

FormIt intègre un système Annuler/Rétablir unique, qui peut être utilisé de deux manières différentes pour annuler une action par groupe ou de manière chronologique et globale :

* L’option Annuler/Rétablir lors de la modification d’un groupe imbriqué affecte uniquement les modifications apportées à l’intérieur de ce groupe
   * Cela signifie que vous pouvez effectuer une modification dans ce groupe, puis effectuer de nombreuses modifications dans d’autres groupes, et revenir au groupe d’origine et avoir la possibilité d’annuler la dernière modification effectuée dans ce groupe sans affecter les modifications effectuées plus récemment dans un autre groupe.
* L’option Annuler/Rétablir de l’esquisse principale \(pas lors de la modification d’un groupe\) fonctionne comme les systèmes Annuler/Rétablir classiques : la dernière modification effectuée dans **n’importe quel** groupe est annulée, selon l’ordre chronologique.

Le gestionnaire d’annulation enregistre chaque modification apportée à l’intérieur de chaque groupe dans votre modèle FormIt, y compris les modifications apportées à l’esquisse principale. Cette option est utile pour identifier visuellement les opérations annulées dans un groupe du modèle.

![](../.gitbook/assets/undo-manager.png)

Le gestionnaire d’annulation indique en **gras** l’état actuel, ainsi que les opérations antérieures à cet état et les opérations qui existaient auparavant, mais qui ont été annulées depuis.

Vous pouvez cliquer avec le bouton droit de la souris sur un état et choisir « Faire tourner vers » pour annuler ou rétablir l’opération de manière à revenir à l’état du modèle.

Les groupes qui ont été explicitement supprimés ou qui n’existent plus en raison d’une action Annuler ou Rétablir sont affichés comme \*Inactifs\*. Pour restaurer ces derniers, annulez ou rétablissez-les dans leur groupe parent jusqu’à ce qu’ils soient de nouveau disponibles.

