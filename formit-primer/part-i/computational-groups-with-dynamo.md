# 1.10 – Groupes de calcul avec Dynamo

_Dans ce chapitre, nous allons utiliser la puissance de calcul de_ [_**Dynamo**_](http://dynamobim.org/) _pour placer et modifier des groupes flexibles liés aux exemples de graphiques Dynamo OOTB._

_Si vous n’avez pas terminé la dernière section, téléchargez et ouvrez le fichier_ _**1.10 – Computational Groups with Dynamo.axm**_ _à partir du dossier_ _**Jeux de données Partie I FormIt Primer**._

_Vous pouvez_ [_**en savoir plus ici**_](http://formit.autodesk.com/page/formit-dynamo) _sur la manière dont FormIt et Dynamo fonctionnent ensemble dans le cadre de workflows de conception informatique._

## **Création d’un escalier de terrasse inférieure**

1 – Assurez-vous que les calques **Lower Terrace, Main Building Floor** et **Plan Image** sont activés, car c’est là que vous allez ajouter l’escalier.

2 – Pour placer un groupe d’escaliers lié à l’un des exemples Dynamo OOTB, procédez comme suit :

1. Ouvrez la **palette Dynamo** dans la barre des palettes. Quelques objets Dynamo sont normalement intégrés dans le répertoire **Dynamo Samples**.
2. Cliquez sur l’exemple Dynamo **Stairs** pour l’importer dans l’espace modèle. FormIt exécute le graphique en arrière-plan et génère la géométrie de l’escalier à partir de ce graphique.
3. Déplacez le curseur sur la zone de dessin. Une fois l’escalier chargé, un aperçu fantôme de la géométrie de l’escalier se déplace à côté du curseur de la souris. Placez le curseur sur la zone de dessin, près de la terrasse, puis cliquez pour placer l’escalier. Appuyez sur la touche **Échap** afin d’effacer la sélection. Notez qu’après avoir placé l’escalier, la **palette Properties** s’ouvre automatiquement.

![](../../.gitbook/assets/0%20%2815%29.png)

_**Remarque :**_ [_**vous pouvez également lier des répertoires locaux**_](https://formit.autodesk.com/page/formit-dynamo#dynamo-getting-started) _contenant des graphiques Dynamo et exécuter vos propres graphiques Dynamo locaux de la même manière que ces exemples._

3 – Pour mettre à jour les cotes de l’escalier, procédez comme suit :

1. Une fois le groupe d’escaliers sélectionné, modifiez les entrées disponibles dans la section **INPUTS** de Dynamo, au bas de la **palette Properties**, pour les faire correspondre comme illustré ci-dessous. La plupart des groupes créés à l’aide de scripts Dynamo disposent d’une section Dynamo incluse dans leurs propriétés lorsqu’ils sont sélectionnés.
   * Add Top Landing = False
   * Add Middle Landing = False
   * Add Bottom Landing = False
   * Floor-to-Floor Height = 2.6
   * Stair Width = 12
   * Riser Height = 0.6
   * Tread Length = 1.25
   * Tread Overlap = 0.25
   * Tread Thickness = 0.25
   * Height Between Middle Landings = \(non pertinent, car aucun palier central n’est créé\)
   * Middle Landing Length = \(non pertinent, car aucun palier central n’est créé\)
   * Top/Bottom Landing Length = \(non pertinent, car aucun palier n’est créé\)
2. Cliquez sur le bouton **Run** pour exécuter à nouveau le script Dynamo à l’aide des valeurs d’entrée mises à jour.
3. Déplacez le groupe selon vos besoins pour placer l’escalier à l’emplacement approprié en fonction du calque **Plan Image**. Veillez à ne pas modifier l’élévation du groupe d’escaliers lorsque vous le déplacez. Reportez-vous aux chapitres précédents pour en savoir plus sur les astuces et techniques permettant de déplacer des éléments du modèle.

![](../../.gitbook/assets/1%20%2811%29.png)

_**‌Remarque :**_ _l’entrée_ _**Floor-to-Floor Height**_ _est une approximation de la hauteur totale de l’escalier. L’entrée_ _**Riser Height**_ _est le paramètre qui définit réellement la hauteur de l’escalier. Dans cet exemple, nous définissons l’entrée_ _**Floor-to-Floor Height**_ _sur 2.6’, mais la hauteur finale de l’escalier est de 3.0’ \(0.6’ \(**Riser Height**\) x 5 \(nombre de contremarches\)\). Étant donné que la travée entre le sol et le sommet de la terrasse est de 3’-2”, les 2” restants sont compris dans la contremarche supérieure._

## **Création d’un escalier de bâtiment principal**

_Dans les étapes précédentes, nous avons créé un escalier sans palier. Nous allons maintenant créer un escalier qui utilise un palier supérieur aligné avec le calque_ _**Main Building Floor**._

1 – Tout d’abord, copiez l’escalier que nous venons de créer :

1. Sélectionnez l’escalier existant, puis cliquez n’importe où sur le calque **Plan Image** pour lancer une commande de déplacement. FormIt utilise alors l’élévation du calque **Plan Image** comme hauteur de référence de départ pour placer la nouvelle copie. Appuyez sur la touche **Ctrl** pour effectuer une **copie rapide**.
2. Déplacez le curseur vers le bâtiment principal au-dessus de la terrasse. Notez que la face supérieure de la terrasse est maintenant le nouveau plan de référence. Cliquez pour placer le groupe.

![](../../.gitbook/assets/2%20%289%29.png)

_**Remarque :**_ _étant donné que le calque_ _**Plan Image**_ _se trouve sur le plan_ _**Ground Level**__, l’__**outil Move**_ _utilise ce plan comme référence pour son point de départ. Notez l’info-bulle_ _**On Face**_ _dans l’image ci-dessus, qui indique que la face Plan Image est sélectionnée comme référence de départ et la face supérieure du calque_ _**Lower Terrace Floor**_ _comme référence de fin._

2 – Utilisez l’outil **Make Unique \(MU\)** pour que les modifications apportées aux entrées Dynamo de cet escalier n’affectent pas l’escalier inférieur. Repositionnez le groupe à l’endroit souhaité afin qu’il soit proche de son emplacement final. Nous réglerons cela ultérieurement. Vous pouvez activer ou désactiver la visibilité du calque **Lower Terrace** afin d’afficher le plan ci-dessous et de faciliter ainsi son positionnement. Par contre, veillez à ne pas modifier l’élévation du nouvel escalier lorsque vous le déplacez.

3 – Dans la **palette Properties**, mettez à jour les **entrées Dynamo** comme illustrées ci-dessous et exécutez le script à nouveau.

* Add Top Landing = True
* Floor-to-Floor Height = 2.333
* Riser Height = 0.466
* Tread Length = 1.5
* Top/Bottom Landing Length = 2.5

![](../../.gitbook/assets/3%20%281%29.jpeg)

_**Remarque :**_ _si vous définissez l’entrée_ _**Add Bottom Landing**_ _sur_ _**True**_ _et que vous relancez le script, la face supérieure du palier inférieur doit s’aligner sur la face supérieure du calque_ _**Lower Terrace Floor**. Cela est dû au fait que, contrairement à l’escalier précédent, nous avons ajusté l’entrée_ _**Riser Height**_ _pour faire correspondre l’entrée_ _**Floor-to-Floor Height**_ _à la hauteur réelle que nous souhaitons \(2’-4” ou 2.333’\)._

2 – Repositionnez le groupe sur sa position finale. Le palier supérieur doit être aligné avec le calque **Main Building Floor**.

3 – Pour finaliser l’escalier, ajoutez le matériau **Stone - Travertine** pour qu’il corresponde aux sols. Pour en savoir plus sur l’application de matériaux, reportez-vous aux chapitres précédents.

