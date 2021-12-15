# Enregistrement automatique

À partir de la version v17.3, FormIt pour Windows inclut la fonction Enregistrement automatique, permettant de créer une copie de sauvegarde de votre modèle FormIt pendant que vous travaillez. Ce fichier de sauvegarde peut être utilisé pour récupérer des données si FormIt se ferme avec des modifications non enregistrées.

### Activation/désactivation de la fonction Enregistrement automatique

Recherchez les options de configuration de la fonction Enregistrement automatique dans Modifier > Préférences > Enregistrement automatique.

![](../.gitbook/assets/20190613-autosave.png)

La fonction Enregistrement automatique est activée par défaut. Pour la désactiver complètement, il vous suffit de décocher la case.

Pour définir l’intervalle \(en minutes\) auquel l’enregistrement automatique effectuera une copie de sauvegarde, saisissez une valeur dans la case numérique « Intervalle d’enregistrement automatique ».

Notez que ces préférences sont définies au niveau de l’application et ne changent pas lors de l’ouverture de différents fichiers.

### Fonctionnement de la fonction Enregistrement automatique

Lorsque la fonction Enregistrement automatique est activée, elle détermine si le fichier FormIt actif contient des modifications non enregistrées. Si des modifications ne sont pas enregistrées, l’enregistrement automatique crée une copie de sauvegarde du fichier à l’intervalle spécifié.

Les fichiers de sauvegarde sont stockés à côté du fichier d’origine et portent l’extension `.axmb`.

Par exemple, si votre fichier FormIt d’origine est stocké dans `C:/Users/<user>/FormIt/MyProject.axm`, le fichier de sauvegarde se trouve dans `C:/Users/<user>/FormIt/MyProject.axmb`.

Si vous démarrez une nouvelle session FormIt sans ouvrir de fichier existant, les modifications non enregistrées sont disponibles à l’adresse `C:/Users/<user>/Documents/Untitled.axmb`. Une fois le nouveau modèle enregistré dans un autre emplacement, la sauvegarde commence à ajouter des modifications non enregistrées à côté du nouvel emplacement, comme indiqué ci-dessus.

Lorsque vous enregistrez les modifications apportées au fichier d’origine, l’enregistrement automatique supprime automatiquement le fichier de sauvegarde, car la sauvegarde est désormais plus ancienne que le fichier d’origine. Toutefois, si vous apportez des modifications ultérieures au fichier enregistré, l’option d’enregistrement automatique vous invite à recommencer la sauvegarde à l’intervalle spécifié.

Si votre fichier de travail comporte des modifications non enregistrées et que vous décidez de fermer FormIt et d’ignorer les modifications, la sauvegarde d’enregistrement automatique sera supprimée. Toutefois, si FormIt doit se fermer (soit par un arrêt de l’ordinateur, soit par un blocage de l’application), le fichier de sauvegarde d’enregistrement automatique est conservé et peut être utilisé ultérieurement pour récupérer des données.

### Utilisation de la fonction Enregistrement automatique

FormIt minimise l’impact potentiel de l’enregistrement automatique sur les performances en exécutant la sauvegarde dans un processus distinct. Dans le cas de fichiers de petite et de moyenne taille, vous ne devriez pas remarquer quand la fonction Enregistrement automatique effectue une sauvegarde. Dans le cas de fichiers très volumineux \(400 Mo environ et plus\), vous pouvez remarquer une pause momentanée pendant que FormIt copie le modèle entier et commence la sauvegarde dans un processus distinct.

Si vous souhaitez savoir si un enregistrement automatique est en cours, consultez la barre d’état située dans la partie inférieure gauche de l’application pour vérifier si le message d’enregistrement automatique suivant est affiché :

![](../.gitbook/assets/20190613-autosave-status-bar.png)

Si votre barre d’état est désactivée, activez-la dans Windows > Barre d’état ou via le raccourci HS.

### Récupération de données avec la fonction Enregistrement automatique

Lorsque vous ouvrez un fichier FormIt pour lequel une sauvegarde est disponible, FormIt vous avertit que le fichier de sauvegarde existe. Comme indiqué ci-dessus, cela peut être dû à la fermeture de FormIt sans que vous ayez choisi d’enregistrer les modifications apportées à ce projet lors de sa dernière modification ou à la fermeture inattendue de FormIt.

![](../.gitbook/assets/20190613-autosave-notification.png)

Cliquez sur l’hyperlien « Ouvrir ? » pour charger le fichier de sauvegarde `.axmb`.

De même, vous pouvez utiliser Fichier > Ouvrir et sélectionner manuellement le fichier `.axmb` dans l’explorateur de fichiers pour ouvrir une sauvegarde.

Une fois le fichier de sauvegarde ouvert, la prochaine fois que vous l’enregistrerez, FormIt vous demandera de choisir un autre fichier FormIt \(`.axm`\) à remplacer. Vous ne pouvez pas remplacer les fichiers de sauvegarde FormIt \(`.axmb`\).



