# 1.6 – Contrôle de la visibilité avec les calques

_Comme dans AutoCAD et Photoshop, les calques dans FormIt vous permettent de gérer la visibilité des objets dans votre modèle. Dans ce chapitre, nous allons créer un calque pour enregistrer et masquer le volume du bâtiment en vue d’une analyse ultérieure._

_Si vous n’avez pas terminé la dernière section, téléchargez et ouvrez le fichier __**1.6 - Control Visibility with Layers.axm**__ à partir du dossier_ _**Jeux de données Partie I FormIt Primer**._

## **Créer des calques**

1 – Pour créer de nouveaux calques, procédez comme suit :

1. Accédez à la **palette Calques** et cliquez trois fois sur le signe **+** pour créer trois calques.
2. Double-cliquez sur les noms des calques pour les renommer **Volume**, **Sol du bâtiment principal** et **Image du plan.**

![](../../.gitbook/assets/0%20%2820%29.png)

_**Remarque :**_ _vous pouvez cliquer sur un nom de calque et le faire glisser vers le haut ou vers le bas pour réorganiser les calques._

2 – Pour affecter le groupe **Volume – Bâtiment principal** au calque **Volume** :

1. Dans la zone de dessin, sélectionnez le groupe **Volume – Bâtiment principal**.
2. Dans la **palette des calques**, choisissez le calque **Volume** dans le menu déroulant « **Sélection activée :** ». De même, affectez le groupe **Image du plan** au calque **Image du plan**.

![](../../.gitbook/assets/1%20%2813%29.png)

## **Dupliquer le groupe**

_Nous allons maintenant commencer à modéliser le bâtiment plus en détail. La première étape consiste à créer la géométrie du sol en fonction du volume du bâtiment que nous avons déjà._

1 – Sélectionnez à nouveau le groupe **Volume – Bâtiment principal**. Appuyez sur **Ctrl + C \(Copier\)** pour copier, puis sur **Ctrl + Maj + V \(Coller sur place\)** pour coller le volume au même endroit.

2 – Pour dissocier la nouvelle géométrie de groupe du groupe d’origine : cliquez avec le bouton droit de la souris pour accéder au **menu contextuel**, puis choisissez l’option **Rendre unique \(MU\)**.

![](../../.gitbook/assets/2%20%2818%29.png)

_**Remarque** : le nouveau groupe n’est plus associé à l’original. Les modifications apportées au nouveau groupe ne modifieront pas le groupe d’origine._

## **Création de la géométrie du sol**

1 – Réaffectez le calque du groupe comme suit :

1. Cliquez une fois pour sélectionner l’un des groupes **Volume – Bâtiment principal**.
2. Placez le groupe sur le calque **Sol du bâtiment principal** à l’aide de la liste déroulante « **Sélection activée :** » de la **palette des calques**.
3. Désactivez le calque **Volume** pour masquer sa géométrie et la protéger contre les modifications accidentelles.

![](../../.gitbook/assets/3%20%2818%29.png)

2 – Double-cliquez sur le groupe visible **Volume – Bâtiment principal** pour le modifier. Renommez le groupe **Sol** dans la **palette Propriétés**.

![](../../.gitbook/assets/4%20%2812%29.png)

3 – **Cliquez une fois** sur la **face supérieure** de la géométrie pour la sélectionner. Cliquez à nouveau et commencez à faire glisser la face vers le bas. Lorsque vous faites glisser la face vers le bas, tapez **11’-2"**. La **boîte de dialogue Cotation** s’affiche. Cliquez sur **OK** après avoir entré la valeur. Le sol obtenu doit avoir une épaisseur de 1’. Double-cliquez dans l’espace pour quitter le groupe.

![](../../.gitbook/assets/5%20%2810%29.png)

