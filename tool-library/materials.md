# Matériaux

Faites apparaître vos modèles FormIt avec des matériaux qui prennent en charge les textures de réflexion, de lustre et en relief.

## Groupe de fonctions Matériaux

![](<../.gitbook/assets/materials-sample-category (2).png>)

Dans le groupe de fonctions Matériaux, vous pouvez choisir parmi une grande variété d’échantillons de matériaux, naviguer entre les bibliothèques de matériaux liées et, à partir de FormIt 2021, consulter et utiliser le contenu des matériaux d’autres fichiers FormIt (.AXM).

### Sources de la bibliothèque de matériaux

Dans FormIt 2021 et les versions ultérieures, le groupe de fonctions Matériaux dispose d’une interface déroulante permettant de choisir parmi les sources de la bibliothèque de matériaux disponibles : Dans l’esquisse, Échantillons de matériaux et [Bibliothèques liées ](https://windows.help.formit.autodesk.com/tool-library/materials#linking-material-libraries).

![](<../.gitbook/assets/materials-directory-picker (1).png>)

#### Dans l’esquisse

Affiche les matériaux enregistrés dans l’esquisse FormIt active.

#### Échantillons de matériaux

Affiche une liste des exemples de matériaux disponibles. Ces offres sont stockées sur un serveur basé sur le cloud. Notez les points suivants :

* Une connexion Internet est requise lors de l’accès aux catégories Échantillons de matériaux pour la première fois.
* Lorsque vous accédez à une catégorie pour la première fois, elle est téléchargée puis mise en cache sur votre ordinateur, de sorte que les sessions ultérieures ne nécessitent pas de téléchargement.
* L’équipe FormIt met parfois à jour les offres incluses dans Échantillons de matériaux. Dans ce cas, FormIt supprime et télécharge automatiquement les catégories pour obtenir la dernière version.

![](../.gitbook/assets/materials-samples\_original.png)

**Bibliothèques liées**

D’autres répertoires et emplacements apparaîtront après la [liaison des bibliothèques de matériaux](https://windows.help.formit.autodesk.com/tool-library/materials#linking-material-libraries).

### Créer, Supprimer et Pipette

![](../.gitbook/assets/materials\_add.PNG) L’outil **Créer un matériau** vous permet de créer un matériau et de définir sa couleur, sa texture, sa texture en relief, sa texture de découpe, sa transparence et ses paramètres de réflexion/lustre.

![](<../.gitbook/assets/materials\_delete (1) (1).PNG>) **Supprimez** le(s) matériau(s) sélectionné(s).

![](../.gitbook/assets/materials\_eyedropper.PNG)L’outil **Pipette** vous permet de sélectionner un matériau peint dans la scène et de commencer immédiatement peindre avec.

* Cliquez sur l’outil Pipette, puis sur une face peinte avec un matériau.
* Le matériau présent sur la face est mis en surbrillance dans le groupe de fonctions et l’outil Pinceau devient actif lorsque ce matériau est chargé.

### Actualiser, Lier des bibliothèques et Purger les éléments non utilisés

\*\*\*\*![](../.gitbook/assets/materials-link.png) L’outil **Lier les bibliothèques de matériaux** vous permet de lier des bibliothèques de matériaux à partir des répertoires locaux. Les répertoires contenant des fichiers JPG, PNG ou AXM (FormIt) affichent du contenu. Pour plus d’informations, reportez-vous à la rubrique [Liaison de bibliothèques de matériaux](https://windows.help.formit.autodesk.com/tool-library/materials#linking-material-libraries).

![](../.gitbook/assets/materials-refresh.png)L’outil **Actualiser** vous permet d’actualiser le répertoire actuel. Cet outil est uniquement activé lorsque vous visualisez un répertoire lié localement (et non Dans l’esquisse ou Échantillons de matériaux).

![](../.gitbook/assets/materials-purge.png)L’outil **Purger les éléments non utilisés** vous permet de supprimer des matériaux de l’esquisse FormIt actuelle.

Les matériaux inutilisés peuvent s’accumuler naturellement au cours du processus d’itération, mais ils augmentent considérablement la taille du fichier s’ils utilisent des textures de haute qualité.

Les matériaux inutilisés s’affichent avec un nom gris dans la liste Dans l’esquisse.

Cliquez sur l’outil Purger les éléments non utilisés pour supprimer tous les matériaux inutilisés. Une invite s’affiche. Elle vous permet d’annuler l’action en cas de doutes. Ce bouton est uniquement activé dans la liste Dans l’esquisse.

### Liaison de bibliothèques de matériaux

FormIt 2021 et les versions ultérieures permettent de lier le groupe de fonctions Matériaux aux répertoires locaux (bibliothèques) incluant le contenu des matériaux, y compris les dossiers des fichiers JPG, PNG et/ou FormIt :

![](../.gitbook/assets/materials-axms.png)

![Affichez les différents matériaux à partir d’un fichier FormIt ou de fichiers JPG/PNG dans un répertoire.](../.gitbook/assets/materials-axm-content.png)

* Les **fichiers JPG/PNG** s’affichent sous forme de matériaux, qui peuvent être peints directement dans l’esquisse FormIt actuelle.
   * Lorsque vous cliquez sur une miniature, le fichier image est directement converti en matériau FormIt et copié dans l’esquisse actuelle.
   * FormIt vous renvoie dans le répertoire « Dans l’esquisse », contenant le matériau que vous venez de copier dans l’esquisse.
* **Les fichiers FormIt \(*.axm)** s’affichent sous forme de dossiers avec une icône FormIt.
   * Si vous cliquez sur les dossiers du fichier FormIt, tous les matériaux FormIt enregistrés dans ce fichier s’affichent.
   * Notez que FormIt doit charger une partie du fichier pour obtenir le contenu des matériaux. Par conséquent, l’affichage des matériaux des fichiers plus volumineux dans le groupe de fonctions peut prendre plus de temps.

### Interactions de matériaux

Pour **peindre un matériau**, cliquez une fois sur la miniature. L’outil Pinceau s’affiche. Vous pouvez maintenant placer le curseur sur la géométrie dans la zone de dessin FormIt et cliquer sur les faces ou les groupes pour les peindre.

Une fois que vous êtes dans l’outil Pinceau, procédez comme suit :

* Un simple clic vous permet de peindre des faces et des groupes.
   * Lorsque vous peignez des groupes, le matériau est intégré en cascade à la géométrie imbriquée et couvre toute surface ou tout groupe peint avec le matériau par défaut.
* Pour peindre des solides entiers, double-cliquez sur une face afin de sélectionner tous les éléments attachés.

Vous pouvez également sélectionner des faces et des groupes en premier, puis cliquer une fois sur la miniature d’un matériau afin de peindre la sélection avec ce matériau.

**Pour modifier un matériau**, double-cliquez sur la miniature afin d’afficher l’éditeur de matériaux (voir ci-dessous).

Pour **renommer un matériau**, double-cliquez sur son nom.

**Pour identifier un matériau** peint sur la géométrie, sélectionnez-le, puis recherchez la surbrillance et l’icône indiquant le(s) matériau(x) peint(s) sur la géométrie sélectionnée.

![](../.gitbook/assets/material\_selected.png)

**Le matériau par défaut** peut être utilisé pour « effacer » efficacement les matériaux d’une face ou d’un groupe. Toute géométrie non peinte à l’aide d’un matériau est implicitement peinte à l’aide du matériau par défaut.

### Gestion de listes

Pour ajuster la taille des miniatures, ajustez la largeur de la colonne (cliquez sur la ligne verticale à droite de « Matériau » et faites-la glisser).

Utilisez la barre « Filtrer... » pour rechercher des matériaux spécifiques.

Les matériaux dont le nom s’affiche en gris correspondent aux matériaux qui ne sont pas utilisés dans l’esquisse actuelle.

## Création et modification des matériaux

![](<../.gitbook/assets/materials-editor (1).png>)

Lorsque vous créez ou modifiez un matériau, la boîte de dialogue Éditeur de matériaux s’affiche, dans laquelle vous pouvez personnaliser les éléments suivants :

* **Couleur**
* **Textures d’image**
   * Cliquez sur la miniature pour choisir une nouvelle texture.
   * Cliquez sur l’icône Enregistrer pour enregistrer la texture afin de la modifier dans une autre application.
   * Cliquez sur l’icône Supprimer pour supprimer la texture de ce matériau.
      * **Texture à partir d’un fichier image**
         * JPG ou PNG
      * **Texture en relief à partir d’un fichier image**
         * JPG recommandé
         * Idéal pour ajouter des effets de profondeur aux matériaux.
         * Vous pouvez utiliser des logiciels gratuits tels que ShaderMap pour générer des textures en relief en fonction d’une texture.
      * **Texture de découpe à partir d’un fichier image**
         * PNG
         * Idéal pour les matériaux qui présentent une transparence partielle, comme les clôtures grillagées ou les panneaux perforés.
* **Nom**
* **Échelle horizontale et verticale**
   * Lorsque le bouton Verrouiller l’aspect est activé, il permet de s’assurer que l’échelle horizontale et verticale respecte le rapport hauteur/largeur de la texture.
   * Pour étirer un matériau, ajustez l’échelle horizontale indépendamment de l’échelle verticale.
   * Vous pouvez remplacer l’échelle horizontale et verticale par face à l’aide de l’outil Ajuster le positionnement des matériaux (voir ci-dessous).
* **Transparence**, **Réflexion** et **Lustre**

## Ajustement du positionnement des matériaux

Lorsque vous peignez un matériau sur une face, FormIt évalue la meilleure orientation possible de manière approximative :

* Les faces verticales s’orientent avec le haut de la texture orienté le long de l’axe Z.
* Les faces horizontales orientent la texture dans le sens de la longueur du côté le plus long de la face.

Utilisez l’outil **Ajuster le positionnement des matériaux** pour remplacer le positionnement des matériaux par défaut, ainsi que l’échelle du matériau sur des faces spécifiques :

* Sélectionnez une ou plusieurs faces peintes avec un matériau.
   * Si la face hérite son matériau de son groupe parent, vous devez peindre la face directement en premier.
* Accédez à l’outil Ajuster le positionnement des matériaux via le raccourci clavier MP ou à partir du menu contextuel :

![](../.gitbook/assets/adjust-material-placement.PNG)

Utilisez les commandes à l’écran pour déplacer, faire pivoter et mettre à l’échelle les textures de matériaux directement sur la face de manière interactive :

![](../.gitbook/assets/materialplacement.gif)

![](../.gitbook/assets/adjust-material-placement.gif)

Pour réinitialiser les modifications apportées au positionnement du matériau, il vous suffit de peindre à nouveau la face avec le matériau d’origine, dans le groupe de fonctions Matériaux.

## Conversion de matériaux vers Revit

Les matériaux sont transférés vers Revit lors de l’utilisation du [complément FormIt](https://formit.autodesk.com/page/formit-revit) pour Revit 2018 ou version ultérieure.
