# 1.11 – Importation de modèles avec la bibliothèque de contenu

_Dans ce chapitre, nous allons importer des modèles SketchUp existants et utiliser la bibliothèque de contenu FormIt afin de placer des familles OOTB qui ont été converties à partir de Revit. Notez que lorsque vous ouvrez des fichiers SKP avec FormIt, ils sont fournis avec des matériaux, des groupes et des composants, des calques \(étiquettes\) et des scènes intacts. Un nettoyage peut être nécessaire pour que vos projets restent bien organisés et ordonnés._

_Dans ce chapitre, nous allons utiliser des fichiers du dossier_ **Farnsworth House Data Set > Supporting Files** (Jeu de données Maison Farnsworth > Fichiers de support). Si ce n’est pas déjà fait, veillez à télécharger les dossiers requis ou l’intégralité du jeu de données à partir du dossier _**FormIt Primer Part 1 Datasets** (Jeux de données de la partie I du guide FormIt Primer)._

## **Importation et modification de fichiers SKP**

_Nous allons tout d’abord ajouter un élément de contenu téléchargé à votre bibliothèque de contenu personnel_. Notez que dans cet exercice, nous allons utiliser uniquement des fichiers SKP. Pour en savoir plus sur l’ouverture/l’importation d’autres formats de fichier, reportez-vous à [**ce billet de blog sur les fonctionnalités de FormIt 2021.2**](https://formit.autodesk.com/blog/post/formit-2021-2-and-new-revit-add-in-now-available) et **ce chapitre sur les ** **formats de fichier d’importation et d’exportation étendus**.

1 – Assurez-vous d’**enregistrer \(Ctrl + S\)** tout travail ouvert, puis lancez une nouvelle esquisse FormIt. Pour ce faire, vous pouvez procéder comme suit :

1. Ouvrez une autre session sur FormIt dans une nouvelle fenêtre en cliquant avec le bouton droit de la souris sur l’icône FormIt dans la **barre des tâches de Windows** et en cliquant sur l’icône **FormIt**. Une nouvelle fenêtre FormIt s’ouvre, vous permettant d’exécuter deux sessions FormIt côte à côte.
2. OU, après l’enregistrement, lancez une **nouvelle esquisse \(Ctrl + N\)** à partir de la liste déroulante **Fichier** dans la barre du **menu principal**.

![](../../.gitbook/assets/0%20%2819%29.png)

2 – Créez un dossier appelé **Custom FormIt Content** (Contenu Formit personnalisé) dans le dossier **Farnsworth House Data Set > Supporting Files > FormIt** (Jeu de données Maison Farnsworth > Fichiers de support > FormIt) du dossier _**Farnsworth House Data Set** (Jeu de données Maison Farnsworth)._

3 – **Enregistrez \(Ctrl + S\)** votre nouvelle esquisse dans ce dossier. Nous vous recommandons de le nommer comme suit : **Ottoman – Barcelona\_Mies.axm**

4 – Dans le nouveau fichier FormIt vide, procédez comme suit :

1. **Importez un fichier local \(Ctrl + I\)** en sélectionnant **Importer > Localement...** dans la liste déroulante **Fichier** de la barre du **menu principal**.
2. Choisissez : **Ottoman – Barcelona\_Mies.skp** à partir de **Farnsworth House Data Set > Supporting Files > SketchUp**(Jeu de données Maison Farnsworth > Fichiers de support >SketchUp) et cliquez sur **Ouvrir**.

_**Remarque :**_ _si le fichier_ _**Ottoman – Barcelona\_Mise.skp**n’est pas visible, vérifiez que la liste déroulante des formats de fichier située dans la partie inférieure droite est définie sur_ _**Tous les formats pris en charge**._

![](../../.gitbook/assets/1%20%287%29.png)

5 – Renommez le groupe importé **Ottoman – Barcelona\_Mies**.

6 – Lorsque nous importerons ce modèle dans notre fichier Farnsworth House (Maison Farnsworth), il sera placé à l’aide du point d’**origine** de ce fichier. Pour contrôler le point de placement l, il faut déplacer le groupe **Ottoman – Barcelona\_Mies** de sorte qu’un de ses coins soit situé à l’**origine**. Pour ce faire :

1. Assurez-vous que l’option **Accrocher à la grille \(SG\)** est activée. Utilisez l’outil **Ligne \(L\)** pour tracer une ligne de référence à partir de l’**origine** \(les axes X, Y et Z se coupent\). Cliquez n’importe où pour placer le deuxième point.
2. Sélectionnez le groupe Ottoman et lancez l’option Déplacer en cliquant une fois sur le coin inférieur gauche de son pied, comme illustré. _Pour en savoir plus sur le déplacement des objets, reportez-vous aux chapitres précédents._
3. Déplacez le groupe vers l’**origine**, en l’accrochant au point de départ de la ligne de référence que vous venez de dessiner.
4. Supprimez la ligne de référence.

![](../../.gitbook/assets/2%20%2817%29.png)

7 – Nous vous recommandons de supprimer les calques indésirables qui ont été importés avec le fichier SKP, car les calques de ce modèle seront importés dans notre modèle Farnsworth House (Maison Farnsworth). Pour ce faire, accédez à la **palette Calques**, sélectionnez **Layer 0** (Calque 0), puis cliquez sur le bouton **-**. Cette opération supprime le calque tout en conservant sa géométrie.

![](../../.gitbook/assets/3%20%2816%29.png)

_**Remarque :**_ _chaque fois que vous supprimez un calque, les groupes ou les géométries qui se trouvaient sur ce calque sont affectés à_ _**Aucun calque**. Il s’agit de la valeur par défaut pour tout objet qui n’a pas encore été attribué à un calque._

## **Création d’une miniature de contenu**

_Cette étape consiste à configurer une scène à utiliser comme miniature du_ _**contenu**_ _, qui s’affichera dans la_ _**palette Bibliothèque de contenu**._

1 – Pour définir les paramètres d’affichage de la·scène·Thumbnail (Miniature), procédez comme suit :

1. Dans l’onglet **Environnement** de la **palette Styles visuels**, décochez toutes les cases et définissez la couleur **Lower/ Background** (Inférieur/arrière-plan) sur blanc.
2. Assurez-vous que le mode d’affichage est défini sur **Perspective** **\(VP\)**.
3. Utilisez les **outils de navigation de la vue** pour effectuer un zoom avant et choisir un emplacement de caméra qui représente bien l’objet, comme dans l’image ci-dessous.

![](../../.gitbook/assets/4%20%2813%29.png)

2 – Pour enregistrer les paramètres que vous venez de définir, créez une scène :

1. Accédez à la **palette Scènes**.
2. Cliquez sur le bouton **+**. Cette opération permet de créer une scène en fonction de vos paramètres actuels.
3. Renommez-la **Thumbnail** (Miniature) et assurez-vous que les quatre \(4\) premières cases sont cochées : **Caméra**, **Calques**, **Soleil et ombres** et **Styles visuels**. Les autres paramètres de la scène ne sont pas très utiles pour la création de l’image miniature.
4. Utilisez le bouton **Mettre à jour la scène** à tout moment pour actualiser votre **scène** afin qu’elle corresponde à la vue de la caméra et aux paramètres visuels actuels.

![](../../.gitbook/assets/5%20%2811%29.png)

3 – **Enregistrez \(Ctrl + S\)** à nouveau le modèle Ottoman terminé. Notez que la **miniature de contenu** est créée à partir de la vue active lors du dernier enregistrement du modèle. Par conséquent, assurez-vous que vous vous trouvez dans la **scène Thumbnail (Miniature)** avant d’enregistrer.

_Si vous le souhaitez, vous pouvez comparer votre fichier au nôtre en ouvrant le fichier_ _**Ottoman – Barcelona\_Mies.axm**_ _enregistré dans_ _**Farnsworth House Data Set > Fichiers de support > FormIt> Furniture**_ _(Jeu de données Maison Farnsworth > Fichiers de support > Formit > Mobilier) dans le dossier_ _**Farnsworth House Data Set**(Jeu de données Maison Farnsworth).‌_

_Vous pouvez suivre les mêmes étapes ci-dessus avec les fichiers SKP de banc et de chaise situés dans le même dossier que le modèle Ottoman._

_**Conseil :**_ _pour accélérer le processus, nous vous recommandons d’utiliser le fichier_ _**Ottoman – Barcelona\_Mies.axm**_ _que vous venez de créer en tant que gabarit. Lors de la modélisation, vous pouvez réactiver la_ _**grille**_ _et les_ _**axes**_ _dans la_ _**palette Styles visuels**. Ajustez uniquement la position de la caméra de votre_ _**scène Thumbnail (Miniature)**_ _pour chaque élément de mobilier, afin de vous assurer que les_ _**miniatures de contenu**_ _restent cohérentes pour tous vos modèles de contenu._

## **Liaison d’une bibliothèque de contenu**

_Revenons au projet Farnsworth House (Maison Farnsworth). Nous allons apprendre à lier le dossier **FormIt** dans le dossier **Farnsworth House Data Set** (Jeu de données Maison Farnsworth), afin d’accéder facilement à tous ses fichiers, y compris le dossier_ **Custom FormIt Content** _(Contenu Formit personnalisé) que nous venons de créer, à partir de notre projet._

1 – Rebasculez sur le modèle Farnsworth House (Maison Farnsworth), ou rouvrez-le. _Si vous n’avez pas terminé le dernier chapitre, téléchargez et ouvrez le fichier_ _**1.11 – Import Models with Content Library.axm**_ _à partir du dossier_ _**Farnsworth House Data Set** (Jeu de données Maison Farnsworth)._

1. Ouvrez la **palette Bibliothèque de contenu** et cliquez sur l’icône **Lier le répertoire de la bibliothèque de contenu**. La fenêtre **Préférences** s’affiche avec l’onglet **Bibliothèque de contenu** ouvert.
2. Cliquez sur l’icône **+** pour **ajouter un nouvel emplacement de bibliothèque de contenu**. Une troisième fenêtre s’ouvre pour vous permettre de naviguer dans le répertoire de votre ordinateur et de sélectionner un dossier.
3. Dans le dossier _**Farnsworth House Data Set** (Jeu de données Maison Farnsworth), parcourez les dossiers suivants :_ _**Supporting Files > FormIt** (Fichiers de support > FormIt). Vous y trouverez les_ dossiers contenant les fichiers **.axm** créés précédemment dans ce chapitre. Double-cliquez sur le dossier **FormIt** pour le sélectionner.
4. Cliquez sur **Sélectionner un dossier**. Le chemin d’accès au dossier s’affiche dans le groupe de fonctions **Emplacements des bibliothèques – Local**.
5. De retour dans la fenêtre **Préférences**, cliquez sur **OK**. Le dossier lié est ajouté à la **bibliothèque de contenu**.
6. Pour accéder à cette nouvelle bibliothèque, ouvrez le menu déroulant situé dans la partie supérieure de la **palette Bibliothèque de contenu** et sélectionnez **FormIt**.
7. Notez que la structure de dossiers et tous les fichiers **.axm** du dossier lié s’affichent dans la **palette Bibliothèque de contenu**. Double-cliquez sur un sous-dossier pour accéder aux fichiers qu’il contient.

![](../../.gitbook/assets/link-library-content.png)

**Remarque :** si vous avez accès à **Autodesk Docs** \(connu précédemment sous le nom d’Autodesk 360\), vous pouvez également accéder aux fichiers que vous y avez stockés via le menu déroulant **Bibliothèque de contenu**.

## **Placement de contenu à partir de la bibliothèque**

_‌Nous allons maintenant placer les éléments de contenu que nous avons créés dans le modèle Farnsworth._

1 – Pour que vous puissiez visualiser l’intérieur de la maison afin d’y placer le mobilier, désactivez le calque **Roof** (Toit) et utilisez l’outil **Orbite \(O\)** pour faire tourner la vue en perspective en orbite jusqu’à ce que vous puissiez voir l’intégralité du calque Main Building Floor (Sol du bâtiment principal).

2 – Dans la **palette Bibliothèque de contenu**, vérifiez que la liste déroulante est toujours définie sur **FormIt**. Avant de placer le mobilier que vous venez de créer, placez le « noyau » de la maison :

1. Cliquez sur le dossier nommé **Other** (Autre) pour l’ouvrir, puis cliquez sur la miniature **Farnsworth House – Core** (Maison Farnsworth – Noyau) pour la sélectionner.
2. Placez le curseur de la souris sur **Main Building Floor** (Sol du bâtiment principal), puis cliquez sur le **centre de gravité** du sol pour placer le **noyau**.
3. Pour revenir au dossier FormIt, utilisez le bouton **Naviguer vers le haut**.

![](../../.gitbook/assets/7%20%282%29.jpeg)

3 – Définissez la caméra sur **Orthogonale \(VO\)** et **Vue de dessus \(VT\)**, et activez le calque **Main Building Floor** (Sol du bâtiment principal) pour afficher le calque **Plan Image** (Image du plan). Reportez-vous aux chapitres précédents pour en savoir plus sur les paramètres **Vues** et **Calques**.

4 – Sélectionnez l’élément **Farnsworth House – Core** (Maison Farnsworth – Noyau) et déplacez-la jusqu’à ce qu’elle soit étroitement alignée avec le calque Plan Image (Image du plan).

![](../../.gitbook/assets/8%20%281%29.png)

_**Remarque :**_ _lorsque vous déplacez le_ _**noyau**, veillez à ne pas modifier son élévation. Vous pouvez utiliser la touche_ _**Maj**_ _pour limiter le mouvement à l’un des axes ou vous assurer que les points de référence de départ et d’arrivée de l’option_ _**Déplacer \(M\)**_ _sont à la même hauteur en cliquant uniquement sur le calque_ _**Plan Image** (Image du plan) et non sur le __**noyau**__. Reportez-vous aux chapitres précédents pour en savoir plus sur l’outil_ _**Déplacer \(M\)**_ _._ 

## **Placement de mobilier à partir de la bibliothèque**

1 – En suivant la même procédure, vous pouvez désormais placer le mobilier que vous avez créé précédemment dans ce chapitre à partir du dossier **Custom FormIt Content** (Contenu Formit personnalisé). Si vous n’avez pas converti les trois \(3\) fichiers SKP, vous pouvez utiliser les versions prédéfinies dans le dossier **Furniture** (Mobilier).

_**Remarques :**_

* _Activez de nouveau le calque_ _**Main Building Floor**_ _(Sol du bâtiment principal), de sorte que vous puissiez placer le mobilier directement sur la surface de_ _**Main Building Floor**(Sol du bâtiment principal)._
* _Lors du placement d’un nouvel objet, utilisez la touche_ _**Tab**_ _pour alterner entre les plans de placement._
* _Lors du placement d’un nouvel objet, utilisez la touche_ _**Espace**_ _ pour le faire pivoter de 90 intervalles avant de le placer._

![](../../.gitbook/assets/9%20%283%29.png)

2 – De même, explorez les **exemples de la bibliothèque de contenu** pour placer du contenu OOTB. Notez que certains d’entre eux ont plusieurs tailles différentes, comme les types de familles dans Revit.

![](../../.gitbook/assets/10%20%286%29.png)

## **Utilisation de l’outil Échelle**

1 – En utilisant les techniques que vous venez d’apprendre, placez une occurrence du composant **tree\_pine** à partir du dossier **Farnsworth House Data Set > FormIt > Planting** (Jeu de données Maison Farnsworth > Formit > Plantes).

1. Une fois placé, sélectionnez le groupe et renommez-le **Tree** (Arbre). Cliquez avec le bouton droit de la souris pour accéder au **menu contextuel** et choisissez **Échelle non uniforme \(NU\)**.
2. Cliquez sur l’un des **boutons Échelle non uniforme** pour redimensionner et modifier les proportions du groupe **Tree** (Arbre) selon vos besoins.

![](../../.gitbook/assets/11%20%283%29.png)

![](../../.gitbook/assets/12%20%282%29.png)

_**Remarque :**_ _de même, l’outil_ _**Échelle \(SC\)**_ _peut être utilisé pour mettre à l’échelle un modèle ou un groupe entier de manière uniforme._

2 – Copiez ce groupe et placez plusieurs arbres autour de la maison, à l’aide des **outils Échelle** pour créer plusieurs tailles et proportions.

![](../../.gitbook/assets/13%20%286%29.png)

_**Remarque :**_ _même si les arbres appartiennent tous au même groupe, nous avons pu les_ _**mettre à l’échelle**_ _selon différentes tailles. L’utilisation des outils_ _**Échelle \(SC\)**_ _et_ _**Échelle non uniforme \(NU\)**_ _en dehors du mode de modification de groupe vous permet de modifier des occurrences individuelles du même groupe. Si vous deviez modifier un des groupes_ _**Tree**_ _(Arbre) et modifier sa géométrie ou son matériau, toutes les occurrences de groupe seraient mises à jour, mais chacune conserverait son échelle personnalisée actuelle. Essayez !_

### **Organisation du modèle**

_N’oubliez pas de toujours trier le contenu ajouté sur les calques. Dans cet exemple, nous vous recommandons de placer le noyau et tout le mobilier sur le calque_ _**Main Building Floor**_ _(Sol du bâtiment principal) et les arbres sur un nouveau calque nommé_ _**Planting**(Plantes)._

