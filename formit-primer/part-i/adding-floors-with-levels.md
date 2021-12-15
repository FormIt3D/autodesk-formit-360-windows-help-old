# 1.4 – Ajout de sols avec des niveaux

_Les niveaux vous permettent de sectionner des volumes avec des références de sol individuelles et de calculer l’aire brute par volume du bâtiment. Les niveaux FormIt et leurs noms personnalisés sont convertis en niveaux Revit lorsque le fichier est converti dans Revit._

_Si vous n’avez pas terminé la dernière section, téléchargez et ouvrez le fichier **1.4 - Add Floors with Levels.axm** à partir du dossier **Jeux de données Partie I FormIt Primer**._

## **Création et personnalisation de niveaux**

1 – Pour créer des niveaux, procédez comme suit :

1. Accédez à la **palette Niveaux** dans la **barre des palettes**.
2. Cliquez sur **+** \(**Ajouter un niveau**\) quatre fois pour créer quatre niveaux.
3. Double-cliquez sur l’élévation actuelle de chaque niveau pour les modifier comme suit : **0’-0", 2’-2", 4’-6"** et **17’-8"**.
4. Double-cliquez sur le nom actuel de chaque niveau et renommez-les : **Sol, Terrasse, Bâtiment principal** et **Haut du toit.**

![](../../.gitbook/assets/0%20%2816%29.png)

_**Remarque** : vous pouvez cliquer sur l’icône_ _**++**_ _pour créer plusieurs niveaux, séparés par une distance spécifiée et uniforme. Cette option est pratique pour les bâtiments de plusieurs étages_.

## **Application de niveaux à la géométrie**

_Dans les étapes précédentes, nous avons uniquement créé des niveaux. Vous pouvez à présent appliquer ces niveaux à la géométrie que vous avez créée._

1 – Pour appliquer les niveaux à la géométrie existante, procédez comme suit :

1. Double-cliquez sur le volume supérieur de la terrasse pour le sélectionner.
2. Dans la **palette Propriétés**, cliquez sur **Utiliser les niveaux**. Cette étape permet de présélectionner tous les niveaux qui coupent actuellement la géométrie sélectionnée.
3. Trois niveaux sont maintenant appliqués à la géométrie sélectionnée \(**Bâtiment principal, Terrasse** et **Sol**\), mais dans le cadre de cet exercice, nous allons uniquement appliquer l’option **Sol**. Désactivez les cases **Bâtiment principal** et **Terrasse**.
4. Cette procédure permet de s’assurer que seule la surface coupée par le **sol** est prise en compte pour le calcul de l’aire brute, qui peut être visualisée dans le champ **Aire par niveau**.

![](../../.gitbook/assets/1%20%284%29.png)

_**Remarque** : si aucune ligne de niveau bleue ne s’affiche sur le volume, tapez_ _**DL**_ _pour utiliser l’outil_ _**Afficher les niveaux**._

![](../../.gitbook/assets/2%20%283%29.png)

