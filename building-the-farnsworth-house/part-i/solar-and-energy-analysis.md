# Analyse d’énergie et d’ensoleillement

Maintenant que le modèle a été créé, nous pouvons l’utiliser pour étudier l’**impact solaire et énergétique** de notre conception. Ces fonctions sont intégrées à FormIt afin que vos premières études puissent être comprises du point de vue des performances du bâtiment. Ces fonctionnalités sont disponibles uniquement dans **FormIt Pro**. Si vous suivez les instructions de l’application Web, vous n’y aurez peut-être pas accès.

Si vous n’avez pas terminé la dernière section, cliquez sur Fichier > Ouvrir et choisissez **farnsworth08.axm** dans le dossier FormIt Primer.

## Ombres

Avant d’utiliser ces outils d’analyse, vous devez [définir l’emplacement](). FormIt peut ainsi accéder à des données précises sur le soleil, les ombres et le climat.

1. Cliquez sur l’icône du soleil dans la [**barre d’outils Action**](../../formit-introduction/tool-bars.md) et activez **Ombres \(DS\)**.

   ![](../../.gitbook/assets/3bdf0e2a-0ad4-4aac-b6fc-5e789643b0d6.png)

2. Réglez les curseurs **Jour** et **Temps** pour observer la variation des ombres.

   ![](../../.gitbook/assets/upperterracesketch_32.png)

3. Notez que la terrasse couverte est ombragée pendant les heures les plus chaudes de l’été : ce n’est certainement pas un accident, mais une question de conception !

**Remarque** : les ombres peuvent entraîner une baisse des performances de l’application. Pour tenter de résoudre ce problème, essayez l’une des méthodes suivantes : désactivez les ombres si la navigation devient lente ou désactivez les calques tels que le **mobilier** s’ils ne sont pas nécessaires à l’étude des ombres.

## Analyse d’ensoleillement

En tant que personnes visuelles, les concepteurs peuvent apprendre et communiquer une quantité incroyable d’informations à partir de diagrammes de carte thermique comme celui que nous sommes sur le point de créer.

1. Dans la partie inférieure du [**menu Soleil**](../../formit-introduction/tool-bars.md), cliquez sur le bouton **Analyse d’ensoleillement**.
2. Vous passez dans un mode spécial où les **ombres**, les **raccourcis clavier** et les autres **barres d’outils** sont désactivés.
3. En mode **Analyse d’ensoleillement**, le comportement de sélection est différent. Vous pouvez sélectionner les **groupes**, vous n’avez pas besoin de maintenir la touche **Ctrl** ou **Maj** enfoncée pour ajouter des éléments à votre jeu de sélection, et vous pouvez désélectionner des éléments en cliquant à nouveau dessus. Vous pouvez **cliquer une fois**, **double-cliquer** ou **sélectionner** une géométrie dans une fenêtre.
4. Choisissez les faces que vous souhaitez étudier. **Cliquez une fois** sur la partie supérieure du **toit** et sur la partie supérieure des **étages**. Évitez de sélectionner de petits éléments tels que du mobilier.

   ![](../../.gitbook/assets/upperterracesketch_33.png)

5. Dans le coin supérieur gauche de la zone de dessin, recherchez la barre d’outils **Analyse d’ensoleillement**. Cliquez sur **Analyser**. FormIt calcule et effectue le rendu des surfaces. Les paramètres peuvent être ajustés avant **et** une fois l’analyse terminée.

   ![](../../.gitbook/assets/solaranalysis.png)

6. Le paramètre **
   Pic du mois** affiche les valeurs de **pic** \(en BTU/pi²\) pour le mois spécifié. Il sert aux **études d’ombrage**. Lorsque vous modifiez le paramètre du mois, le graphique est instantanément mis à jour. **Placez le curseur** sur une surface analysée pour obtenir une valeur **spécifique**.

   ![](../../.gitbook/assets/460060a0-ea3b-4095-af45-40045811be22.png)

7. Le paramètre **Cumul année** affiche l’énergie **cumulée** pour l’année entière \(en KwH/m²\). Il sert aux **études de potentiel PV**.

   ![](../../.gitbook/assets/a9f61dfb-dfc9-4751-b145-b131a69c53cf.png)

8. Pour exporter ces études d’**analyse d’ensoleillement**, cliquez sur **Fichier > Exporter \(Ctrl + E\)** et sélectionnez **Image** dans la liste de gauche.

## Analyse d’énergie avec Insight

FormIt est doté des mêmes outils d’analyse des performances du bâtiment que Revit. **Insight** fournit un tableau de bord des paramètres du système de bâtiment qui peuvent être ajustés afin de refléter les scénarios potentiels sans devoir **réanalyser** la géométrie du modèle. Insight fonctionne mieux avec la géométrie de **volume** FormIt.

1. Vérifiez que vous êtes connecté à votre compte Autodesk Account. Désactivez **tous** les calques, **à l’exception** du calque **Volume**. Au moins un **niveau** doit être appliqué à la géométrie.
2. FormIt envoie uniquement la géométrie **visible** à Insight. Notez que même un simple **volume** génère une mine de données à partir d’**Insight**.

   ![](../../.gitbook/assets/energymassing.png)

3. Cliquez sur le bouton **Insight > Générer Insight**. Étant donné que l’analyse s’exécute dans le cloud, vous pouvez continuer à effectuer des modélisations pendant le calcul.

   ![](../../.gitbook/assets/energymenu.png)

4. Une fois l’analyse terminée, cliquez sur le bouton **Afficher Insight** pour afficher votre **modèle énergétique** et les **facteurs de performances** (vous pouvez éventuellement visiter le site Web directement à l’adresse [**http://insight.autodesk.com**](http://insight.autodesk.com/)\).

   ![](../../.gitbook/assets/energydashboard.png)

5. Dans le tableau de bord Insight, pour définir une valeur \(ou une plage de valeurs\) pour chaque widget **Facteur de performance**, cliquez sur le facteur et faites glisser les points bleus. La plage est utile si vous ne connaissez pas encore le système spécifique utilisé pour votre bâtiment.
6. Chaque modification apportée à un **facteur** entraîne la mise à jour de la **plage de coûts énergétiques** (mesurée en USD/m²/an\). Vous pouvez comparer les performances de votre conception aux références comme **Ashrae 90.1** et le défi **Architecture 2030**.
7. Si votre conception change radicalement, vous pouvez renvoyer le volume mis à jour vers le même tableau de bord. Si vous souhaitez créer un **autre** tableau de bord pour la conception mise à jour, vous devez d’abord effectuer un enregistrement à l’aide de l’option **Enregistrer sous** dans FormIt.
8. Si l’analyse d’énergie échoue, vous pouvez avoir des **problèmes d’étanchéité \(DW\)** basés sur la géométrie. Ceux-ci peuvent être vérifiés et corrigés dans FormIt.
9. Désactivez le calque **Volume** et réactivez tous les autres calques.

