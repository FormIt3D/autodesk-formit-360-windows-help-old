# 1.4 - Añadir suelos con niveles

_Los niveles permiten segmentar masas con referencias de suelo individuales y calcular el área bruta por masa de edificio. Los niveles de FormIt y sus nombres personalizados se convertirán en niveles de Revit cuando el archivo se convierta a Revit._

_Si no ha completado la última sección, descargue y abra el archivo **1.4 - Add Floors with Levels.axm** de los **conjuntos de datos de la parte 1 de FormIt Primer**._

## **Crear y personalizar niveles**

1 - Para crear niveles, realice lo siguiente:

1. Vaya a la **paleta Nivel** en la **barra de paletas**.
2. Haga clic en **+** \(**Añadir nivel**\) cuatro veces para crear cuatro niveles.
3. Haga doble clic en la elevación actual de cada nivel para modificarla a **0'-0", 2'-2", 4'-6"** y **17'-8"**.
4. Haga doble clic en el nombre actual de cada nivel y cámbieles el nombre a **Suelo, Terraza, Edificio principal** y **Parte superior de la cubierta.**

![](../../.gitbook/assets/0%20%2816%29.png)

_**Nota** Puede hacer clic en el icono __**++**__ para crear varios niveles con una distancia especificada y uniforme. Esto es útil para edificios de varias plantas_.

## **Aplicar niveles a geometría**

_En los pasos anteriores, solo hemos creado niveles. Ahora ya podemos aplicar esos niveles a la geometría que hemos creado._

1 - Para aplicar niveles a la geometría existente, realice lo siguiente:

1. Haga doble clic en la masa de terraza superior completa para seleccionarla.
2. En la **paleta Propiedades**, haga clic en **Utilizar niveles**. Este paso preseleccionará todos los niveles que se intersequen actualmente con la geometría seleccionada.
3. Ahora se le han aplicado tres niveles a la geometría seleccionada **(Edificio principal, Terraza** y **Suelo**\), pero en este ejercicio solo deseamos aplicar **Suelo**. Desactive **Edificio principal** y **Terraza**.
4. Este proceso garantiza que solo se tenga en cuenta el área intersecada por **Suelo** para el cálculo del área bruta, que se puede ver en el campo **Área por nivel**.

![](../../.gitbook/assets/1%20%284%29.png)

_**Nota** Si no aparecen líneas de nivel de color azul en la masa, escriba_ _**DL**_ _para activar la opción_ _**Mostrar niveles**._

![](../../.gitbook/assets/2%20%283%29.png)

