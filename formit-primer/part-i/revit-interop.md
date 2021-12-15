# 1.15 – Utilisation de Revit

_L’une des fonctionnalités les plus intéressantes de FormIt est la possibilité de déplacer les modèles d’un environnement de modélisation flexible comme FormIt vers un environnement paramétrique puissant comme Revit. Dans ce chapitre, nous allons passer en revue quelques exercices qui permettent de déplacer différents éléments de FormIt vers Revit et vice versa._

_Ce chapitre utilise des exemples de familles Revit. Si ce n’est pas déjà fait, vous pouvez les télécharger à partir du dossier **Farnsworth House Data Set (Jeu de données Maison Farnsworth House).** Si vous n’avez pas suivi l’intégralité du didacticiel jusqu’à présent, vous pouvez également télécharger et ouvrir le fichier **1.15 – Working With Revit.axm** à partir du dossier **Jeux de données Partie I FormIt Primer**._

_Dans ces exercices, nous allons utiliser Revit 2022, qui offre des fonctionnalités d’interopérabilité améliorées avec FormIt. Les versions antérieures de Revit ne disposent pas de certaines fonctionnalités présentées dans ce didacticiel, et leur interface utilisateur est différente._

## De Revit à FormIt

### Conversion des familles Revit à utiliser dans FormIt

Si vous \(ou votre entreprise\) disposez d’une mine de familles Revit que vous souhaitez utiliser dans FormIt, consultez cette section, car elle explique comment exporter par lots des fichiers RFA vers FormIt.

_**Remarque :**_ _les étapes ci-dessous indiquent l’interface et les étapes nécessaires lors de l’utilisation de Revit 2022, mais les outils_ _**Convertir le format RFA au format FormIt**_ _sont disponibles depuis Revit 2016._

1 – Ouvrez un nouveau projet ou une nouvelle famille Revit. Étapes suivantes :

1. Dans le ruban **Compléments**, recherchez le groupe de fonctions **FormIt Converter** et cliquez sur le bouton **Convertir un fichier RFA au format FormIt**. La **boîte de dialogue Convertir des familles Revit** s’affiche.
2. Dans le champ **Chemin d’accès aux fichiers de famille Revit**, accédez à l’emplacement où vous avez enregistré le dossier suivant sur votre ordinateur : **Jeu de données Maison Farnsworth > Fichiers de support > Revit**.
3. Dans le champ **Chemin d’accès au contenu FormIt**, accédez à **Jeu de données Maison Farnsworth > Fichiers de support > FormIt > Contenu FormIt personnalisé**. Si vous n’avez pas terminé le chapitre **1.11 – Importation de modèles avec la bibliothèque de contenu**, vous devrez peut-être créer le dossier **Contenu FormIt personnalisé** ou choisir une autre destination.
4. Pour lancer le processus de conversion, cliquez sur **OK**.

![](../../.gitbook/assets/0%20%2823%29.png)

_**Remarques :**_

* _Ce processus prend un certain temps, car Revit ouvre le fichier_ _**RFA**_ _dans le premier chemin, puis le convertit et l’enregistre au format_ _**AXMF**_ _pour FormIt._
* _Dans cet exercice, nous allons convertir un seul fichier, mais vous pouvez utiliser cette procédure pour convertir par lots tous les fichiers_ _**RFA**_ _du dossier sélectionné \(y compris les fichiers_ _**RFA**_ _dans les dossiers imbriqués\)._

2 – Une fois le processus terminé, revenez à FormIt. Le nouveau contenu s’affiche alors dans la **palette Bibliothèque de contenu**, dans le dossier **FormIt >** **Contenu FormIt personnalisé** que nous avons précédemment lié. Si vous avez enregistré les fichiers **AXMF** convertis à un autre emplacement ou si vous n’avez pas terminé le chapitre **1.11 – Importation de modèles avec la bibliothèque de contenu**, vous devrez peut-être ajouter ce dossier à votre bibliothèque de contenu pour en afficher le contenu. Reportez-vous au chapitre 1.11 pour obtenir des instructions sur l’ajout de dossiers à votre bibliothèque de contenu.

![ ](../../.gitbook/assets/1%20%2824%29.png)

**Remarque** : _l’exportation ne prend pas en charge toutes les catégories de Revit. Les familles « indépendantes » ou « basées sur le niveau » sont prises en charge, mais pas les familles « basées sur l’hôte », telles que les portes et les fenêtres. Les éléments Volume, Meubles de rangement, Environnement, Mobilier, Système de mobilier, Modèle générique, Parking, Site et Équipement spécialisé sont tous pris en charge. Toutes les familles non prises en charge dans le pli sélectionné sont simplement ignorées._

## De FormIt à Revit

_Il existe deux manières d’importer une géométrie de FormIt vers Revit. Vous pouvez importer un fichier_ _**.axm** existant dans un projet Revit ou un fichier de famille Revit, qui se comportera de la même façon qu’un modèle importé ou un fichier CAO. Vous pouvez également lancer FormIt à partir de Revit et importer chaque groupe FormIt dans Revit en tant qu’élément Modèle générique individuel. La deuxième méthode est décrite dans le chapitre **2.8 – Workflows Revit avancés** de la_ _**partie**_ _**II** du guide._

### Importation du modèle Maison Farnsworth dans Revit

1 – Pour importer un fichier FormIt \(**.axm**\) dans Revit, démarrez un nouveau projet Revit et ouvrez la vue 3D par défaut. Étapes suivantes :

1. Accédez à l’**onglet Insérer**, puis cliquez sur le bouton **Importer CAO**. La fenêtre **Importer les formats CAO** s’ouvre.
2. Assurez-vous que la liste déroulante **Fichiers de type** est définie sur **Fichiers FormIt \(\*.axm\)**.
3. Recherchez et sélectionnez le fichier **.axm** Farnsworth sur lequel vous avez travaillé. Si vous n’avez pas suivi les instructions de la partie I du guide, vous pouvez également ouvrir le fichier **1.15 – Working With Revit.axm** à partir du dossier **Jeu de données Maison Farnsworth > Fichiers de chapitre**.
4. Assurez-vous que l’option **Importer les niveaux FormIt** est cochée.
5. Une fois les paramètres définis, cliquez sur **Ouvrir**. La géométrie FormIt est importée dans Revit en tant qu’élément unique.

![](../../.gitbook/assets/2%20%2824%29.png)

Importation d’un fichier FormIt à l’aide du bouton Importer CAO.

![](../../.gitbook/assets/3%20%2821%29.png)  Élément .axm importé. Notez que les niveaux du modèle FormIt sont également importés dans Revit.

_Comme pour les autres formats CAO, les calques du fichier d’origine sont importés dans Revit. Cette fonction vous permet de définir différents paramètres de visibilité pour chaque calque afin de manipuler facilement l’apparence graphique de votre fichier FormIt dans n’importe quelle vue Revit._

2 – Pour ajuster la visibilité des calques du fichier .axm importé, procédez comme suit :

1. Accédez à la fenêtre **Remplacements visibilité/graphisme \(VG oo VV\)**, puis à l’onglet **Catégories importées** et développez le fichier FormIt importé. Ensuite, désélectionnez le calque **Plantes** afin de désactiver le calque dans la vue active, puis cliquez sur **OK**.
2. Définissez le **style visuel** sur **Réaliste**. Vous pouvez constater que tous les matériaux FormIt ont été importés dans Revit.

![](../../.gitbook/assets/4%20%2820%29.png)

3 – Les matériaux FormIt importés sont maintenant disponibles dans ce projet Revit, étiquetés avec la classe **FormIt**. Ouvrez simplement le **navigateur de matériaux** et recherchez « FormIt » pour tous les afficher. Ils peuvent désormais être utilisés dans votre projet Revit comme n’importe quel autre matériau.

![](../../.gitbook/assets/5%20%2819%29.png)

