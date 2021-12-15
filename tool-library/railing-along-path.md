# Railing Along Path

## Optimisé par Dynamo

FormIt 2021 et les versions ultérieures permettent de générer un garde-corps le long d’une trajectoire et de personnaliser rapidement les résultats en place. L’exemple Railing Along Path est optimisée par Dynamo, ce qui signifie que le garde-corps obtenu est facilement configurable afin d’obtenir les résultats souhaités, et la réexécution de la logique permet de mettre à jour la géométrie en place.

![](../.gitbook/assets/railing-along-path.gif)

## Lancement de Railing Along Path

* Accédez au groupe de fonctions Dynamo dans FormIt pour Windows et vérifiez que vous vous trouvez dans le répertoire Dynamo Samples.
* Cliquez sur l’exemple Railing Along Path.
* Dans la partie gauche de l’écran, une fenêtre s’affiche et vous invite à sélectionner la trajectoire du garde-corps.
   * Vous devez sélectionner uniquement une série d’arêtes contiguës ou un groupe contenant uniquement une série d’arêtes.
   * Une fois la trajectoire sélectionnée, cliquez sur le bouton « finish » ou appuyez sur Entrée/Retour.
* Le groupe de fonctions Dynamo indique que les modifications sont en cours de traitement. Lorsque vous avez terminé, vous disposez d’un garde-corps généré par Dynamo dans un groupe FormIt, prêt à être modifié \(reportez-vous à la section ci-dessous\).

## Itération en place

Après l’exécution de l’exemple Railing Along Path, les résultats sont définis sur les valeurs par défaut. Si ces valeurs ne vous conviennent pas, vous pouvez personnaliser le garde-corps en fonction de vos besoins.

Lors de l’exécution de l’exemple Railing Along Path, un groupe contenant les résultats est créé. FormIt sélectionne alors automatiquement le groupe et affiche les options disponibles pour cette occurrence Railing Along Path.

Pour revenir aux propriétés Railing Along Path, sélectionnez le groupe et basculez vers le groupe de fonctions Properties, ou modifiez le groupe qui affiche automatiquement les propriétés.

![](../.gitbook/assets/railing-along-path-options.png)

### Railing Height

Hauteur globale du garde-corps. Ce paramètre utilise les unités FormIt actives.

### Post Spacing

Espacement entre les poteaux verticaux principaux. Ce paramètre utilise les unités FormIt actives.

### Add Posts at Path Vertices

Lorsque la valeur est définie sur **True**, les poteaux sont ajoutés à chaque sommet de la trajectoire sélectionnée et le calcul du positionnement du poteau suivant est réinitialisé à ce point.

Par exemple, si vous avez sélectionné une série de trois arêtes, un poteau s’affiche au niveau de chacun des deux points internes. Ce paramètre est utile si les sommets indiquent un changement de direction \(par exemple, montée d’escaliers ou virages\) où un poteau serait naturellement présent.

Lorsque la valeur est définie sur **False**, les poteaux sont uniquement ajoutés le long de la trajectoire à partir d’une extrémité. La distance est mesurée le long de la trajectoire et les sommets sont ignorés. Ce paramètre est utile si vous avez sélectionné un arc, une spline ou un cercle, où les sommets ne sont pas importants et que vous souhaitez que l’espacement des poteaux les ignore.

### Reverse Path Direction

Lors du calcul du positionnement des poteaux, la direction de la trajectoire choisie détermine l’extrémité de la trajectoire qui démarre la mesure de l’espacement des poteaux.

Si l’espacement des poteaux génère de l’espace sur une extrémité indésirable de la trajectoire, vous pouvez remplacer cette valeur par **True** pour inverser la courbe et commencer la mesure de l’espacement des poteaux à l’extrémité opposée.

### Post Width + Depth

Taille \(en plan\) des profils de poteaux verticaux rectangulaires. Ce paramètre utilise les unités FormIt actives.

### Handrail Width + Height

Taille \(en section\) du profil rectangulaire des mains courantes. Ce paramètre utilise les unités FormIt actives.

### Baluster Orientation

Lorsque ce paramètre est activé, les barreaux sont orientés horizontalement, comme les câbles. Si la valeur est définie sur False, les barreaux sont orientés verticalement, pour une esthétique plus traditionnelle.

### Baluster width + Depth

Taille du profil rectangulaire du barreau. Ce paramètre utilise les unités FormIt actives.

### Baluster Spacing

Quantité d’espace entre chaque barreau. Ce paramètre utilise les unités FormIt actives.

### Bottom Rail Start Height

Distance entre le bas du garde-corps et la traverse inférieure qui soutient les barreaux. Ce paramètre utilise les unités FormIt actives.

### Run

Après avoir modifié les options, cliquez sur le bouton « Run » pour exécuter le graphique Dynamo sous-jacent et générer de nouveaux résultats. Ce bouton devient bleu lorsque les paramètres ont été modifiés. Vous devez donc cliquer dessus pour afficher les mises à jour dans la géométrie finale.‌

### Edit Embedded Graph

Cliquez sur ce bouton pour lancer l’environnement de l’éditeur graphique Dynamo. Celui-ci vous permet d’afficher et de modifier le graphique Dynamo sous-jacent afin de modifier plus rapidement les paramètres et d’afficher les mises à jour en direct, ou d’inspecter/ajuster la logique.

