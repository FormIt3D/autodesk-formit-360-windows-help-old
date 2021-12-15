# Niveaux et aire

Après avoir créé une géométrie dans FormIt, vous pouvez appliquer des niveaux pour indiquer où se trouvent les élévations de sol et pour générer des calculs d’aire.

Pour découvrir le fonctionnement des calques, consultez le guide [FormIt Primer](../formit-primer/part-i/adding-floors-with-levels.md).

## Création et configuration de niveaux

Le groupe de fonctions Niveaux se trouve sur le côté droit de FormIt pour Windows :

![](../.gitbook/assets/20191217-levels-panel-1.png)

#### Création et suppression de niveaux

* Pour créer un niveau, cliquez sur le bouton « + ».
* Pour créer une série de niveaux, cliquez sur le bouton « ++ ».
   * Cela vous permet de spécifier le nombre de niveaux à créer et la distance verticale entre eux.
* Sélectionnez un ou plusieurs niveaux et cliquez sur « - » pour les supprimer.

#### Renommage, définition des élévations et renumérotation des niveaux

* Pour renommer un niveau, double-cliquez sur son nom ou cliquez avec le bouton droit de la souris, puis choisissez « Modifier le nom ».
* Pour ajuster l’élévation d’un niveau, double-cliquez sur le numéro ou cliquez avec le bouton droit de la souris, puis choisissez Modifier l’élévation.
* Cliquez sur l’icône Actualiser située en haut de la fenêtre pour renuméroter les niveaux.
   * Cette option est utile si vous avez ajouté ou supprimé des niveaux et que le schéma d’attribution de nom par défaut est désynchronisé \(c’est-à-dire Niveau 1, Niveau 2, Niveau 5\).
   * Ce bouton ignore tous les niveaux avec des noms personnalisés, mais renumérote tous les niveaux avec le nom suivant la syntaxe « Niveau 1 ».

## Application de niveaux

Pour appliquer des niveaux à un objet, vous devez sélectionner l’objet et accéder au groupe de fonctions Propriétés.

Notez que pour appliquer des niveaux à un objet, celui-ci doit être solide, sans face arrière ni problèmes d’étanchéité. [Découvrez comment vérifier si votre modèle a des problèmes d’étanchéité et de faces arrière](https://formit.autodesk.com/blog/post/repairing-solid-models).

Lorsqu’un objet solide est sélectionné dans la zone de dessin \(dans cet exemple, une coque de bâtiment simple\), le groupe de fonctions Propriétés affiche une case à cocher « Utiliser les niveaux ».

* Si des niveaux sont déjà définis pour l’esquisse FormIt \(reportez-vous aux sections ci-dessus\), la case à cocher utilise tous les niveaux qui croisent cette forme \(en ignorant ceux qui seraient trop élevés ou trop bas\).
* Si l’esquisse FormIt ne comporte pas encore de niveaux, cette case à cocher permet de créer suffisamment de niveaux par défaut\(hauteur de palier à palier de 12’\) pour couper la forme entière et applique automatiquement ces niveaux à cet objet.

![](../.gitbook/assets/20191217-properties-panel.png)

## Niveaux et Revit

Lorsque des niveaux sont appliqués à la géométrie FormIt, ils sont envoyés à Revit lors de l’utilisation du complément [FormIt](https://formit.autodesk.com/page/formit-revit).

Dans Revit, vous pouvez utiliser les niveaux FormIt pour créer des sols de volumes, des sols par face et des plans d’étage associés aux niveaux FormIt.



