# 1.8 - Crear pilares con matriz

_En este ejercicio, vamos a crear un boceto de un elemento detallado: un pilar de viga en I. A continuación, utilizaremos la herramienta Matriz para crear rápidamente varias copias espaciadas uniformemente._

_Si no ha completado la última sección, descargue y abra el archivo_ _**1.8 – Create Columns with Array.axm**_ _de los_ _**conjuntos de datos de la parte 1 de FormIt Primer**._

## **Crear el boceto del perfil de pilar**

1 - Para facilitar el proceso de dibujo, realice lo siguiente:

1. Vaya a la **Vista superior \(VT\)**.
2. Cambie el modo de vista a **Ortogonal \(VO\)**.
3. Desactive las capas **Main Building**, **Floor** y **Roof**. Este paso impedirá que la nueva geometría se ajuste a la geometría existente en esas capas.
4. Amplíe la esquina superior izquierda de la imagen de **plano de planta importado** para poder ver el pilar en detalle.
5. Desactive la función **Forzar cursor a rejilla \(SG\)** \(si la ha activado\). Esto ayudará a dibujar las líneas de detalle.

![](../../.gitbook/assets/0%20%2813%29.png)

_Para dibujar el pilar, dibujaremos primero la mitad y, a continuación, lo reflejaremos para crear rápidamente la otra mitad simétrica._

2 - Para crear la primera mitad de la viga en I, utilice la **herramienta Línea \(L\)** para crear el siguiente boceto con las cotas especificadas. No se preocupe por la posición exacta del pilar en la imagen de plano.

![](../../.gitbook/assets/1%20%2818%29.png)

3 - Para reflejar la forma que acaba de dibujar, realice lo siguiente:

1. Haga doble clic para seleccionar todas las caras y los bordes de la geometría dibujada.
2. Haga clic con el botón derecho y seleccione la **herramienta Reflejar \(MI\)**.
3. Haga clic en el pinzamiento naranja central del **widget Reflejar** y colóquelo en la esquina inferior izquierda de la geometría.
4. Utilice la flecha inferior del botón de flecha de doble cara del widget para rotar el eje de simetría -90 grados \(sentido horario\).
5. Haga clic una vez en el espacio o pulse **Esc** para finalizar el proceso de reflejo. El resultado debe tener un aspecto similar al de un perfil de viga en I con una línea que desciende por el medio. Pulse **Esc** de nuevo para anular la selección.

![](../../.gitbook/assets/2%20%285%29.png)

![](../../.gitbook/assets/3%20%287%29.png)

_**Nota**: La orientación y la ubicación de la geometría final se previsualizan con la forma azul fantasma mientras se ajusta el widget Reflejar. Puede utilizar esta vista preliminar como referencia para reflejar la geometría en la ubicación deseada._

4 - Para unir ambos lados en una sola geometría, elimine la línea que los divide. Para ello, haga clic en ella para seleccionarla y, a continuación, pulse **Suprimir**. Ahora las dos superficies se unen en una sola.

5 - Para mover la geometría a su ubicación final, realice lo siguiente:

1. Si está desactivada, active las capas **Plan Image** y **Roof** para utilizarlas como guía.
2. Haga doble clic en el perfil de pilar para seleccionar su cara y todas sus líneas. Empiece a mover la selección a lo largo del eje verde \(**Eje Y**\). Mantenga pulsada la tecla **Mayús** y mueva el perfil hasta que se alinee con la cubierta y, a continuación, haga clic para colocarlo.
3. De forma similar al paso anterior, vuelva a mover la geometría; esta vez, bloquéela en el eje rojo \(**Eje X**\).
4. Haga clic para colocarla encima de la viga en I dibujada en **Plan Image**. Acercarse es suficiente, como en la siguiente imagen, la posición horizontal no tiene que ser perfecta.

_**Nota:**_ _La tecla_ _**Mayús**_ _bloqueará la geometría para moverla solo a lo largo de un eje, en este caso, el verde \(**Eje Y**\). De este modo, se garantiza que el perfil del pilar no se mueva hacia arriba y se alinee accidentalmente con la parte superior del plano de cubierta._

![](../../.gitbook/assets/4%20%289%29.png)

## **Extrusión y matriz del pilar**

1 - Para facilitar el siguiente proceso de dibujo, vuelva a cambiar el modo de vista a **Perspectiva \(VP\)** y utilice **Orbitar \(O\)** para colocar la cámara como si se visualizase el perfil de la viga en I desde el noroeste. Utilice la flecha norte situada en la esquina inferior izquierda para facilitar la colocación de la vista.

![](../../.gitbook/assets/5%20%281%29.jpeg)

_**Nota:**_ _Para obtener información sobre cómo desplazarse por el boceto, se recomienda que consulte el capítulo sobre_ _**desplazamiento por la escena**_ _._

2- Seleccione la cara del perfil del pilar y extruya la cara hasta**17'-8"**.

_**Nota:**_ _Si el perfil del pilar se alinea con la cubierta al moverlo, extruya la cara hacia abajo_ _**17'-8"**   en lugar de hacia arriba._

3 - Reduzca la vista y active la capa **Roof** \(si está desactivada\). La parte superior del pilar debe alinearse con la parte superior de la cubierta.

![](../../.gitbook/assets/6%20%289%29.png)

4 - Para mantener el modelo organizado y ordenado, seleccione de nuevo la geometría del pilar y realice lo siguiente:

1. Utilice la herramienta **Grupo \(G\)** y asígnele el nombre **Column Tall**.
2. Cree una nueva **capa** denominada **Column** y añádala al grupo.
3. Importe el material **Metal - Brushed - Colorized** y pinte el grupo con él.

![](../../.gitbook/assets/7%20%284%29.png)

_**Nota:**_ _Consulte los capítulos anteriores para obtener más información sobre los_ _**grupos**, las_ _**capas** y los_ _**materiales**._

4 - Haga clic en **Esc** para desactivar la herramienta de pincel.

## **Organizar en matriz los pilares**

1 - Vaya a la **Vista superior \(VT\)** y cambie de nuevo el modo de cámara a **Ortogonal \(VO\)**.

2 - Desactive la capa **Roof**.

3 - Para iniciar el proceso de agrupación en matriz, realice lo siguiente:

1. Haga clic una vez para seleccionar el grupo de pilares. Haga clic con el botón derecho para abrir el **menú contextual** y seleccione **Matriz \(AR\)**.
2. En el cuadro de diálogo **Propiedades de matriz**, utilice los siguientes parámetros:
   * **Longitud entre copias**
   * **Lineal** \(por defecto\)
   * **Agrupar cada sólido e incluir en matriz** \(por defecto\)
   * **Número de copias: 3**
   * Pulse **Aceptar** para cerrar el cuadro de diálogo.

![](../../.gitbook/assets/8%20%283%29.png)

4 - Para colocar los nuevos elementos, realice lo siguiente:

1. Haga clic una vez en el pilar para iniciar la herramienta **Matriz**. Mueva el cursor a lo largo del eje rojo \(**Eje X**\).
2. Defina la cota en **22'**. Ahora tiene **cuatro** pilares con una separación de **22'**.
3. Pulse **Esc** para borrar la selección.

![](../../.gitbook/assets/9%20%286%29.png)

5 - Para seleccionar todos los grupos de **Tall Column** a la vez, coloque el cursor sobre uno de ellos y pulse la tecla **Tab** una vez. Observe que se han resaltado los cuadros delimitadores de los cuatro pilares. Haga clic una vez en el pilar sobre el que ha colocado el cursor del ratón; se seleccionarán todos. Esta es una forma rápida de seleccionar todos los ejemplares del mismo grupo a la vez.

6 - Utilice de nuevo la herramienta **Matriz \(AR\)** para crear los pilares en el otro lado del edificio. Esta vez, realice una copia a lo largo del eje verde a través del edificio. Establezca la cota en **29'- 4 5/8".**

_**Nota:**_ _29' 4 5/8" = 8 5/8" \(profundidad del pilar\) + 28'-8" \(anchura del edificio principal\)._

7 - Para visualizar todo el edificio, vaya a la **Vista 3D \(V3\)** y establézcalo en **Perspectiva \(VP\)**. Si están desactivadas, active las capas **Main Building Floor**, **Roof**, **Lower Terrace** y **Column**.

![](../../.gitbook/assets/10%20%287%29.png)

## **Crear los pilares de la terraza**

_Ahora duplicaremos los pilares del edificio principal para crear versiones similares, pero más cortas, para la terraza._

1 - Para facilitar el dibujo, es recomendable volver a los parámetros **Ortogonal \(OV\)** y **Vista superior \(VT\)**.

2 - Para crear los nuevos pilares, realice lo siguiente:

1. Mantenga pulsada la tecla **Ctrl** o **Mayús** y haga clic en los tres pilares más próximos al **suelo de la terraza interior** para seleccionarlos.
2. Haga clic una vez en cualquiera de los pilares para empezar a mover los tres pilares seleccionados a la vez. Pulse la tecla **Ctrl** una vez para crear una **copia rápida**. Aparecerá una vista preliminar fantasma de la copia.
3. Mueva las copias hacia abajo a lo largo del eje verde \(**Eje Y**\) **23'-4 3/8"**. Pulse **Esc**.
4. Sin anular la selección, mueva los pilares copiados a lo largo del eje rojo \(**Eje X**\) **22'** para colocarlos en su posición final.
5. Con los tres nuevos pilares seleccionados, haga clic otra vez con el botón derecho en uno de los pilares copiados y seleccione **Establecer como exclusivo \(MU\)**. Estos pilares están ahora asociados entre sí, pero son exclusivos frente a los originales.

_**Nota:**_ _Si se mantiene pulsada la tecla_ _**Mayús**_ _o_ _**Ctrl**_ _, es posible seleccionar varios elementos a la vez o eliminar elementos de la selección actual._

![](../../.gitbook/assets/11%20%287%29.png)

3 - Modifique el nuevo grupo de pilares. Para ello, realice lo siguiente:

1. Haga doble clic para editar uno de los nuevos grupos y cambie su nombre a **Column Short.**
2. Ajuste la altura del nuevo pilar para alinearlo con la parte superior de la **suelo de terraza** **inferior** \(3'-2"\). Para ello, seleccione y arrastre la cara del pilar hacia abajo a lo largo del eje azul \(**Eje Z**\) y mantenga pulsada la tecla **Mayús**. Coloque el cursor sobre cualquier lugar de la cara superior del **suelo de terraza inferior** y la altura del pilar se alineará automáticamente con la terraza inferior. Una vez que se haya definido la altura, haga clic para finalizar.

![](../../.gitbook/assets/12%20%284%29.png)

_**Nota:**_ _Puede comprobar la altura de los pilares cortos mediante la herramienta_ _**Medir \(ME\)**_ _. También puede seleccionar uno de los bordes verticales del pilar y ver su longitud en la_ _**paleta Propiedades**._

4- Mediante las técnicas que acaba de aprender, copie el pilar corto más lejano al lado opuesto del **suelo de terraza inferior** para crear el último pilar restante.

![](../../.gitbook/assets/13%20%284%29.png)

