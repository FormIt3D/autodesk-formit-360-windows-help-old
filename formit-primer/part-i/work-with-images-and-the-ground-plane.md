# 1.2 – Configuration d’un projet avec des images et une grille

_Pour importer des images PNG ou JPG sur le plan du sol du modèle, sélectionnez Fichier > Importer dans la barre de navigation. Toutefois, pour mieux contrôler l’échelle et la position d’une image importée, vous pouvez créer un matériau personnalisé et l’appliquer à un rectangle que vous avez dessiné vous-même._

_Si vous n’avez pas terminé la dernière section, téléchargez et ouvrez le fichier_ _**1.2 – Project Set Up with Images and Grid.axm**_ _à partir du dossier_ _**Jeux de données Partie I FormIt Primer**._

## **Calcul de la taille de l’image**

Le fichier **plan.png** fourni est l’image d’un plan imprimé sur une feuille de 24” x 26” \(ARCH D\) dont la résolution est de 3 600 pixels de large sur 2 400 pixels de haut. Grâce à l’échelle du dessin \(¼ po = 1 pi-0 po\) et les dimensions de l’image, vous pouvez calculer que 1’ = 25 pixels, ce qui signifie que l’image doit être de 144’ x 96’ lorsqu’elle est importée dans FormIt à pleine échelle.

![](../../.gitbook/assets/0%20%281%29.png)

## **Importation d’une image à l’échelle**

1 – Cliquez sur l’icône **Vue de dessus** dans la **barre de navigation flottante** pour visualiser la scène du dessus.

![](../../.gitbook/assets/1%20%281%29.png)

2 – Choisissez l’**outil Rectangle \(R\)** dans la barre d’outils Esquisse 3D.

![](../../.gitbook/assets/2%20%281%29.png)

3 – Pour créer un rectangle ayant les dimensions exactes de **144’** x **96’**, cliquez n’importe où dans l’espace de travail pour définir le point de départ, puis déplacez la souris pour afficher un aperçu et définir la première longueur de côté. Commencez à saisir une valeur de cote pour accéder à une boîte de dialogue dans laquelle vous pouvez entrer la cote exacte. Cliquez sur **OK** ou appuyez sur la touche **Entrée** pour valider la cote. Répétez la procédure pour définir la longueur du deuxième côté et terminer le rectangle.

![Saisissez la longueur du premier côté du rectangle.](../../.gitbook/assets/3%20%281%29.png)

![Saisissez la longueur du deuxième côté du rectangle.](../../.gitbook/assets/4%20%281%29.png)

![Terminez le rectangle.](../../.gitbook/assets/5%20%281%29.png)

4 – Pour créer le matériau « Plan d’étage » procédez comme suit :

1. Ouvrez la **palette Matériaux**.
2. Cliquez sur l’icône **+** pour créer un matériau.
3. Nommez le nouveau matériau « **Plan d’étage ».**
4. Sous **CARTES**, cliquez sur la mosaïque d’aperçu **Texture** et accédez au fichier **plan.png** dans le dossier **Jeu de données Maison Farnsworth > Fichiers de support > Images**. Ensuite, cliquez sur **Ouvrir**.
5. Sous **PROPRIÉTÉS**, modifiez l’échelle de l’image en saisissant **144’** dans le champ **Échelle horizontale** et **96’** dans le champ **Échelle verticale**. Il se peut que vous deviez déverrouiller les échelles horizontale et verticale \(icône de **maillons de chaîne**\) afin d’insérer des valeurs qui modifient les proportions de l’image.
6. Cochez la case **Transparence** et définissez le curseur au milieu de la plage environ. Cela permet d’aligner l’image du plan d’étage importée sur l’image satellite.
7. Cliquez sur **OK** pour terminer le matériau.

![](../../.gitbook/assets/create-1.png)

5 – Pour peindre le rectangle, procédez comme suit :

1. Dans la **palette Matériaux**, cliquez sur la mosaïque du matériau **Floor Plan** (Plan d’étage) pour peindre avec ce matériau.
2. Cliquez sur le rectangle que vous avez dessiné pour le peindre. Appuyez sur **Échap** pour quitter l’outil Pinceau.

![](../../.gitbook/assets/7.jpeg)

6 – Si le matériau apparaît à l’envers ou inversé, vous devrez peut-être inverser la face. Pour ce faire, cliquez avec le bouton droit de la souris pour accéder au **menu contextuel**, puis choisissez le bouton Inverser la face \(FF\).

![](../../.gitbook/assets/8.png)

## **Alignement de l’image importée sur l’image satellite**

1 – Pour déplacer l’image, double-cliquez d’abord sur le rectangle pour le sélectionner. Ensuite, cliquez sur le rectangle et faites-le glisser jusqu’à ce qu’il chevauche le bâtiment dans l’image satellite. Pour le moment, essayez d’aligner le rectangle le mieux possible. Nous ajusterons l’alignement ultérieurement.

![](../../.gitbook/assets/9.png)

2 – Pour faire pivoter le rectangle afin de l’aligner sur l’image Satellite, procédez comme suit :

1. Cliquez avec le bouton droit de la souris sur le rectangle pour afficher le menu contextuel. Choisissez l’outil **Rotation \(Q\).**
2. Le **widget Rotation** s’affiche au milieu du rectangle. Pour sélectionner le widget, cliquez une fois sur la poignée orange au milieu. Déplacez le widget vers le coin inférieur gauche du rectangle. Il s’accroche au coin. Cliquez pour le placer.
3. Tapez **9**. La zone de cote s’affiche. Cliquez sur **OK** pour faire pivoter le rectangle de 9 degrés dans le sens anti-horaire.

![](../../.gitbook/assets/10.png)

![](../../.gitbook/assets/11.png)

## **Alignement de la grille sur l’image satellite**

1 – Nous allons maintenant aligner la grille sur l’image satellite et le plan d’étage. Cliquez avec le bouton droit de la souris n’importe où sur le **plan du sol**, puis choisissez **Définir les axes \(SZ\)**.

![](../../.gitbook/assets/12.png)

2 – Le widget **Définir l’axe** s’affiche. Déplacez l’axe vers le coin inférieur gauche du rectangle, où il doit s’accrocher. Cliquez pour le placer.

![](../../.gitbook/assets/13.png)

3 – Cliquez sur la poignée située à l’extrémité de l’axe rouge. Déplacez la poignée vers le coin inférieur droit du rectangle de sorte que l’axe rouge soit aligné avec le bord inférieur du plan. Cliquez en dehors de l’espace pour valider cette modification.

![](../../.gitbook/assets/14.png)

4 – Pour aligner la vue sur la nouvelle grille, cliquez sur l’icône Vue de dessus dans la barre de navigation pour réinitialiser la scène.

![](../../.gitbook/assets/15.png)

5 – Pour vous assurer que les deux images du bâtiment se superposent, sélectionnez le plan pour le déplacer une fois de plus jusqu’à ce qu’il chevauche correctement l’image satellite.

![](../../.gitbook/assets/16.png)

6 – L’image satellite, le rectangle et la grille sont désormais alignés, ce qui simplifie l’esquisse 3D.

