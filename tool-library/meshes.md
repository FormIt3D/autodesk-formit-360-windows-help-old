# Maillages

À partir de la version v17.0, FormIt propose un nouveau type de géométrie : les maillages.

Les maillages sont des représentations optimisées des objets FormIt standard et sont particulièrement utiles pour améliorer les performances des géométries comportant de nombreux polygones, telles que du mobilier ou des environnements 3D, par exemple, des personnes, des arbres, des voitures et de la signalisation. Les maillages sont également très utiles pour les géométries DWG complexes qui pourraient autrement affecter les performances de FormIt.

Les objets peuvent être convertis en maillages et les maillages peuvent être reconvertis en objets sans perte de données. Certains types de fichiers sont automatiquement importés en tant que maillages, par exemple, des fichiers OBJ, STL et DWG. Pour en savoir plus sur la conversion entre les types de maillage, ainsi que sur les autres avantages et limitations des maillages, reportez-vous aux sections ci-dessous.

### Conversion d’objets en maillages

Toute combinaison de sommets, d’arêtes, de faces ou de corps solides peut être convertie en maillages.

Il vous suffit de sélectionner des objets, puis d’utiliser le raccourci OM \(Objets en maillages\) ou de cliquer avec le bouton droit de la souris et de choisir Objects to Meshes dans le menu contextuel :

![](../.gitbook/assets/context-menu_object-to-mesh.PNG)

Une fois les objets convertis en maillages, un message de confirmation s’affiche en haut de l’écran :

![](../.gitbook/assets/success_object-to-mesh.PNG)

**Conversion d’objets en maillages :**

* Les arêtes qui ont été lissées sur les objets restent lissées dans les maillages obtenus.
* Les orientations des matériaux sur les objets restent inchangées dans les maillages obtenus.
* Un maillage est créé pour chaque matériau appliqué. Par exemple, si vous convertissez un cube unique peint de 6 couleurs différentes, vous obtiendrez 6 maillages différents.
   * La conversion en objet permet de recréer le joint des maillages individuels en un corps solide.
* La sélection d’un corps solide convertit et remplace le corps entier par un maillage, mais la sélection d’arêtes ou de sommets individuels appartenant à un solide crée un maillage au-dessus de la géométrie existante, sans affecter le corps d’origine.
* La conversion d’un jeu d’arêtes ou de sommets crée un maillage de ligne unique \(maillage constitué d’arêtes\) ou un maillage de points unique \(maillage constitué de points\), ce qui signifie que vous ne pourrez pas sélectionner des arêtes ou des sommets individuels une fois qu’ils auront été combinés en un maillage unique. Reconvertissez-les en objets si vous souhaitez ajuster la position d’un seul élément.

**Conversion d’une géométrie groupée en maillages :**

* Les maillages deviennent encore plus puissants lorsque vous convertissez un groupe entier et tous ses groupes imbriqués en maillages.
* Les groupes et leur contenu imbriqué peuvent être convertis en groupes à l’aide d’un plug-in :
   * Recherchez l’icône Plugin Manager située à droite de l’application :
      * ![](../.gitbook/assets/plugin-manager_icon.PNG)
   * Recherchez le plug-in Mesh + Unmesh All et cochez la case pour l’installer :
      * ![](../.gitbook/assets/plugin-manager_mesh-unmesh-all.PNG)
   * Le plug-in Mesh + Unmesh All se charge. Il vous suffit de sélectionner un groupe contenant les objets que vous souhaitez convertir en maillages, puis de cliquer sur Mesh All.
      * ![](../.gitbook/assets/mesh-unmesh-all-plugin.PNG)
   * Lors de la conversion d’objets imbriqués ou de maillages à l’aide de ce plug-in, un message de mise à jour s’affiche en haut de l’écran pour vous indiquer le nombre de groupes et d’occurrences de groupes affectés par l’opération :

![](../.gitbook/assets/success_mesh-all.PNG)

### Interaction avec les maillages

**En raison de leur optimisation, les maillages présentent les limitations et comportements suivants :**

* Vous ne pouvez pas modifier les faces, arêtes ou sommets individuels d’un maillage.
   * Toutefois, vous pouvez repeindre les maillages et déplacer les maillages individuels créés à la suite de l’application de différents matériaux aux faces \(reportez-vous aux sections ci-dessus\).
* L’accrochage aux maillages est limité aux faces et aux sommets des maillages. Pour des raisons de performances, l’accrochage et la déduction ne fonctionnent pas avec les arêtes des maillages.
   * Toutefois, les fichiers DWG convertis en maillages \(un autre type de maillage connu sous le nom de maillage de ligne\) conservent la possibilité d’accrocher et de déduire les arêtes de maillage.
* Il n’est pas possible d’appliquer des niveaux aux maillages.
* Les maillages ne signalent pas les problèmes d’étanchéité ou de faces arrière. Reconvertissez-les en objets pour vérifier s’ils sont étanches ou non.
   * Les objets qui étaient étanches avant la conversion en maillage le restent lors de la conversion en objet.
* Les maillages ne peuvent pas être utilisés dans des opérations de modélisation avancées, telles que les opérations de jonction/coupe de solide, de coque 3D, de décalage 3D, de congé, de lissage, de balayage ou de couverture.

Dans le cas contraire, les maillages s’affichent et se comportent comme n’importe quel autre objet FormIt : placés dans des groupes, affectés à des calques, visualisés dans des scènes, utilisés pour l’analyse, etc.

**Vous savez que vous interagissez avec un maillage si l’info-bulle indique « On Mesh » ou si le groupe de fonctions Properties indique un maillage :**

![](../.gitbook/assets/snap_on-mesh.PNG)

![](../.gitbook/assets/properties-panel_mesh.PNG)

**Certains types de fichiers sont automatiquement importés en tant que maillages pour améliorer les performances :**

* Les fichiers STL et OBJ, qui peuvent contenir une géométrie dense, comme les nuages de points d’autres applications, sont automatiquement importés en tant que maillages.
* Les fichiers DWG, qui peuvent contenir des millions de petits segments d’arête sur des courbes de haute qualité, sont automatiquement importés en tant que maillages.

### Reconversion des maillages en objets

Il vous suffit de sélectionner Meshes, puis d’utiliser le raccourci MO \(Maillages en objets\) ou de cliquer avec le bouton droit de la souris et de choisir Meshes to Objects dans le menu contextuel :

![](../.gitbook/assets/context-menu_mesh-to-object.PNG)

Une fois les objets convertis en maillages, un message de confirmation s’affiche en haut de l’écran :

![](../.gitbook/assets/success_mesh-to-object.PNG)

**Lors de la conversion de maillages en objets :**

* Tous les objets qui étaient auparavant solides/étanches avant la conversion en maillage sont joints en un solide étanche lors de la conversion en objet.
* La conversion d’une série d’arêtes \(par exemple à partir d’un fichier DWG\) ou d’une série de sommets \(par exemple à partir d’un nuage de points\) en maillage et inversement place automatiquement les objets non maillés dans un groupe.
   * Cela empêche la fusion des nouvelles arêtes ou des nouveaux sommets avec d’autres géométries, pouvant avoir des effets négatifs et des répercussions sur les performances.
   * Pour libérer les arêtes ou les sommets, il vous suffit de dissocier le groupe obtenu.

**Reconversion de maillages regroupés en objets :**

* Reportez-vous aux instructions ci-dessus pour utiliser le plug-in Mesh + Unmesh All afin de reconvertir les groupes et leurs maillages imbriqués en objets.

