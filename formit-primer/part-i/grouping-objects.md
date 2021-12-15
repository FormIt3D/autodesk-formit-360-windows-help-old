# 1.5 Groupement d’objets

_Dans FormIt, les groupes fonctionnent de la même manière que les familles dans Revit et les composants dans SketchUp. Le groupement d’objets différents empêche la jonction de leur géométrie. Les copies d’un groupe agissent comme une instance de la géométrie d’origine, ce qui signifie que les modifications apportées à une copie auront une incidence sur toutes les copies._

_Si vous n’avez pas terminé la dernière section, téléchargez et ouvrez le fichier __**1.5 – Group Objects.axm**__ à partir du dossier_ _**Jeux de données Partie I FormIt Primer**._

## **Créer un groupe**

1 – Double-cliquez sur le volume de la terrasse supérieure pour le sélectionner.

2 – Cliquez avec le bouton droit de la souris, puis choisissez **Grouper \(G\)**, ou appuyez simplement sur la touche « **G** ».

![](../../.gitbook/assets/0%20%281%29.jpeg)

3 – Notez qu’après la création d’un groupe, vous êtes automatiquement placé dans l’outil Déplacer.

## **Déplacement d’un groupe**

1 – Pour faciliter le processus de modélisation, activez l’option **Accrochage à la grille \(SG\)**, si elle est désactivée.

![](../../.gitbook/assets/1%20%2814%29.png)

2 – Pour déplacer l’objet sélectionné, toujours dans la commande **Déplacer \(M\)**, cliquez une fois sur l’angle inférieur du volume. Déplacez ensuite le curseur vers le haut. Une ligne d’axe bleue (\Z\) s’affiche. Cette ligne vous aidera à déplacer l’objet vers le haut.

3 – Lorsque l’axe bleu est visible, tapez **4’-6”**. Une boîte de dialogue de cotation s’affiche ensuite. Après avoir saisi la cote, cliquez sur **OK** ou appuyez sur la touche **Entrée** du clavier. La masse entière se déplace alors vers le haut, hors du plan du sol, le long de l’**axe Z**.

_**Remarque :**_ _comme dans Revit, vous pouvez également taper_ _**4’6**,_ _**4’6”,**_ _ou_ _**4.5**. Le programme interprète la valeur comme 4\(pieds\) 6\(pouces\) lorsque vous utilisez les unités anglo-saxonnes._

![](../../.gitbook/assets/2%20%282%29.png)

## **Modification d’un groupe**

1 – Pour entrer dans le **mode de modification de groupe**, double-cliquez sur le volume.

1. Dans la **palette Propriétés**, renommez le groupe « **Volume - Bâtiment principal** ».
2. Pour enregistrer les modifications et quitter le **mode de modification de groupe**, cliquez sur l’icône en forme de coche **Terminer la modification du groupe** située dans le coin supérieur gauche de la zone de dessin ou double-cliquez dans l’espace.

![](../../.gitbook/assets/3%20%2812%29.png)

_**Remarques**:_

* _Pour en savoir plus sur les options_ _**Catégorie**_ _, reportez-vous au chapitre_ _**Utilisation de Revit**_ _._
* _Chaque groupe possède son propre historique d’annulation/de rétablissement distinct de l’ensemble du projet. Vous pouvez cliquer sur les flèches_ _**Annuler**_ _et_ _**Rétablir**_ _dans l’_ _**Assistant Modifier le groupe**_ _situé dans le coin supérieur gauche de la zone de dessin._

## **Application de niveaux à un groupe**

_**Remarque :**_ _le groupement d’une géométrie remplace les paramètres précédents que vous avez appliqués à la géométrie. De ce fait, vous devrez réappliquer les niveaux de l’exercice précédent._

1 – Pour appliquer des niveaux à un groupe, procédez comme suit :

1. Cliquez sur le groupe **Volume** **- Bâtiment principal** pour le sélectionner.
2. Accédez à la **palette Propriétés** et cochez la case **Utiliser les niveaux.**
3. Ne conservez que le niveau **Bâtiment principal** et désélectionnez tous les autres.
4. Le champ **Aire par niveau** affiche l’aire brute des objets sélectionnés. La surface de chaque **niveau** est affichée devant le nom de chaque **niveau**.
5. Si aucune ligne de niveau bleue ne traverse horizontalement l’objet, activez l’affichage des niveaux. Pour ce faire, accédez au **menu Paramètres > Style visuel > Niveaux d’affichage \(DL\).**

_**Remarque** : si aucune surface n’est indiquée pour le niveau_ _**Bâtiment principal**_ _, la géométrie ne croise peut-être pas le niveau, qui doit être situé à une hauteur de 4’-6”. Pour résoudre ce problème, repositionnez la géométrie ou la hauteur du_ _**niveau**_ _de sorte qu’ils se coupent._

![](../../.gitbook/assets/levels-to-groups.png)

2 – Pour désélectionner le groupe, appuyez sur la touche **Échap** ou cliquez une fois dans l’espace. Si aucun objet n’est sélectionné, la **palette Propriétés** indique l’aire brute de l’esquisse globale plutôt que l’aire d’un objet spécifique.

![](../../.gitbook/assets/5%20%2815%29.png)

## **Gérer les groupes**

1 – Pour afficher et gérer tous les groupes de l’esquisse, procédez comme suit :

1. Accédez à la **palette Arborescence des groupes**. Les groupes suivants s’affichent :
   * Groupe **Terrain** : groupe créé automatiquement lors de **l’importation de l’image satellite**.
   * Groupe **Volume - Bâtiment principal** : groupe de géométrie de volume de bâtiment que vous venez de créer.
   * Groupe **groupe 2** : groupe sans nom contenant l’image du plan d’étage.
2. Pour renommer le groupe **groupe 2** à l’aide de la palette Arborescence des groupes, double-cliquez sur le groupe **groupe 2**, puis tapez **Image du plan**.

![](../../.gitbook/assets/6%20%284%29.png)

_**Remarques :**_

* _Pour un modèle ordonné, nous vous recommandons de conserver des noms de groupe descriptifs._
* _Cette méthode est pratique pour gérer et modifier tous les groupes du modèle à partir d’un emplacement unique._

2 – Le groupe **Image du plan** étant toujours sélectionné, accédez à la **palette Propriétés**. Notez que le nom du groupe a également été mis à jour dans le champ **Groupe**.

![](../../.gitbook/assets/7.png)

## **Masquer le contexte du groupe**

_Cet outil permet de masquer rapidement toute la géométrie située en dehors du groupe que vous modifiez. Il est très pratique lorsque le modèle est volumineux et complexe et que d’autres géométries vous gênent._

1 – Pour isoler un groupe, procédez comme suit :

1. Double-cliquez sur sa géométrie pour modifier le groupe.
2. Accédez à **Paramètres** dans le **menu principal** et cochez la case **Masquer le contexte du groupe** ou appuyez simplement sur la touche **H** de votre clavier. Le groupe **Image du plan** disparaît.
3. Terminez la modification du groupe. Notez que le mode **Masquer le contexte de groupe \(H\)** est uniquement actif dans l’**Assistant Modifier le groupe**.
4. Pour désactiver à nouveau ce mode, appuyez simplement sur la touche **H**. Cette option peut être activée ou désactivée à tout moment, à l’intérieur ou à l’extérieur d’un groupe.

![](../../.gitbook/assets/8%20%285%29.png)

