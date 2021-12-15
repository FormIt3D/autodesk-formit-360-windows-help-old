# Groupes

L’une des techniques les plus élémentaires, mais importantes, des workflows FormIt concerne le groupement. Les groupes vous permettent d’éviter que la géométrie ne reste collée et de définir des relations parent/enfant entre les éléments copiés. De ce fait, si vous mettez à jour un élément, les deux éléments sont mis à jour. Pour en savoir plus sur les groupes, cliquez [ici](../formit-primer/part-i/grouping-objects.md).

Les groupes peuvent être créés et modifiés de deux manières : à partir du menu contextuel d’un groupe sélectionné ou à partir de la barre d’outils principale.

## Interactions des groupes

Pour **créer un groupe**, sélectionnez les éléments que vous souhaitez regrouper (arêtes, faces, solides ou autres groupes) et cliquez avec le bouton droit de la souris. Choisissez l’outil **Grouper \(G\)** dans le menu contextuel. Les images importées et les images satellites ne peuvent pas être regroupées.

Pour **sélectionner un groupe**, cliquez une fois sur le groupe. Lorsque vous sélectionnez un groupe, des lignes en pointillés apparaissent. Elles indiquent la taille totale du groupe.

Pour **modifier un groupe**, double-cliquez sur le groupe. Cette opération permet de lancer un mode de modification dans lequel vous pouvez uniquement afficher et accrocher des éléments situés en dehors du groupe actuel, mais pas les sélectionner. Vous pouvez également masquer les éléments situés en dehors du groupe actuel à l’aide du raccourci clavier **H**.

Vous pouvez créer des **groupes dans des groupes** : ils sont appelés **groupes imbriqués** et peuvent être créés dans le mode de modification de groupe. Pour monter d’un niveau dans les groupes imbriqués, cliquez n’importe où en dehors des groupes.

Pour **quitter le mode de modification de groupe**, double-cliquez n’importe où en dehors du groupe.

Vous pouvez **copier un groupe** pour créer une relation entre le groupe d’origine et sa copie : si vous modifiez un groupe copié, les mêmes modifications affecteront tous les groupes associés.

Pour **rompre la relation entre les groupes copiés**, sélectionnez les groupes que vous souhaitez séparer, cliquez avec le bouton droit de la souris, puis choisissez **Rendre unique** dans le menu contextuel. Vous pouvez également sélectionner Rendre unique dans la barre d’outils Groupes.

Pour **sélectionner tous les groupes associés**, placez le curseur sur un groupe et appuyez sur la touche Tab. Lorsque tous les groupes associés sont mis en surbrillance, cliquez sur les groupes pour les sélectionner. Vous pouvez ensuite effectuer une action sur tous les groupes à la fois.

L’[**arborescence des groupes**](groups-tree.md) fournit un emplacement unique pour afficher et gérer tous les groupes d’un projet.

## Accès au menu contextuel et à la barre d’outils Groupes

## ![](../.gitbook/assets/grouptoolbar.png)

**Groupement d’éléments**

Pour créer un groupe à partir de la barre d’outils Groupes, sélectionnez un ou plusieurs éléments, cliquez sur l’icône **Créer un groupe**, puis sur l’icône **Terminer**. Vous pouvez également sélectionner **Créer un groupe** dans la barre d’outils Groupes, puis sélectionner les éléments que vous souhaitez regrouper et cliquer sur l’icône **Terminer**.

Pour **modifier un groupe depuis la barre d’outils Groupes**, sélectionnez l’icône **Modifier le groupe**, puis cliquer sur le groupe que vous voulez modifier. Quand vous avez terminé les modifications, sélectionnez l’icône **Modifier le groupe**. Cet outil vous permet de choisir le groupe spécifique que vous souhaitez modifier, même s’il est profondément imbriqué.

**Pour rendre un groupe unique à partir de la barre d’outils,** sélectionnez l’icône **Rendre unique** dans la barre d’outils Groupes. En outre, vous pouvez sélectionner **Rendre unique** dans la barre d’outils Groupes, puis sélectionner le groupe que vous souhaitez rendre unique et cliquer sur l’icône **Terminer**.

**Pour dissocier un groupe de la barre d’outils Groupes,** sélectionnez le groupe à modifier et choisissez l’icône **Dissocier** dans le menu de la barre d’outils Groupes. Cet outil permet de dissocier votre sélection actuelle, mais ne dissocie aucun groupe imbriqué. Sinon, sélectionnez **Dissocier** dans la barre d’outils, le groupe que vous voulez changer, puis cliquez sur l’icône **Terminer**.

**Pour dissocier tous les groupes imbriqués sous le groupe sélectionné,** sélectionnez un groupe avec des groupes imbriqués et choisissez **Dissocier tous les groupes imbriqués** dans la barre d’outils Groupes.

**Pour dissocier tous les groupes du modèle, **sélectionnez l’outil **Tout dissocier** dans la barre d’outils Groupes.

## Groupes et Revit

Si vous connaissez les **familles** Revit, vous connaissez le concept de groupes dans FormIt. Les groupes FormIt possèdent des fonctions que vous pouvez utiliser pour les transférer intelligemment dans Revit.

**Catégories de groupes FormIt**

Vous pouvez spécifier les **catégories** des groupes dans FormIt afin que vos groupes FormIt deviennent des familles des mêmes catégories lorsque vous les importez dans Revit. Pour affecter des catégories à vos groupes FormIt, sélectionnez un groupe, passez en mode de **modification de groupe** et utilisez le groupe de fonctions **Propriétés** pour choisir des catégories. Vous pouvez également affecter des catégories dans le groupe de fonctions **Arborescence des groupes**.

**Noms de groupes FormIt**

Vous pouvez également utiliser le groupe de fonctions **Propriétés** pour spécifier un nom pour votre groupe FormIt. Cela peut être utile pour naviguer dans votre propre modèle. De plus, quand vous importez votre modèle dans Revit, vous pouvez facilement filtrer les éléments en utilisant le nom du groupe.

Notez que les **groupes imbriqués dans FormIt ne sont pas importés dans Revit en tant que groupes imbriqués**. Cela empêche l’imbrication des familles Revit.

