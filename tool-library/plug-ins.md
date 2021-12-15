# Modules d’extension

Utilisez Plugin Manager pour installer des plug-ins utiles de l’équipe FormIt ou découvrez comment [**créer vos propres plug-ins FormIt**](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html)**.**

#### FormIt Plugin Manager

FormIt Plugin Manager fonctionne comme un hub permettant de découvrir et de gérer des plug-ins FormIt.

Plugin Manager est chargé automatiquement au démarrage de FormIt, à condition que FormIt ait accès à Internet.

Vous pouvez accéder au gestionnaire de plug-ins en cliquant sur l’icône de son onglet située sur le côté droit de la fenêtre de l’application :

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/PluginManagerTab.PNG)

#### Plugin Manager classe les différents types de plug-ins :

* **Plug-ins installés**
* **Plug-ins recommandés**
   * Les plug-ins recommandés par l’équipe FormIt permettent de développer les fonctionnalités de base de FormIt et de déverrouiller de nouveaux workflows.
   * Les plug-ins développés par la communauté apparaissent ici après avoir été approuvés par l’équipe FormIt. Plus de détails à venir sur ce sujet.
* **Plug-ins publics**
   * Plug-ins créés par la communauté, mais qui n’ont pas été vérifiés ou approuvés par l’équipe FormIt.

#### Plugin Manager est conçu à l’aide d’une série d’interfaces développables et réductibles, ce qui facilite la gestion des plug-ins et de leurs référentiels :

* **Gestion des plug-ins :**
   * Cliquez sur un nom de plug-in pour en afficher la description.
   * Activez ou désactivez le commutateur pour installer ou désinstaller le plug-in.
      * Le plug-in se manifeste sous la forme d’une barre d’outils située dans la partie supérieure de l’application, d’un groupe de fonctions situé sur la droite ou d’une boîte de dialogue située au milieu, selon le type de plug-in.
* Si vous [développez votre propre plug-in](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html), vous pouvez ajouter son URL privée dans le champ situé en bas et cliquer sur \(+\) :

![FormIt Plugin Manager](https://formit3d.github.io/FormItExamplePlugins/docs/images/addNew.png)

#### Fonctionnement des plug-ins

* Les plug-ins sont basés sur le Web et disponibles dans FormIt pour Windows et FormIt pour le Web.
* Les plug-ins sont constitués d’une série de fichiers et de dossiers hébergés sur GitHub ou sur un serveur local lors de la création de votre propre fichier.
* Étant donné que les plug-ins externes \(plug-ins non hébergés localement\) nécessitent une connexion Internet pour se charger, les points suivants s’appliquent :
   * Les plug-ins externes ne se chargent pas si aucune connexion Internet n’est détectée au démarrage de FormIt.
   * Une fois chargés, certains plug-ins externes peuvent continuer à travailler en mode hors ligne pour cette session, mais d’autres peuvent se bloquer jusqu’à ce que la connectivité soit restaurée.
   * Les plug-ins externes chargent le dernier code sur le serveur à chaque exécution, de sorte que leur fonctionnalité est mise à jour chaque fois que l’auteur apporte une modification.
* Étant donné que ces plug-ins sont chargés de façon asynchrone, l’ordre des plug-ins dans l’interface FormIt peut changer dans chaque nouvelle session.
* Plugin Manager utilise les clés de registre de Windows pour stocker les référentiels et les plug-ins installés.
   * Si vous devez restaurer les paramètres par défaut de votre Plugin Manager, supprimez la clé de registre suivante :
      * Computer\HKEY\_CURRENT\_USER\Software\Autodesk\FormIt 360\Plugins
      * Notez que cette action entraîne la désinstallation de tous les référentiels et plug-ins ajoutés par l’utilisateur, réinitialisant ainsi Plugin Manager afin d’inclure uniquement les référentiels et plug-ins intégrés.

