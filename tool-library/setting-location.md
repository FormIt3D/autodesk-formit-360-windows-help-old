# Définition de l’emplacement

La définition de l’emplacement de votre projet dans le monde est importante pour la précision de votre modèle et des analyses en aval, notamment pour les raisons suivantes :

* L’emplacement est utilisé pour importer une image satellite utilisée pour tracer un site ou un bâtiment existant.
* L’emplacement est utilisé pour importer un terrain 3D, qui peut servir à référencer les données topologiques d’un site.
* L’emplacement est utilisé pour positionner avec précision le soleil dans le ciel, ce qui a une incidence sur le calcul des ombres.
* L’emplacement est utilisé pour l’analyse d’ensoleillement et l’analyse d’énergie afin de fournir des calculs analytiques précis.

Vous devez être connecté à votre compte Autodesk Account pour accéder à la boîte de dialogue Définir l’emplacement et à ses services.

### Mise en route avec l’emplacement

* Lancez la boîte de dialogue **Définir l’emplacement** à partir de l’outil **Emplacement** de la barre d’outils ou à l’aide du raccourci clavier SL.

![](../.gitbook/assets/location-toolbar.png)

* Tout d’abord, saisissez l’emplacement de votre projet dans la zone de recherche située dans le coin supérieur gauche de la fenêtre _Définir l’emplacement_.

![](../.gitbook/assets/location-step-1%20%281%29.png)

* Sélectionnez l’une des options d’emplacement proposées automatiquement ou appuyez sur la touche Entrée pour choisir la première option.
* Un zoom avant est effectué automatiquement sur l’emplacement que vous avez recherché.

### Définir l’emplacement uniquement et Importer une image satellite et un terrain

Une fois que vous avez recherché un emplacement, choisissez l’une des deux options suivantes :

* L’option **Définir l’emplacement uniquement** permet de définir l’emplacement dans le fichier sans importer d’image satellite.
* L’option **Importer une image satellite et un terrain** permet de définir l’emplacement, ainsi que l’image satellite et le terrain à l’aide d’un niveau de zoom et d’étendues que vous pouvez configurer.

### Importation d’une image satellite

* Cliquez sur **Importer une image satellite et un terrain** dans la partie supérieure droite de la fenêtre **Définir l’emplacement**.
* Un aperçu de l’image satellite s’affiche au centre de la fenêtre, avec une indication de l’emplacement de l’origine FormIt par rapport à l’image.

![](../.gitbook/assets/location-step-2.png)

* Faites glisser l’image satellite dans le carré pour ajuster sa position.
* Une fois que la surface carrée contient l’image souhaitée, cliquez sur **Terminer l’importation**.
* L’image est importée à l’échelle, avec le nord géographique orienté vers le haut, centrée sur l’origine de la zone de dessin FormIt. Pour modifier la transparence et l’ordre Z de l’image importée, double-cliquez dessus et accédez à la [**palette Propriétés**](../formit-introduction/tool-bars.md).

![](../.gitbook/assets/location-step-3.png)

### Mise à jour de l’image satellite

Après avoir importé la première image satellite, utilisez la fenêtre Définir l’emplacement pour ajuster le niveau de zoom ou l’étendue de l’image satellite.

* Accédez·à nouveau la fenêtre **Définir l’emplacement** à partir de la barre d’outils, comme indiqué ci-dessus.
* Cliquez sur **Importer une image satellite et un terrain.**
* Le niveau de zoom et l’étendue de l’image satellite actifs s’affichent, comme indiqué dans la zone de dessin FormIt.
* Il vous suffit d’ajuster la position ou le zoom, puis de cliquer sur **Terminer l’importation** comme vous l’avez fait auparavant.
* Lorsque l’image est réimportée dans la zone de dessin, elle est placée à l’emplacement correct par rapport à la position de l’image d’origine \(et ne peut plus être centrée sur l’origine\) :

![](../.gitbook/assets/location-step-4.png)

### Importation d’un terrain

Dans FormIt 2021.3, lorsque vous utilisez la boîte de dialogue **Définir l’emplacement** pour importer une image satellite, vous obtenez également le terrain.

![](../.gitbook/assets/terrain-button_original.png)

Lorsque le terrain est importé, il est placé sur un calque, qui est désactivé par défaut \(si vous avez commencé la modélisation, votre modèle est peut être recouvert par le terrain\).

Lorsque vous êtes prêt à afficher le terrain, activez le calque Terrain en cochant la case correspondante :

![](../.gitbook/assets/terrain-layer%20%281%29.png)

![](../.gitbook/assets/terrain_solid.png)

### Utilisation du terrain

Le terrain est placé dans un groupe FormIt. Double-cliquez sur le groupe pour le modifier.

Vous y trouverez deux maillages : un pour les côtés et le bas, et un pour le haut.

Si vous souhaitez modifier le terrain, vous devez convertir les maillages en un seul objet solide :

* Sélectionner les deux maillages
* Cliquez avec le bouton droit de la souris, puis choisissez l’option Maillages en objets ou utilisez le raccourci MO.

![](../.gitbook/assets/terrain-mesh-context.png)

Lors de la conversion des deux maillages en un objet simultanément, FormIt peut les combiner en un objet solide et multiple, qui peut être utilisé pour des opérations de solide telles que la coupe booléenne.

À partir de là, vous pouvez utiliser une combinaison de [Vue de dessus](orthographic-views.md) et de [Caméra orthogonale](orthographic-camera.md) pour tracer la limite de votre site sur un plan horizontal, puis extruder ce plan dans un volume qui croise le terrain. L’utilisation d’un [matériau](materials.md) transparent vous permet de visualiser le terrain à travers le solide de découpe :

![](../.gitbook/assets/terrain-cutter-before.png)

Utilisez l’outil Couper la géométrie et sélectionnez le terrain comme « solide à couper » et le volume de découpe comme « solide à supprimer ».

![](../.gitbook/assets/terrain-cut-menu.png)

Le solide de découpe est supprimé du terrain, exposant ainsi un espace vide où vous pouvez dessiner le nouveau site et les nouvelles fondations.

![](../.gitbook/assets/terrain-cutter-after.png)

Vous pouvez utiliser des [calques](layers.md) pour masquer le solide de découpe, ou même faire des copies du terrain avec et sans la découpe, au cas où vous auriez besoin de référencer le terrain d’origine, ou de changer la forme de découpe avant d’exécuter l’opération de découpe de solide.

