# Railing Along Path

## Con tecnología de Dynamo

En FormIt 2021 y versiones posteriores, puede generar una barandilla a lo largo de un camino y personalizar rápidamente los resultados in situ. La herramienta "Railing Along Path" cuenta con tecnología de Dynamo, lo que significa que la barandilla resultante se puede configurar fácilmente para obtener los resultados deseados y si se vuelve a ejecutar la lógica, se actualizará la geometría in situ.

![](../.gitbook/assets/railing-along-path.gif)

## Inicio de "Railing Along Path"

* Vaya al panel Dynamo en FormIt para Windows y asegúrese de que se encuentra en el directorio de muestras de Dynamo.
* Haga clic en la muestra "Railing Along Path".
* En el lado izquierdo de la pantalla, aparecerá una solicitud para seleccionar un camino para la barandilla.
   * Aquí, debe seleccionar solo una serie de bordes contiguos o un grupo que contenga solo una serie de bordes.
   * Una vez que haya seleccionado el camino, haga clic en el botón "finish" o pulse Intro.
* El panel de Dynamo indicará que está procesando los cambios. Cuando haya terminado, tendrá una barandilla generada por Dynamo en un grupo de FormIt, lista para modificar \(consulte la información mostrada a continuación\).

## Iteración in situ

Después de ejecutar "Railing Along Path", observará que sus resultados se han establecido en los valores por defecto. Es posible que le parezcan satisfactorios estos valores, pero también puede personalizar la barandilla para adaptarla a sus necesidades.

Cuando se ejecuta, esta función crea un nuevo grupo que contiene los resultados y FormIt selecciona automáticamente el grupo y las opciones disponibles para ese ejemplar de "Railing Along Path".

Siempre puede volver a las propiedades de "Railing Along Path". Para ello, seleccione el grupo y cambie al panel Propiedades o modifique el grupo que mostrará automáticamente las propiedades.

![](../.gitbook/assets/railing-along-path-options.png)

### Altura de barandilla

La altura total de la barandilla. Utiliza las unidades actuales de FormIt.

### Post Spacing

La distancia entre las pilastras verticales principales. Utiliza las unidades actuales de FormIt.

### Add Posts at Path Vertices

Si se establece en **True**, las pilastras se añadirán en cada vértice del camino seleccionado y el cálculo de la siguiente posición de la pilastra se restablecerá en ese punto.

Por ejemplo, si ha seleccionado una serie de tres bordes, aparecerá una pilastra en cada uno de los dos puntos interiores. Esto resulta útil si los vértices indican un cambio de dirección \(como subir escaleras o girar esquinas\) en el que se colocará de forma natural una pilastra.

Si se establece en **False**, las pilastras solo se añadirán a lo largo del camino empezando desde un extremo y midiendo la distancia a lo largo del camino, omitiendo los vértices a lo largo de la trayectoria. Esto resulta útil si ha seleccionado un arco, una spline o un círculo, donde los vértices no son importantes y desea que la distancia entre pilastras los omita.

### Reverse Path Direction

Al calcular la posición de las pilastras, la dirección del camino seleccionado determinará el extremo del camino en el que se iniciará la medición de la distancia entre pilastras.

En los casos en que la distancia entre pilastras dé como resultado el espacio restante en un extremo no deseado del camino, puede cambiar este valor a **True** para voltear la curva e iniciar la medición de la separación entre pilastras en el extremo opuesto.

### Post Width + Post Depth

El tamaño \(en plano\) de los perfiles de pilastra vertical rectangular. Utiliza las unidades actuales de FormIt.

### Handrail Width + Handrail Height

El tamaño \(en sección\) del perfil de pasamanos rectangular. Utiliza las unidades actuales de FormIt.

### Baluster Orientation

Si se establece en "True", los balaustres se orientarán horizontalmente, como los cables. Si se establece en "False", los balaustres se orientarán verticalmente para obtener una estética más tradicional.

### Baluster Width + Baluster Depth

El tamaño del perfil rectangular del balaustre. Utiliza las unidades actuales de FormIt.

### Baluster Spacing

La cantidad de espacio entre cada balaustre. Utiliza las unidades actuales de FormIt.

### Bottom Rail Start Height

La distancia entre la parte inferior de la barandilla y el barandal inferior que soporta los balaustres. Utiliza las unidades actuales de FormIt.

### Ejecutar

Después de editar las opciones, haga clic en el botón Ejecutar para ejecutar el gráfico subyacente de Dynamo y generar nuevos resultados. Este botón se colorea de azul cuando se han modificado los parámetros, por lo que debe hacer clic en él para ver las actualizaciones en la geometría final.‌

### Editar gráfico incrustado

Al hacer clic en este botón, se inicia el entorno del editor de gráficos de Dynamo, por lo que puede ver y editar el gráfico subyacente de Dynamo para cambiar los parámetros y ver las actualizaciones directas con mayor rapidez o para inspeccionar o ajustar la lógica.

