# Création de facettes de courbe et de surface

FormIt est un système de modélisation polyédrique. Les objets tels que les cercles, les arcs et les splines sont donc représentés par une série d’arêtes droites. De même, une surface incurvée, comme la paroi d’un cylindre ou d’un dôme, est constituée d’une série de faces planes avec des arêtes de bordure masquées.

Par défaut, FormIt utilise 40 arêtes, ou facettes, pour représenter un cercle et 24 facettes pour représenter un objet 3D incurvé comme un cylindre. Pour les surfaces plus complexes comme un dôme, une valeur de 24 définit le nombre de facettes du périmètre et a également un impact sur la densité des facettes du reste de la forme.

Dans FormIt pour Windows v18 et versions ultérieures, les valeurs de création de facettes de courbe et de surface sont personnalisables :

![](../.gitbook/assets/faceting\_planter.gif)

![](<../.gitbook/assets/faceting (1).png>)

**Curve Faceting Quality**

La modification de la qualité de création de facettes de courbe a une incidence sur le nombre de facettes utilisées lors du dessin de nouveaux cercles et arcs dans FormIt, ainsi que lors du placement de formes primitives. Par exemple, si vous définissez cette option sur 64, vous créez un cercle complet de 64 côtés ou un arc d’un quart de cercle avec 16 facettes.

Cette valeur affecte également la qualité des cercles et des arcs importés à partir de fichiers SAT, ainsi que lors de l’ancrage de la géométrie à partir de Dynamo. Vous pouvez définir cette valeur pour les nouvelles esquisses ou uniquement pour l’esquisse actuelle.

Pour les courbes existantes, vous pouvez également utiliser le plug-in Rebuild Curve pour reconstruire rétroactivement un arc ou un cercle **existant** avec un nouveau nombre de facettes :

![](../.gitbook/assets/screen-shot-2020-01-10-at-1.20.53-pm.png)

![](../.gitbook/assets/faceting\_rebuild-curve.gif)

**Qualité de création de facettes de surface**

La modification de ce paramètre global affecte la qualité des surfaces incurvées 3D importées à partir de fichiers SAT et lorsqu’elles sont ancrées à partir de Dynamo.

Par exemple, si vous définissez cette option sur 64, l’ancrage d’une sphère à partir de Dynamo utilise 64 faces autour de l’équateur de la sphère, plus 64 facettes dans chacun des anneaux allant vers les pôles de la sphère, ce qui peut rapidement faire beaucoup. Utilisez des valeurs plus élevées avec précaution, car cela peut avoir une incidence sur les performances de FormIt dans certains cas. Une fois que vous obtenez un résultat de haute qualité, vous pouvez [le convertir en maillage](meshes.md) pour améliorer les performances.

Lorsque vous utilisez Dynamo, vous pouvez modifier la qualité de la création de facettes et cliquer sur « Exécuter le graphique » dans le groupe de fonctions Propriétés sans modifier les paramètres, afin d’utiliser d’autres nombres pour la création de facettes :

![](../.gitbook/assets/faceting\_column.gif)

Comme avec les courbes, vous pouvez définir la qualité de la création de facettes de surface pour les nouvelles esquisses ou pour l’esquisse actuelle uniquement.

Notez que les valeurs de la création de facettes sont actuellement limitées à des multiples de 4. Par conséquent, lorsque vous saisissez des nombres manuellement, FormIt arrondit au multiple le plus proche. Vous pouvez utiliser les curseurs et les flèches pour parcourir les valeurs acceptées.

![](../.gitbook/assets/units-+-precision.png)
