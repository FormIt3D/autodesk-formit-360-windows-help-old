# 1.8 – Création de poteaux avec un réseau

_Dans cet exercice, nous allons esquisser un élément détaillé, un poteau en I. Nous utiliserons ensuite l’outil Réseau pour créer rapidement plusieurs copies espacées de façon régulière._

_Si vous n’avez pas terminé la dernière section, téléchargez et ouvrez le fichier_ _**1.8 – Create Columns with Array.axm**_ _à partir du dossier_ _**FormIt Primer Part 1 Datasets** (Jeux de données de la partie I du guide FormIt Primer)._

## **Esquisse du profil de poteau**

1 – Pour faciliter le processus de dessin, procédez comme suit :

1. Accédez à la vue **Vue de dessus \(VT\)**.
2. Définissez le mode d’affichage **Orthogonale \(VO\)**.
3. Désactivez les calques **Main Building** **Floor** (Sol du bâtiment principal) et **Roof** (Toit). Cette étape empêche la nouvelle géométrie de s’accrocher à la géométrie existante sur ces calques.
4. Effectuez un zoom sur le coin supérieur gauche de l’image du **plan d’étage importé** afin de visualiser le poteau en détail.
5. Désactivez la fonction **Accrocher à la grille \(SG\)** \(si vous l’avez activée\). Cela vous aidera à dessiner les lignes de détail.

![](../../.gitbook/assets/0%20%2813%29.png)

_Pour dessiner le poteau, nous allons d’abord dessiner une moitié, puis lui appliquer une symétrie afin de créer rapidement l’autre moitié._

2 – Pour créer la première moitié de la poutre en I, utilisez l’outil **Ligne \(L\)** pour créer l’esquisse suivante à l’aide des cotes spécifiées. Ne vous inquiétez pas de la position exacte du poteau sur l’image du plan.

![](../../.gitbook/assets/1%20%2818%29.png)

3 – Pour appliquer une symétrie à la forme que vous venez de dessiner, procédez comme suit :

1. Double-cliquez pour sélectionner toutes les faces et arêtes de la géométrie dessinée.
2. Cliquez avec le bouton droit de la souris et choisissez l’outil **Symétrie \(MI\)**.
3. Cliquez sur la poignée orange centrale du **widget de symétrie** et placez-la dans le coin inférieur gauche de la géométrie.
4. Utilisez la flèche du bas du bouton à double flèche dans le widget afin de faire pivoter l’axe de symétrie de -90 degrés \(sens horaire\).
5. Cliquez une fois dans l’espace ou appuyez sur la touche **Échap** pour terminer le processus de symétrie. Le résultat doit ressembler à un profil de poutre en I avec une ligne au milieu. Appuyez de nouveau sur la touche **Échap** afin d’effacer la sélection.

![](../../.gitbook/assets/2%20%285%29.png)

![](../../.gitbook/assets/3%20%287%29.png)

_**Remarque** : lorsque vous ajustez le widget de symétrie, l’emplacement et l’orientation de la géométrie finale sont affichés avec la forme bleue fantôme. Vous pouvez utiliser cet aperçu comme référence pour mettre en miroir la géométrie à l’emplacement souhaité._

4 – Pour joindre les deux côtés en une seule géométrie, cliquez sur la ligne de séparation pour la sélectionner, puis appuyez sur la touche **Suppr** pour la supprimer. Les deux surfaces sont maintenant jointes en une seule surface.

5 – Pour déplacer la géométrie à son emplacement final, procédez comme suit :

1. Si les calques **Plan Image** (Image du plan) et **Roof** (Toit) sont désactivés, activez-les pour les utiliser comme guide.
2. Double-cliquez sur le profil du poteau pour sélectionner sa face et toutes ses lignes. Commencez à déplacer la sélection le long de l’axe vert \(**axe Y**\). Maintenez la touche **Maj** enfoncée et déplacez le profil jusqu’à ce qu’il soit aligné avec le toit, puis cliquez pour le placer.
3. Comme à l’étape précédente, déplacez à nouveau la géométrie, mais cette fois, verrouillez-la sur l’axe rouge \(**axe X**\).
4. Cliquez pour la placer sur la poutre en I dessinée dans le calque **Plan Image** (Image du plan). Il est possible de l’approcher, comme dans l’image suivante. La position horizontale n’a pas besoin d’être parfaite.

_**Remarque :**_ _la touche_ _**Maj**_ _permet de verrouiller le déplacement de la géométrie le long d’un seul axe, dans ce cas, l’axe vert \(**axe Y**\). Cela permet de s’assurer que le profil du poteau ne se déplace pas accidentellement vers le haut et ne s’aligne pas sur le haut du plan du toit._

![](../../.gitbook/assets/4%20%289%29.png)

## **Extrusion et mise en réseau du poteau**

1 – Pour faciliter le processus de dessin suivant, revenez au mode de vue **Perspective \(VP\)** et utilisez l’outil **Orbite \(O\)** pour positionner la caméra de manière à visualiser le profil de poutre en I du nord-ouest. Utilisez la flèche nord située dans le coin inférieur gauche pour vous aider à positionner la vue.

![](../../.gitbook/assets/5%20%281%29.jpeg)

_**Remarque :**_ _pour savoir comment naviguer dans l’esquisse, nous vous recommandons de consulter le chapitre_ _**Naviguer dans la scène**_ _._

2 – Sélectionnez la face du profil du poteau et extrudez la face jusqu’à **17 pi-8 po**.

_**Remarque :**_ _si, lors du déplacement du profil du poteau, il s’est aligné sur le toit, extrudez la face vers le bas de_ _**17 pi-8 po**   au lieu de la déplacer vers le haut._

3 – Effectuez un zoom arrière et activez le calque **Roof** (Toit) \(si désactivé\). Le haut du poteau doit s’aligner sur le haut du toit.

![](../../.gitbook/assets/6%20%289%29.png)

4 – Pour que le modèle reste organisé et ordonné, sélectionnez à nouveau la géométrie du poteau et effectuez les opérations suivantes :

1. Utilisez l’outil **Grouper \(G\)**pour créer un groupe et nommez-le **Column Tall** (Grand poteau).
2. Créez un **calque** appelé **Column** (Poteau) et ajoutez-y le groupe.
3. Importez le matériau **Metal – Brushed – Colorized** (Métal – Brossé – Coloré) et peignez le groupe avec.

![](../../.gitbook/assets/7%20%284%29.png)

_**Remarque :**_ _reportez-vous aux chapitres précédents pour plus d’informations sur les_ _**groupes**, les_ _**calques** et les_ _matériaux**.**_

4 – Cliquez sur **Échap** pour désactiver l’outil Pinceau.

## **Mise en réseau des poteaux**

1 – Accédez à la vue **Vue de dessus \(VT\)** et définissez de nouveau le mode caméra sur **Orthogonale \(VO\)**.

2 – Désactivez le calque **Roof** (Toit).

3 – Pour démarrer le processus de mise en réseau, procédez comme suit :

1. Cliquez une fois sur le groupe de poteaux pour le sélectionner. Cliquez avec le bouton droit de la souris pour afficher le **menu contextuel** et choisissez **Réseau \(AR\)**.
2. Dans la boîte de dialogue **Propriétés de réseau**, utilisez les paramètres suivants :
   * **Longueur entre les copies**
   * **Linéaire** \(modèle par défaut\)
   * **Grouper chaque solide puis créer un réseau** \(modèle par défaut\)
   * **Nombre de copies : 3**
   * Appuyez sur **OK** pour fermer la boîte de dialogue.

![](../../.gitbook/assets/8%20%283%29.png)

4 – Pour placer les nouveaux éléments, procédez comme suit :

1. Cliquez une fois sur le poteau pour démarrer le **réseau**. Déplacez le curseur le long de l’axe rouge \(**axe X**\).
2. Définissez la cote sur **22 pi**. Vous disposez à présent de **quatre** poteaux séparés de **22 pi**.
3. Appuyez sur la touche **Échap** pour effacer la sélection.

![](../../.gitbook/assets/9%20%286%29.png)

5 – Pour sélectionner tous les groupes **Tall Column** (Grand poteau) à la fois, placez le curseur de la souris sur l’un d’eux et appuyez une fois sur la touche **Tab**. Notez que les zones de contour des 4 poteaux ont été mises en surbrillance. Cliquez une fois sur le poteau sur lequel est placé le curseur de la souris pour tous les sélectionner. Cette méthode permet de sélectionner rapidement toutes les occurrences du même groupe à la fois.

6 – Générez un autre **réseau \(AR\)** pour créer les poteaux de l’autre côté du bâtiment. Cette fois, créez une copie le long de l’axe vert sur le bâtiment. Définissez la cote sur **29 pi-4 5/8 po.**

_**Remarque :**_ _29 pi 4 5/8 po = 8 5/8 po \(profondeur de poteau\) + 28 pi-8 po \(largeur du bâtiment principal\)._

7 – Pour visualiser l’ensemble du bâtiment, accédez à la vue **Vue 3D \(V3\)** et définissez-la sur **Perspective \(VP\)**. Si les calques **Main Building Floor** (Sol du bâtiment principal), **Roof** (Toit), **Lower Terrace** (Terrasse inférieure) et **Column** (Poteau) sont désactivés, activez-les.

![](../../.gitbook/assets/10%20%287%29.png)

## **Création des poteaux de la terrasse**

_Nous allons maintenant dupliquer les poteaux du bâtiment principal pour créer des versions similaires, mais plus courtes, pour la terrasse._

1 – Pour faciliter le dessin, nous vous recommandons de revenir aux paramètres **Orthogonale \(OV\)** et **Vue de dessus \(VT\)**.

2 – Pour créer les nouveaux poteaux, procédez comme suit :

1. Maintenez la touche **Ctrl** ou **Maj** enfoncée et cliquez sur les 3 poteaux les plus proches de la géométrie **Lower Terrace Floor** pour les sélectionner.
2. Cliquez une fois sur l’un des poteaux pour déplacer simultanément les trois poteaux sélectionnés. Appuyez une fois sur la touche **Ctrl** pour créer une **copie rapide**. Un aperçu fantôme de la copie s’affiche.
3. Déplacez les copies vers le bas le long de l’axe vert \(**axe Y**\) de **23 pi-4 3/8 po**. Appuyez sur la touche **Echap**.
4. Sans désélectionner, déplacez les poteaux copiés le long de l’axe rouge \(**axe X**\) de **22 pi** pour les placer dans leur position finale.
5. De nouveau, avec les 3 nouveaux poteaux toujours sélectionnés, cliquez avec le bouton droit de la souris sur l’un des poteaux copiés et choisissez **Rendre unique \(MU\)**. Ces poteaux sont maintenant associés les uns aux autres, mais uniques par rapport aux originaux.

_**Remarque :**_ _maintenez la touche_ _**Maj**_ _ou_ _**Ctrl**_ _enfoncée pour sélectionner plusieurs éléments à la fois ou supprimer des éléments de votre sélection actuelle._

![](../../.gitbook/assets/11%20%287%29.png)

3 – Modifiez le nouveau groupe de poteaux comme suit :

1. Double-cliquez pour modifier l’un des nouveaux groupes et le renommer **Column Short (Petit poteau).**
2. Ajustez la hauteur du nouveau poteau pour l’aligner sur le haut de **Lower Terrace** **Floor** (Sol de la terrasse inférieure) \(3 pi-2 po\). Pour ce faire, sélectionnez et faites glisser la face du poteau vers le bas le long de l’axe bleu \(**axe Z**\) et maintenez la touche **Maj** enfoncée. Placez le curseur n’importe où sur la face supérieure de **Lower Terrace Floor** (Sol de la terrasse inférieure) et la hauteur du poteau s’aligne automatiquement sur le calque Lower Terrace (Terrasse inférieure). Une fois la hauteur définie, cliquez pour terminer.

![](../../.gitbook/assets/12%20%284%29.png)

_**Remarque :**_ _vous pouvez vérifier la hauteur des poteaux courts à l’aide de l’outil __**Mesurer \(ME\)**__. Vous pouvez également sélectionner l’une des arêtes verticales du poteau et afficher sa longueur dans la_ _**palette Propriétés**._

4 – À l’aide des techniques que vous venez d’apprendre, copiez le poteau court le plus éloigné sur le côté opposé de **Lower Terrace Floor** (Sol de la terrasse inférieure) afin de créer le dernier poteau restant.

![](../../.gitbook/assets/13%20%284%29.png)

