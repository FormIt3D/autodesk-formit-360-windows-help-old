# Accrochages et déductions

Pour faciliter l’esquisse et la modélisation, utilisez les points d’accrochage et de déduction pour créer, placer et modifier la géométrie avec précision. Vous pouvez utiliser l’axe de votre choix comme axe sur lequel dessiner ou exécuter une autre action, telle que l’extrusion d’une surface.

**Remarque :** _reportez-vous à la rubrique_ [_Raccourcis clavier_](../appendix/keyboard-shortcuts.md) _pour savoir comment utiliser les outils du logiciel plus rapidement._

## Accrochage

Plusieurs accrochages peuvent vous aider lors de la création d’esquisses et de la modélisation. L’accrochage aux objets est automatiquement activé et vous pouvez effectuer un accrochage aux éléments suivants :

|                                                                                                                                                                            |                                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------ |
| Sommets | ![](<../.gitbook/assets/inf3 (3) (2).png>) |
| Arêtes. Lorsque vous placez le curseur sur l’arête, des petits points rouges sont dessinés aux extrémités et au milieu. | ![](../.gitbook/assets/inf4.png) |
| Milieux des arêtes | ![](../.gitbook/assets/inf5.png) |
| Plan d’une face. Lorsque vous passez le curseur sur la face, un petit point rouge est dessiné au niveau du centre de gravité de la face. Cela vous permet de trouver facilement ce point si vous souhaitez y effectuer un accrochage. | ![](../.gitbook/assets/inf6.png) |
| Centres de gravité des faces | ![](../.gitbook/assets/inf7.png) |
| Plan de construction, si vous ne n’effectuez d’accrochage à rien d’autre. | ![](../.gitbook/assets/inf8.png) |
| Centres de cercle ou d’arc | ![](../.gitbook/assets/inf9.png) |
| Sommets de maillage | ![](../.gitbook/assets/inf2.png) |
| Plan d’une facette de maillage. | ![](../.gitbook/assets/inf1.png) |

Pour effectuer un accrochage à la grille, vous devez activer le paramètre **Accrocher à la grille (SG)** dans le menu Paramètres.

## Axes et points de déduction

La sélection automatique des points de déduction est toujours activée et vous permet de contraindre le mouvement de la géométrie. Les axes de déduction sont générés automatiquement par les outils ou lorsque vous passez la souris sur des arêtes ou des points. Les axes de déduction sont toujours dessinés à l’écran avec des tirets, ce qui vous permet de savoir où ils se trouvent et de les accrocher facilement.

**Axe :** vous pouvez déplacer la géométrie le long de l’axe X, Y ou Z. La déduction de l’axe X apparaît en rouge, celle de l’axe Y en vert et celle de l’axe Z en bleu.

![](../.gitbook/assets/inf10.png)

**Verrouillage de l’axe :** vous pouvez verrouiller le mouvement le long des axes X, Y ou Z. Maintenez la touche Maj enfoncée pendant que vous êtes sur une déduction d’axe, puis déplacez la souris pour accrocher et déduire d’autres éléments.

![](../.gitbook/assets/inf13.png)

**Parallèle :** vous pouvez esquisser ou déplacer une géométrie parallèlement aux éléments existants. Les déductions perpendiculaires sont violettes. Vous devez placer le curseur sur une ligne que vous souhaitez utiliser comme référence parallèle.

![](../.gitbook/assets/inf14.png)

**Perpendiculaire :** vous pouvez également dessiner ou déplacer une géométrie perpendiculairement aux éléments existants. Les déductions perpendiculaires sont violettes. Vous devez placer le curseur sur une ligne que vous souhaitez utiliser comme référence perpendiculaire.

![](../.gitbook/assets/inf15.png)

**Prolongement à partir d’un point :** vous pouvez également utiliser des déductions afin d’effectuer un prolongement à partir d’un point de référence. Placez le curseur de la souris sur un point que vous souhaitez utiliser comme référence jusqu’à ce que l’info-bulle s’affiche, puis utilisez l’axe de déduction qui s’étend à partir du point.

![](../.gitbook/assets/inf16.png)

**Centre des cercles** : si vous souhaitez effectuer un accrochage au centre d’un arc ou d’un cercle, placez le curseur sur l’arc ou le cercle. Un petit point rouge apparaît au centre. Si vous vous éloignez de l’arc ou du cercle, il reste visible pendant environ 5 secondes. Déplacez le curseur sur le point rouge pour l’accrocher au centre.

![](../.gitbook/assets/inf17.png)

**Milieux d’arcs et de splines** : lorsque vous placez le curseur sur un cercle, un arc ou une spline, vous pouvez effectuer un accrochage au milieu. Le milieu et les extrémités sont représentés par un petit point rouge. Lorsque vous appliquez une déduction à un arc, vous effectuez aussi un accrochage aux sommets des arêtes droites qui représentent l’arc.

![](../.gitbook/assets/inf18.png)

**Suppression des déductions** : il est possible que le dessin génère un plus grand nombre de déductions, ce qui peut empêcher le placement de points qui ne sont pas censés s’accrocher à ces déductions. Si vous appuyez sur les touches **Maj + Espace**, toutes les déductions sont effacées, à l’exception de celles du dernier point placé.

![Avant d’effacer les déductions](../.gitbook/assets/inf19.png)

![Après avoir effacé les déductions](../.gitbook/assets/inf20.png)
