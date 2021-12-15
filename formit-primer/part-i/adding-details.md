# 1.9 –Ajout de détails

_FormIt est un outil de volume très utile, ainsi qu’un outil de modélisation très performant. Nous allons commencer à ajouter des détails au modèle Farnsworth House (Maison Farnsworth) sous la forme de portes et de meneaux pour la zone de verre. Nous aborderons ensuite d’autres outils et nous nous entraînerons à ajouter de nouvelles géométries, des calques, des matériaux, et à gérer les groupes._

_Si vous n’avez pas terminé la dernière section, téléchargez et ouvrez le fichier_ _**1.9 – Adding Details.axm**_ _à partir du dossier_ _**FormIt Primer Part 1 Datasets** (Jeux de données de la partie I du guide FormIt Primer)._

## **Création de cadres de fenêtre**

_Nous allons créer un cadre en métal de 2 po et des meneaux autour de la zone de verre. Notez que ces meneaux chevauchent intentionnellement la zone de verre._

1 – Créez un calque nommé **Glass Walls** (Murs en verre) et déplacez-y le groupe **Glass Wall** (Mur en verre).

2 – Pour faciliter la visualisation, désactivez le calque **Roof** (Toit) pour voir la zone de verre dans son intégralité.

3 – Pour créer le premier cadre de fenêtre, procédez comme suit :

1. Sur le côté ouest du bâtiment, utilisez l’outil **Rectangle \(R\)** pour dessiner une nouvelle surface directement sur la face de verre extérieure. Veillez à créer la surface en dehors du groupe **Glass Walls** (Murs en verre).
2. Sélectionnez la nouvelle face et faites-la glisser de **2 po** vers l’intérieur. Appuyez sur la touche **Échap** afin d’effacer la sélection. Le résultat final doit ressembler à l’image ci-dessous.
3. Cliquez une fois sur la face que vous venez de créer. Cliquez avec le bouton droit de la souris pour accéder au **menu contextuel** et utiliser l’outil **Décaler la face \(OF\).**

_**Remarque :**_ _si vous ne parvenez pas à sélectionner la nouvelle face, appuyez sur la touche_ _**Espace**_ _pour alterner entre les différents objets sélectionnables ou désactivez temporairement le calque_ _**Glass Walls**_ _(Murs en verre)._

![](../../.gitbook/assets/0.jpeg)

4 – Pour définir la cote de décalage, déplacez le curseur vers l’intérieur de la face, puis saisissez **2 po** pour créer un nouveau rectangle plus petit.

![](../../.gitbook/assets/1%20%289%29.png)

5 – Cliquez une fois sur le rectangle intérieur que vous venez de créer pour le sélectionner. Cliquez à nouveau et faites glisser la face vers l’intérieur du bâtiment jusqu’à ce qu’elle disparaisse. Cliquez une fois de plus pour terminer la suppression du volume central de la géométrie du cadre.

![](../../.gitbook/assets/2%20%2821%29.png)

6 – Double-cliquez pour sélectionner la géométrie que vous venez de créer et utilisez l’outil **Grouper \(G\)** pour la regrouper. Nommez le groupe **Mullion Frame – EW** (Cadre du meneau – EO). ​

7 – Créez un calque nommé **Mullion** (Meneau) et placez-y le nouveau groupe.

8 – Pour définir le matériau du cadre, procédez comme suit :

1. Dans la **palette Matériaux**, dupliquez le matériau **Metal – Brushed – Colorized** (Métal – Brossé – Coloré). Pour ce faire, cliquez dessus avec le bouton droit de la souris et choisissez **Dupliquer le matériau**.
2. Double-cliquez sur la mosaïque d’aperçu du nouveau matériau pour le modifier.
3. Renommez-le **Metal – Brushed – Gray** (Métal – Brossé – Gris).
4. Pour modifiez la couleur du matériau, cliquez sur la mosaïque **Color** (Couleur) dans la section **Textures**, puis définissez la valeur **Val:** sur **150** pour assombrir le gris.

![](../../.gitbook/assets/3%20%284%29.png)

9 – Cliquez sur **OK** pour enregistrer les modifications apportées au nouveau matériau, puis utilisez-le pour peindre le groupe **Mullion Frame – EW** (Cadre du meneau – EO). Ensuite, la **palette Propriétés** du groupe doit correspondre à ce qui est indiqué dans l’image ci-dessous :

![](../../.gitbook/assets/4.jpeg)

10 – Créez une occurrence du cadre sur le côté est à l’aide de l’un des outils suivants : **Copie rapide**, **Réseau** ou **Miroir**.

11 – Répétez les étapes ci-dessus pour les côtés nord et sud de la zone de verre. Nommez le nouveau groupe **Mullion Frame – NS** (Cadre du meneau – NS). N’oubliez pas de les peindre et de les placer sur le calque **Mullion** (Meneau).

![](../../.gitbook/assets/5%20%2816%29.png)

_**Remarque :**_ _les cadres des meneaux se chevauchent dans les coins. C’est intentionnel. Le résultat ci-dessus montre la géométrie des cadres des meneaux obtenue avec les calques_ _**Glass Wall**_ _(Mur en verre) et_ _**Column**__ (Poteau) désactivés._

**Création de meneaux**

1 – Dans le plan avec la face de verre extérieure sur le côté sud ou nord du bâtiment, tracez un **rectangle de 2 po x 10 pi-10 po \(R\)** s’étendant du bas jusqu’en haut du cadre du meneau. Ne vous inquiétez pas de la position exacte du rectangle le long du cadre, nous allons le déplacer dans le cadre dans les étapes suivantes.

![](../../.gitbook/assets/6%20%2811%29.png)

2 – Extrudez le rectangle de **2 po**, puis utilisez l’outil **Grouper \(G\)** pour le regrouper et nommez le groupe **Mullion – Vertical** (Meneau – Vertical). Placez le groupe sur le calque **Mullion** et peignez-le avec le matériau **Metal – Brushed – Grey** (Métal – Brossé – Gris).

**Localisation des meneaux**

_Vous allez maintenant définir l’emplacement du premier meneau de sorte qu’il soit centré sur le_ _**milieu**_ _d’un poteau._

1 – Pour afficher à nouveau les poteaux, activez le calque **Column** (Poteau), s’il était désactivé. Lorsque vous êtes dans la **palette Calques**, vous pouvez également désactiver les calques **Lower Terrace** (Terrasse inférieure) et **Plan Image** (Image du plan) pour faciliter les étapes suivantes.

2 – Pour déplacer le meneau vers son nouvel emplacement, procédez comme suit :

1. Cliquez une fois sur le groupe de meneaux verticaux que vous venez de créer pour le sélectionner. Utilisez l’outil **Zoom \(Z\)** pour effectuer un zoom avant et cliquez sur le **milieu** de l’arête extérieure inférieure du meneau, symbolisée par un triangle rouge**.**
2. Déplacez la géométrie horizontalement vers un poteau. Appuyez sur la touche **Maj** pour verrouiller le mouvement sur l’axe rouge \(**axe X**\). Notez qu’une fois le mouvement verrouillé, l’axe rouge devient plus épais.
3. Effectuez un zoom arrière jusqu’à ce que vous puissiez voir la base du poteau. Tout en maintenant la touche **Maj** enfoncée, cliquez sur le **milieu** à la base de la face externe du poteau. Le meneau continue de se déplacer uniquement le long de l’axe rouge \(**axe X**\), mais s’aligne sur le **milieu** sur lequel vous venez de cliquer.

![](../../.gitbook/assets/7%20%281%29.jpeg)

_**Remarque :**_ _le meneau se trouve désormais directement derrière le poteau. Désactivez le calque_ _**Column**_ _(Poteau) ou utilisez l’outil_ _**Orbite \(O\)**_ _pour visualiser le meneau._

3 – Appuyez sur la touche **Échap** pour désactiver l’outil **Déplacer**.

4 – Utilisez l’outil **Réseau \(AR\)** ou **Copie rapide** pour créer quatre \(4\) meneaux verticaux supplémentaires le long du même côté, espacés de **11 pi**. Pour savoir comment utiliser l’outil **Réseau**, reportez-vous aux chapitres précédents.

5 – Utilisez la touche Tab pour sélectionner tous les groupes de meneaux **Vertical** et les copier sur le côté opposé du bâtiment, de sorte que les cadres **nord** et **sud** possèdent des dispositions de meneaux identiques, comme illustré dans l’image suivante :

![](../../.gitbook/assets/8%20%286%29.png)

## **Création des meneaux de porte**

1 – Utilisez l’outil **Orbite \(O\)** pour faire tourner la vue en perspective en orbite jusqu’à ce que vous distinguiez le centre du cadre du meneau ouest.

2 – Comme pour la création de cadres de meneaux, dessinez un panneau de porte de **3 pi-6 po** de large avec un cadre de **2 po x 2 po**. Créez-en un groupe à l’aide de l’outil·**Grouper \(G\)** et définissez les propriétés suivantes : Nom du groupe : **Curtain Wall Door** (Porte de mur-rideau) ; calque : **Mullion** (Meneau) ; matériau : **Metal – Brushed – Grey** (Métal – Brossé – Gris).

3 – Copiez ce groupe pour créer le deuxième cadre de porte et déplacez-les de sorte qu’ils soient centrés dans le groupe **Mullion Frame – EW** (Cadre du meneau – EO), comme illustré ci-dessous.

![](../../.gitbook/assets/9.jpeg)

## **Création d’une corniche à l’aide de l’outil Balayage**

_Nous allons maintenant créer la corniche du modèle Farnsworth House (Maison Farnsworth) à l’aide de l’un des outils de modélisation avancés de FormIt, à savoir_ _**Balayage**. Pour en savoir plus sur les autres fonctionnalités de modélisation avancées, consultez le chapitre_ **2.2 –** _**Modélisation avancée** dans_ _la_ _**partie II du guide FormIt Primer.**_

_La première étape de la création d’un_ _**balayage**_ _consiste à dessiner un contour perpendiculaire à « l’extrusion » du balayage. Pour ce faire, nous allons utiliser la géométrie du toit comme guide._

1 – Activez le calque **Roof** (Toit) et effectuez un zoom avant sur l’un de ses coins.

2 – En utilisant un des côtés verticaux du toit comme référence, dessinez deux rectangles adjacents. Le premier mesure **6 po** de haut sur **4 5/8** po de large, le second **2 po x 2 po**. Supprimez la ligne séparant les deux rectangles pour créer une seule face. Le résultat doit se présenter comme suit.

![](../../.gitbook/assets/10.jpeg)

3 – Pour créer le balayage, procédez comme suit :

1. Sans sélectionner de géométrie, cliquez sur le bouton **Outils de modélisation avancés** dans la **barre d’outils Standard** et sélectionnez **Balayage \(SW\)**.
2. L’**Assistant Sélection de balayage** démarre et vous invite à **sélectionner une face \(ou des arêtes\) pour le contour de balayage**. Sélectionnez la face du contour que vous venez de créer.
3. Une fois le contour sélectionné, vous êtes invité à **sélectionner une face \(ou une arête\) pour la trajectoire de balayage, puis à cliquer sur Terminer**. Sélectionnez la face supérieure du mur. FormIt utilise automatiquement les limites de la face sélectionnée comme trajectoire de balayage et le balayage est créé tout autour du toit.

_**Remarque :**_ _si vous ne parvenez pas à sélectionner l’une des faces,_ utiliser l’outil _**Orbite \(O\)**_ _pour faire tourner la face en orbite afin de mieux la voir, puis réessayez. Vous pouvez également sélectionner toutes les arêtes du toit au lieu de la face supérieure du toit pour terminer le balayage._

![](../../.gitbook/assets/11%20%282%29.png)

4 – Pour organiser votre modèle, créez un groupe **Roof – Cornice** (Toit – Corniche), ajoutez-le au calque **Roof** (Toit) et affectez-lui le matériau **Metal – Brushed – Colorized** (Métal – Brossé – Coloré).

![](../../.gitbook/assets/12%20%281%29.png)

5 – Pour terminer, activez le calque **Column** (Poteau). Vous constaterez que le nouveau balayage coupe le haut des poteaux. Pour résoudre ce problème, modifiez l’un des groupes **Column Tall** (Grand poteau) et faites glisser la face supérieure vers le bas jusqu’à ce qu’elle s’aligne avec le bas de la corniche.

![](../../.gitbook/assets/13%20%285%29.png)

