# Droite décalée

Dessinez des lignes parallèles ou de décalage à l’aide de l’outil Décaler la ligne. Cet outil permet de créer des formes 2D qui peuvent ensuite être extrudées pour ressembler à des murs 3D.

![](../.gitbook/assets/image%20%283%29.png)

L’outil **Décaler la ligne** fonctionne comme l’outil [**Ligne**](https://windows.help.formit.autodesk.com/tool-library/line-tool) :

* Cliquez pour définir le premier point, puis déplacez le curseur et placez les points suivants, en les accrochant à la géométrie existante ou aux axes de déduction.
* Un aperçu de la forme obtenue est affiché. Les deuxième et troisième points déterminent le plan pour le reste des points à suivre, de sorte que le résultat soit planaire.
* Continuez d’ajouter des points, puis appuyez sur la touche **Échap** ou double-cliquez pour terminer l’outil.
* Toutes les auto-intersections seront nettoyées et fusionnées afin d’obtenir une face extrudable.

![Après avoir placé 2 points et fait glisser le troisième point](../.gitbook/assets/walls1.png)

La ligne d’entrée est dessinée en rouge et est placée par défaut au centre des lignes de décalage.

Pour modifier l’alignement des lignes de décalage et leur épaisseur, appuyez sur la touche **Tab**. La boite de dialogue **Options d’outil** s’affiche également :

![Options de l’outil Décaler la ligne](../.gitbook/assets/walls2.png)

Par exemple, définissez l’option **Alignement** sur **Gauche** et l’option **Épaisseur** sur 6” : les lignes de décalage sont dessinées à gauche des lignes d’entrée, à 6 pouces les unes des autres.

![](../.gitbook/assets/walls3.png)

## Conseils utiles

Vous pouvez dessiner une forme fermée en l’accrochant au premier point placé. Le coin obtenu est nettoyé automatiquement :

![](../.gitbook/assets/walls4.png)

Vous pouvez dessiner librement les lignes d’entrée les unes sur les autres. Lorsque l’outil est terminé, les intersections obtenues sont nettoyées.

![](../.gitbook/assets/walls5.png)

![](../.gitbook/assets/walls6.png)

Par nature, l’outil Décaler la ligne doit générer une géométrie sur un plan, de sorte que les premiers points déterminent le plan sur lequel les autres points suivront.

Tout d’abord, dessinez sur le côté d’un cube, par exemple, pour utiliser le plan de cette face. Une fois que trois points non colinéaires sont placés, le plan d’entrée est fixe pour le reste de l’entrée. Notez que lorsque vous dessinez sur une face, la forme obtenue est insérée dans la face, ce qui la divise en plusieurs faces. Pour empêcher l’insertion, la face sur laquelle vous dessinez doit faire partie d’un [groupe](https://windows.help.formit.autodesk.com/tool-library/groups).

![Dessin sur une face verticale](../.gitbook/assets/walls7.png)

![Une fois l’outil terminé, les lignes sont insérées et les faces scindées peuvent être manipulées davantage](../.gitbook/assets/walls8.png)

Vous pouvez également utiliser l’outil Décaler la ligne pour tracer à partir d’un dessin en plan. Importez le plan en tant qu’image.

* Redimensionnez l’image de sorte que le plan soit à l’échelle appropriée. Pour en savoir plus, [cliquez ici](https://windows.help.formit.autodesk.com/building-the-farnsworth-house/work-with-images-and-the-ground-plane).
* Vous pouvez utiliser la [caméra orthogonale](orthographic-camera.md) pour effectuer un tracé dans une [vue de dessus](orthographic-views.md) orthogonale.

![](../.gitbook/assets/walls9.png)

![](../.gitbook/assets/walls10.png)



