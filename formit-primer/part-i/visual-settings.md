# 1.12 – Styles visuels

_La modélisation de volumes conceptuels représente seulement la moitié des fonctionnalités de FormIt. L’autre moitié sont de superbes graphiques qui aident à raconter une histoire à un client ou à un membre d’équipe. Dans ce chapitre, nous allons aborder les méthodes permettant de configurer vos_ _**styles visuels graphiques**_ _et de créer des animations._

_Si vous n’avez pas terminé la dernière section, téléchargez et ouvrez le fichier_ _**1.12 – Visual Styles.axm**_ _à partir du dossier_ _**Jeux de données Partie I FormIt Primer **._

## **Création d’une animation**

_Dans les étapes suivantes, nous allons apprendre à utiliser les_ _**scènes**_ _pour créer une animation._

1 – Pour créer la première **scène**, procédez comme suit :

1. Activez tous les calques, à l’exception de **Terrain**, **Image du plan** et **Volume**.
2. Assurez-vous que le mode de caméra est défini sur **Perspective \(VP\)** et positionnez la caméra légèrement au-dessus de la maison de façon à la visualiser dans son ensemble, comme dans l’image ci-dessous.
3. Ouvrez la **palette Scènes**.
4. Cliquez sur l’icône **+** pour créer une scène à partir de la vue active.
5. Renommez-la **Aerial View 1** et faites correspondre les autres **propriétés de la scène** à celles indiquées dans l’image ci-dessous.

![](../../.gitbook/assets/0%20%2817%29.png)

2 – Pour créer la deuxième **scène**, puis une animation entre elles, procédez comme suit :

1. Ajustez la caméra afin de visualiser la maison sous un autre angle. Créez une **scène** nommée **Aerial View 2** à l’aide de la procédure suivie à l’étape précédente.
2. Cliquer sur le bouton **Play**. Après la définition du **temps de pause** sur **2 secondes**, l’animation démarre lentement, en se déplaçant d’avant en arrière entre les deux scènes. Cette opération se poursuit jusqu’à ce que vous cliquiez sur le bouton **Arrêter** pour arrêter l’animation.

![](../../.gitbook/assets/1%20%2812%29.png)

_**Remarque :**_ _vous pouvez ajuster le_ _**temps de pause**, le_ _**temps de transition** et le_ _**temps de caméra**_ _à l’aide des paramètres situés dans la partie inférieure des_ _**propriétés de la scène.**. Essayez d’ajouter d’autres scènes et d’ajuster ces paramètres pour personnaliser votre animation._

## **Personnalisation des styles visuels**

_Nous allons maintenant créer une autre scène avec des paramètres personnalisés de **styles visuels**._

1ؘ – Tout d’abord, ouvrez la **palette Styles visuels**. Notez qu’il existe quatre \(4\) onglets dans la partie supérieure, chacun contenant des paramètres visuels différents : **Surfaces**, **Arêtes**, **Environnement** et **Diagnostics du modèle**. Pour en savoir plus sur chaque onglet, consultez le chapitre **Styles visuels** de la section **Bibliothèque d’outils**.

2 – Pour personnaliser certains paramètres dans l’**onglet Surface**, procédez comme suit :

1. Activez l’option **Ombres \(DS\)**.
2. Activez l’option **Ombres ambiantes \(DA\)**.
3. Activez l’option **Surfaces monotones \(DM\)**. Cette opération crée une image abstraite en noir et blanc sans aucun matériau.

![](../../.gitbook/assets/2%20%2820%29.png)

3 – Pour personnaliser certains paramètres dans l’**onglet Arête**, procédez comme suit :

* 
   1. Réglez les curseurs afin d’éclaircir le contraste des **arêtes** à environ **30 %**.
   2. Activez l’option **Prolonger les arêtes \(DX\).**
   3. Réglez les curseurs afin d’éclaircir le contraste des **silhouettes** à **30 %**.

![](../../.gitbook/assets/3%20%2811%29.png)

4 – Pour personnaliser certains paramètres dans l’**onglet Environnement**, procédez comme suit :

1. Désactivez l’option **Axes**.
2. Si l’option **Niveaux** est activée, désactivez-la.

![](../../.gitbook/assets/4%20%288%29.png)

5 – Créez une scène nommée **Scène personnalisée** pour enregistrer ces paramètres. Vous pouvez maintenant basculer entre les **scènes** pour réinitialiser les paramètres graphiques.

![](../../.gitbook/assets/5%20%286%29.png)

_**Remarque** : si vous désactivez la propriété_ _**Caméra**_ _de la nouvelle scène, vous pouvez l’utiliser uniquement pour activer les paramètres visuels que nous venons de créer sans déplacer la position de la caméra. Pour essayer, accédez à l’une de vos scènes aériennes précédentes, puis double-cliquez sur la_ _**scène personnalisée**_ _et observez ce qu’il se passe._

_**Remarque :**_ _pour en savoir plus sur les_ _**diagnostics de styles visuels**_ _et les applications avancées pour les_ _**scènes**, consultez la_ _partie II du guide**.**_

