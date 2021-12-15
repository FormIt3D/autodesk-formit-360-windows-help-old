# Système de meneaux de vitrine/mur-rideau

![](../.gitbook/assets/dynamo-storefront-system-options.gif)

## Optimisé par Dynamo

Dynamo permet de créer rapidement des systèmes de meneaux de vitrine/mur-rideau dans FormIt. Le système Storefront Curtainwall se trouve dans le répertoire Dynamo Samples du groupe de fonctions Dynamo :

![](../.gitbook/assets/storefront-curtainwall-button%20%281%29.png)

## Sélection du vitrage pour le système de meneaux

À partir de FormIt 2021.2, le système Storefront Curtainwall utilise le nouveau [nœud SelectFromFormIt](https://formit.autodesk.com/page/formit-dynamo#dynamo-formit-nodes), qui vous permet de sélectionner un élément de « vitrage » \(une seule face ou un solide extrudé\) autour duquel vous pouvez générer un système de meneaux.

![Plan simple d’une « vitre » avec une ouverture pour les portes en bas.](../.gitbook/assets/storefron-system-1_glass-only.png)

Lorsque vous cliquez sur la miniature Storefront Curtainwall \(notez l’icône indiquant qu’une sélection est requise\), FormIt vous invite à sélectionner la géométrie de vitre pour continuer :

![](../.gitbook/assets/storefront-curtainwall-prompt.png)

Tenez compte des remarques et mises en garde suivantes concernant le fonctionnement de la sélection du vitrage :

* Actuellement, seules les surfaces planes sont prises en charge. Si vous sélectionnez une série de surfaces \(par exemple, une surface « incurvée » composée de surfaces planes plus petites\), le script recherche la face plane la plus grande et l’utilise.
* Si votre vitre est opaque, c’est-à-dire qu’une seule face est très légèrement extrudée afin d’apporter une légère épaisseur, le script recherche la plus grande surface afin de générer les meneaux obtenus sur un côté du solide en verre. 
* Vous pouvez esquisser des ouvertures de portes et supprimer la surface obtenue du contour du vitrage. Les meneaux obtenus respectent l’ouverture, laissant ainsi un espace vide pour l’ajout de portes.
* En raison des limitations de Dynamo, ce script ne fonctionne pas si la géométrie du vitrage comporte des ouvertures au milieu.

## Trucs et astuces

Lorsque vous sélectionnez la géométrie d’un graphique Dynamo dans FormIt, certaines astuces d’organisation simplifient l’expérience et l’instanciation des résultats :

* Placez la vitre dans un groupe et utilisez le groupe comme sélection pour le script Storefront/Curtainwall. Cette méthode permet de modifier le profil de la vitre plus facilement après la génération des meneaux. Si la vitre est fortement modifiée entre les exécutions et que les ID de face ont changé, le groupe s’assure que le script identifie toujours la vitre, car il utilise l’ID de groupe et non l’ID de face.
* Si vous prévoyez de copier les résultats du système de meneaux et de les coller à d’autres emplacements de votre modèle, il est préférable que la vitre et les meneaux obtenus soient contenus dans un groupe. Cela permet également d’éviter les problèmes avec le nœud de sélection qui ne sait pas quelle occurrence de vitre utiliser lorsque seul le groupe de meneaux obtenu est copié et collé.
   * Tout d’abord, mettez votre vitre dans un groupe. Double-cliquez dessus pour sélectionner la vitre, puis appuyez sur la touche G ou utilisez les commandes de groupe du menu contextuel ou de la barre d’outils.
   * Sélectionnez le groupe obtenu et placez-le dans un autre groupe.
   * Double-cliquez pour ouvrir le premier groupe. Il s’agit du « conteneur » de la vitre et des meneaux obtenus.
   * Cliquez sur la miniature Storefront Curtainwall et utilisez le groupe de vitres comme sélection.
   * Une fois le script exécuté, vous pouvez quitter le groupe et copier/coller le conteneur selon vos besoins. Vous pouvez modifier toutes les instances \(en ajustant la forme ou les paramètres de la vitre\) sans problème.

## Options du système de meneaux

Une fois que vous avez sélectionné la vitre et exécuté le script, vous obtenez un résultat dans la zone de dessin FormIt, sous la forme d’un groupe FormIt. Ce groupe est automatiquement sélectionné et le groupe de fonctions Properties affiche les options disponibles.

![](../.gitbook/assets/storefront-curtainwall-parameters.png)

* **Run** : si vous modifiez la forme de la vitre et souhaitez réexécuter le graphique pour mettre à jour les résultats du meneau, cliquez sur ce bouton.
* **Edit Embedded Graph** : modifiez le script Dynamo qui génère la géométrie. Ce script est incorporé dans le fichier FormIt et est spécifique de ce groupe.
* **Select Glass \(Surface or Solid\)** : cliquez sur ce bouton pour mettre à jour la sélection vers un autre élément de vitrage autour duquel générer les meneaux.

Le script utilise les valeurs par défaut pour sa première exécution. Vous devez donc les ajuster en fonction de votre cas d’utilisation unique. Toutes les valeurs utilisent les unités FormIt actives.

* **Mullion Width + Depth** : largeur et profondeur de tous les éléments de meneau.
* **Vertical Mullion Spacing** : distance, au centre, entre chaque meneau vertical.
* **Flip Vertical Mullion Layout** : le script commence l’espacement des meneaux verticaux à partir d’un côté, choisi de manière arbitraire. Si le résultat indique que l’espacement des meneaux est défini sur le mauvais côté pour votre cas d’utilisation, définissez cette option sur True pour que la présentation commence sur le site opposé.
* **Center Vertical mullion Layout** : au lieu de commencer le calcul de l’espacement des meneaux verticaux à une extrémité de la vitre, lancez le calcul au milieu, afin de créer une disposition symétrique des meneaux verticaux.
* **First Horizontal Mullion Spacing** : définit l’espacement du premier meneau horizontal en partant du bas. Cette option est utile si vous avez besoin d’une rangée de modules de vitrage plus courts en bas, séparés du reste de l’espacement des meneaux horizontaux.
* **Horizontal Mullion Spacing** : espacement type des meneaux horizontaux, au centre, commençant après le premier meneau comme indiqué ci-dessus.
* **Flip Horizontal Mullion Layout** : si vous souhaitez que la disposition des meneaux horizontaux commence en haut et non en bas, définissez cette option sur True.
* **Center Horizontal Mullion Layout** : au lieu de lancer le calcul de l’espacement des meneaux horizontaux en bas ou en haut de la vitre, lancez le calcul au milieu, afin de créer une disposition symétrique des meneaux horizontaux.

## Options masquées

Vous recherchez d’autres options de personnalisation ? Plusieurs options avancées sont masquées dans le groupe de fonctions Propriétés de FormIt. Pour y accéder, il suffit de cliquer sur « Edit Embedded Graph » afin d’afficher l’intégralité du contenu du graphique dans Dynamo :

![](../.gitbook/assets/dynamo-edit-embedded-graph.png)

### Meneaux aléatoires

![](../.gitbook/assets/storefront-curtainwall-random-verticals.png)

* **Randomize Vertical and Horizontal Mullion Layout** : définissez cette option sur True pour espacer les meneaux verticaux ou horizontaux de façon aléatoire.
* **Min/Max Mullion Spacing \(if random\)** : ajustez ces valeurs pour définir une plage de valeurs d’espacement aléatoire minimum et maximum.

### Meneaux extérieurs

![](../.gitbook/assets/storefront-curtainwall-border-mullion-options.png)

* **Flip Offset Direction of Border Mullions :** par défaut, le système de meneaux utilise le contour du vitrage et le décale vers l’intérieur afin de créer les meneaux extérieurs. Pour effectuer un décalage vers l’extérieur, définissez cette option sur True. Cette opération augmente la taille globale du système de meneaux en dehors du contour du vitrage en fonction du paramètre Largeur du meneau.
* **Tolerance Between Selection and Border Mullions** : par défaut, le système de meneaux est généré exactement au niveau du contour du vitrage, ce qui peut entraîner du Z fighting à l’endroit où le cadre de la vitre et les surfaces externes des meneaux extérieurs se rejoignent. Dans la plupart des cas, ceci n’est pas visible, mais si votre cas d’utilisation requiert que les arêtes du système soient visibles et que vous souhaitez éviter le Z fighting, activez cette option et ajustez la valeur de tolérance si nécessaire.

