# Array Along Path

## Con tecnología de Dynamo

En FormIt 2021 y versiones posteriores, puede organizar los objetos a lo largo de un camino y personalizar rápidamente los resultados in situ. La opción "Array Along Path" cuenta con tecnología de Dynamo, lo que significa que la matriz se puede configurar fácilmente para obtener los resultados deseados y si se vuelve a ejecutar la lógica, se actualizará la geometría in situ.

![](../.gitbook/assets/array-along-path.gif)

## Inicio de "Array Along Path"

* Vaya al panel Dynamo en FormIt para Windows y asegúrese de que se encuentra en el directorio de muestras de Dynamo.
* Haga clic en la muestra de "Array Along Path".
* En el lado izquierdo de la pantalla, aparecerá la solicitud "Select object\(s\) to array".
   * Puede seleccionar cualquier combinación de objetos de FormIt para este paso.
   * Una vez que haya realizado una selección, puede pulsar la flecha "siguiente" situada a la izquierda de la pantalla o pulsar Intro.
* Ahora aparecerá la solicitud "Select path for array".
   * Aquí, debe seleccionar solo una serie de bordes contiguos o un grupo que contenga una serie de bordes contiguos.
   * Una vez que haya seleccionado el camino, haga clic en el botón "finish" o pulse Intro.
* El panel de Dynamo indicará que está procesando los cambios. Cuando haya terminado, tendrá una matriz generada por Dynamo en un grupo de FormIt, lista para modificar \(consulte la información mostrada a continuación\).

## Iteración in situ

Después de ejecutar "Array Along Path", verá que sus resultados se han establecido en valores por defecto, por lo que deseará modificarlos para que se adapten a sus necesidades.

Cuando se ejecuta, esta función crea un nuevo grupo que contiene los resultados y FormIt selecciona automáticamente el grupo y las opciones disponibles para ese ejemplar de "Array Along Path".

Siempre puede volver a las propiedades de "Array Along Path". Para ello, seleccione el grupo y cambie al panel Propiedades o modifique el grupo que mostrará automáticamente las propiedades.

![](../.gitbook/assets/array-along-path-options.png)

### Select Object\(s\) to Array <a id="run"></a>

Haga clic en este botón para volver al asistente de selección a fin de cambiar los objetos que se van a incluir en la matriz.

### Select Array Path

Haga clic en este botón para volver al asistente de selección y cambiar el camino que se utiliza para calcular la matriz.

### Array Type <a id="run"></a>

Esta opción activa o desactiva el tipo de matriz que se va a calcular: por distancia o por número.

**Si se establece en True**, el cálculo será por distancia, por lo que el número mostrado a continuación hará referencia a la distancia entre las copias.

**Si se establece en False**, el cálculo será por número de copias, por lo que el número mostrado a continuación hará referencia al número de copias que caben a lo largo del camino.

### Include Original Selection In Results

Si se establece en **True**, ocurre lo siguiente:

* Los objetos seleccionados se contarán como una de las copias nuevas.
* El grupo de Dynamo resultante incluirá la selección original en sus resultados, por lo que habrá un conflicto de planos entre las nuevas copias y la selección original. Puede colocar la selección original en una [capa](layers.md) y desactivarla para ocultarla.

Si se establece en **False**:

* La matriz resultante **no** incluirá la selección original, por lo que obtendrá el número de copias especificado,**además de** la selección original, por lo que no habrá ningún conflicto de planos.

### Rotate Copies Along Path

Si se establece en **True**, las copias se rotan para mantener la orientación del objeto original en relación con el camino.

Si se establece en **False**, las copias no se rotan, solo se desplazan.

### Utilizar posición relativa a lo largo del camino

Si se establece en **True**, ocurre lo siguiente:

* Cada copia mantendrá la distancia entre el camino y el objeto original.
* Si el objeto original **no** se coloca en uno de los puntos finales del camino, se utilizará el segmento restante más grande del camino para el cálculo de la matriz.

Si se establece en **False**:

* La longitud completa del camino se utilizará para calcular la matriz, independientemente de dónde esté el objeto original en relación con el camino.
* De este modo, se desenlaza la ubicación del camino en relación con el objeto y se utiliza simplemente todo el camino. Resulta útil si el camino y el objeto no están próximos entre sí.

### Reverse Path Direction

Solo para los caminos cerrados. Cuando se utiliza "Array Along Path" con un camino cerrado, la dirección de la curva puede invertir inesperadamente los resultados esperados de la matriz. Establezca esta opción en **True** para invertir la dirección de la matriz si se cambia la orientación de los resultados.

### Ejecutar <a id="run"></a>

Después de editar las opciones, haga clic en el botón Ejecutar para ejecutar el gráfico subyacente de Dynamo y generar nuevos resultados. Este botón se colorea de azul cuando se han modificado los parámetros, por lo que debe hacer clic en él para ver las actualizaciones en la geometría final.‌

### Editar gráfico incrustado <a id="edit-embedded-graph"></a>

Al hacer clic en este botón, se inicia el entorno del editor de gráficos de Dynamo, por lo que puede ver y editar el gráfico subyacente de Dynamo para cambiar los parámetros y ver las actualizaciones directas con mayor rapidez o para inspeccionar o ajustar la lógica.



## Selección de geometría

Al seleccionar objetos para "Array Along Path" y otros gráficos de Dynamo basados en selección, tenga en cuenta lo siguiente:

* Puede seleccionar cualquier combinación de objetos de FormIt: vértices, bordes, caras, sólidos, grupos y mallas.
   * Tenga en cuenta que, en función del paso, algunos de estos objetos no se deben seleccionar.
   * Por ejemplo, al seleccionar el camino, solo debe seleccionar una serie de bordes contiguos o un grupo que contenga una serie de bordes contiguos. Cualquier otra acción provocará errores en el gráfico.
* Puede hacer doble clic en un objeto para seleccionar todo lo que está enlazado.
* Puede utilizar la ventana de selección de área para capturar una serie de objetos.
* Puede seleccionar objetos seleccionados para anular su selección.
* Se necesita al menos un objeto para continuar con un paso basado en selección.



