# 1.6 - Controlar la visibilidad con capas

_Al igual que AutoCAD y Photoshop, las capas de FormIt permiten administrar la visibilidad de los objetos del modelo. En este capítulo, vamos a crear una capa para guardar y ocultar la masa de construcción para su posterior análisis._

_Si no ha completado la última sección, descargue y abra el archivo_ _**1.6 - Control Visibility with Layers.axm**_ _de los_ _**conjuntos de datos de la parte 1 de FormIt Primer**._

## **Crear capas**

1 - Para crear nuevas capas, realice lo siguiente:

1. Vaya a la **paleta Capas** y haga clic en el signo **+** tres veces para crear tres capas.
2. Haga doble clic en los nombres de capa para cambiarles el nombre a **Masa**, **Suelo del edificio principal** e **Imagen de plano.**

![](../../.gitbook/assets/0%20%2820%29.png)

_**Nota**_ _Puede hacer clic en un nombre de capa y arrastrarlo hacia arriba o hacia abajo para reordenar las capas._

2 - Para asignar el grupo **Masa - Edificio principal** a la capa **Masa**, realice lo siguiente:

1. En el lienzo, seleccione el grupo **Masa - Edificio principal**.
2. En la **paleta Capas**, seleccione la capa **Masa** en el menú desplegable **Selección en:**. Del mismo modo, asigne el grupo **Imagen de plano** a la capa **Imagen de plano**.

![](../../.gitbook/assets/1%20%2813%29.png)

## **Duplicar grupo**

_Ahora comenzaremos el proceso de modelado del edificio con más detalle. El primer paso consiste en crear la geometría del suelo en función de la masa de construcción que ya tenemos._

1 - Seleccione de nuevo el grupo **Masa - Edificio principal**. Pulse **Ctrl + C \(Copiar\)** para copiar y, a continuación, **Ctrl + Mayús + V \(Pegar in situ\)** para pegar la masa en el mismo lugar.

2 - Para disociar la nueva geometría del grupo original, haga clic con el botón derecho para acceder al **Menú contextual** y seleccione la opción **Establecer como exclusivo \(MU\)**.

![](../../.gitbook/assets/2%20%2818%29.png)

_**Nota** El nuevo grupo ya no está asociado con el original. Los cambios realizados en el nuevo grupo no modificarán el grupo original._

## **Crear la geometría de suelo**

1 - Vuelva a asignar la capa del grupo como se indica a continuación:

1. Haga clic una vez para seleccionar uno de los grupos de **Masa - Edificio principal**.
2. Coloque el grupo en la capa **Suelo del edificio principal** mediante el menú desplegable **Selección en:** de la **paleta Capas**.
3. Desactive la capa **Masa** para ocultar su geometría y mantenerla a salvo de cualquier modificación accidental.

![](../../.gitbook/assets/3%20%2818%29.png)

2 - Haga doble clic en el grupo visible **Masa - Edificio principal** para editarlo. Cambie el nombre del grupo a **Suelo** en la **paleta Propiedades**.

![](../../.gitbook/assets/4%20%2812%29.png)

3 - **Haga clic una vez** en la **cara superior** de la geometría para seleccionarla. Haga clic de nuevo y comience a arrastrar la cara hacia abajo. Cuando arrastre la cara hacia abajo, introduzca **11'-2"**; aparecerá el **cuadro de diálogo Cota**. Haga clic en **Aceptar** después de introducir el valor. El suelo resultante debe tener un grosor de 1'. Haga doble clic en el espacio para salir del grupo.

![](../../.gitbook/assets/5%20%2810%29.png)

