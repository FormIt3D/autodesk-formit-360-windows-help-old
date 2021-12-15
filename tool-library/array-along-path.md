# Array Along Path

## Optimisé par Dynamo

FormIt 2021 et les versions ultérieures vous permettent de mettre en réseau des objets le long d’une trajectoire et de personnaliser rapidement les résultats en place. L’exemple Array Along Path est optimisé par Dynamo, ce qui signifie que le réseau est facilement configurable afin d’obtenir les résultats souhaités. De plus, la réexécution de la logique permet de mettre à jour la géométrie en place.

![](../.gitbook/assets/array-along-path.gif)

## Lancement de Array Along Path

* Accédez au groupe de fonctions Dynamo dans FormIt pour Windows et vérifiez que vous vous trouvez dans le répertoire Dynamo Samples.
* Cliquez sur l’exemple Array Along Path.
* Dans la partie gauche de l’écran, une fenêtre s’affiche et vous invite à sélectionner les objets à mettre en réseau.
   * Vous pouvez sélectionner n’importe quelle combinaison d’objets FormIt pour cette étape.
   * Une fois que vous avez sélectionné un élément, appuyez sur la flèche « suivant » située à gauche de l’écran ou appuyez sur la touche Entrée.
* Une fenêtre s’affiche et vous invite à sélectionner la trajectoire du réseau.
   * Dans ce cas, vous devez sélectionner uniquement une série d’arêtes contiguës ou un groupe contenant une série d’arêtes contiguës.
   * Une fois la trajectoire sélectionnée, cliquez sur le bouton « finish » ou appuyez sur la touche Entrée.
* Le groupe de fonctions Dynamo indique que les modifications sont en cours de traitement. Lorsque vous avez terminé, vous disposez d’un réseau généré par Dynamo dans un groupe FormIt, prêt à être modifié \(reportez-vous à la section ci-dessous\).

## Itération en place

Après avoir exécuté l’exemple Array Along Path, vous verrez que les résultats sont définis sur les valeurs par défaut. Vous devrez donc les modifier en fonction de vos besoins.

Lorsque l’exemple Array Along Path est exécuté, un nouveau groupe contenant les résultats est créé et FormIt sélectionne automatiquement le groupe et affiche les options disponibles pour cette occurrence Array Along Path.

Pour revenir aux propriétés Array Along Path, sélectionnez le groupe et basculez vers le groupe de fonctions Properties, ou modifiez le groupe qui permet d’afficher automatiquement les propriétés.

![](../.gitbook/assets/array-along-path-options.png)

### Select Object\(s\) to Array <a id="run"></a>

Cliquez sur ce bouton pour revenir à l’assistant de sélection et modifier les objets mis en réseau.

### Select Array Path

Cliquez sur ce bouton pour revenir à l’assistant de sélection et modifier la trajectoire utilisée pour calculer le réseau.

### Array Type <a id="run"></a>

Cette option permet d’activer ou de désactiver le type de réseau à calculer : By Distance ou By Number.

**Lorsque la valeur est définie sur True**, le calcul est effectué en fonction de la distance. Le nombre ci-dessous fait donc référence à la distance entre les copies.

**Lorsque la valeur est définie sur False**, le calcul est effectué en fonction du nombre de copies. Le nombre figurant sous ce champ fait donc référence au nombre de copies à ajuster le long de la trajectoire.

### Include Original Selection In Results

Lorsque la valeur est définie sur **True** :

* Les objets sélectionnés seront comptés comme l’une des nouvelles copies.
* Le groupe Dynamo qui en résulte inclut la sélection d’origine dans ses résultats. Il y aura alors du Z-fighting entre les nouvelles copies et la sélection d’origine. Vous pouvez placer la sélection d’origine sur un [calque](layers.md) et la désactiver pour la masquer.

Lorsque la valeur est définie sur **False** :

* Le réseau obtenu n’inclut **pas** la sélection d’origine. Vous obtenez donc le nombre de copies spécifié **en plus de** la sélection d’origine, et il n’aura pas de Z-fighting entre les résultats.

### Rotate Copies Along Path

Lorsque la valeur est définie sur **True**, les copies pivotent pour conserver l’orientation de l’objet d’origine par rapport à la trajectoire.

Lorsque la valeur est définie sur **False**, les copies ne sont pas pivotées, elles sont seulement déplacées.

### Use Relative Positioning Along Path

Lorsque la valeur est définie sur **True** :

* Chaque copie conserve la distance entre la trajectoire et l’objet d’origine.
* Si l’objet d’origine n’est **pas** placé à l’une des extrémités de la trajectoire, le plus grand segment restant de la trajectoire est utilisé pour le calcul du réseau.

Lorsque la valeur est définie sur **False** :

* Toute la longueur de la trajectoire est utilisée pour calculer le réseau, quel que soit l’emplacement de l’objet d’origine par rapport à la trajectoire.
* Cette option dissocie l’emplacement de la trajectoire de l’objet et permet d’utiliser l’intégralité de la trajectoire. Elle est utile si la trajectoire et l’objet ne sont pas situés près l’un de l’autre.

### Reverse Path Direction

Cette option s’applique uniquement aux trajectoires fermées. Lorsque vous utilisez l’exemple Array Along Path avec une trajectoire fermée, la direction de la courbe peut inverser de manière inattendue les résultats attendus du réseau. Définissez cette option sur **True** pour inverser la direction du réseau si les résultats sont inversés.

### Run <a id="run"></a>

Après avoir modifié les options, cliquez sur le bouton « Run » pour exécuter le graphique Dynamo sous-jacent et générer de nouveaux résultats. Ce bouton devient bleu lorsque les paramètres ont été modifiés. Vous devez donc cliquer dessus pour afficher les mises à jour dans la géométrie finale.‌

### Edit Embedded Graph <a id="edit-embedded-graph"></a>

Cliquez sur ce bouton pour lancer l’environnement de l’éditeur graphique Dynamo. Celui-ci vous permet d’afficher et de modifier le graphique Dynamo sous-jacent afin de modifier plus rapidement les paramètres et d’afficher les mises à jour en direct, ou d’inspecter/ajuster la logique.



## Sélection de la géométrie

Lors de la sélection d’objets pour l’exemple Array Along Path et d’autres graphiques Dynamo basés sur la sélection, tenez compte des points suivants :

* Vous pouvez sélectionner n’importe quelle combinaison d’objets FormIt : sommets, arêtes, faces, solides, groupes et maillages.
   * Notez que, selon l’étape, certains de ces objets ne doivent pas être sélectionnés.
   * Par exemple, lorsque vous sélectionnez la trajectoire, vous devez uniquement sélectionner une série d’arêtes contiguës ou un groupe contenant une série d’arêtes contiguës. Tout autre élément provoquera l’échec du graphique.
* Pour sélectionner tous les éléments attachés à un objet, double-cliquez sur cet objet.
* Pour sélectionner une série d’objets, utilisez la fenêtre de sélection de surfaces.
* Pour désélectionner des objets déjà sélectionnés, sélectionnez-les à nouveau.
* Au moins un objet est requis pour effectuer une étape basée sur une sélection.



