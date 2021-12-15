# Texto 3D

## Con tecnología de Dynamo

En FormIt 2021 y versiones posteriores, puede generar y modificar objetos de texto 3D con tecnología de Dynamo. Dynamo permite editar la fuente, el tamaño y otras propiedades del texto in situ sin necesidad de volver a generar y colocar el texto cuando se necesiten realizar modificaciones.

![](../.gitbook/assets/3d-text.gif)

## Colocación de texto 3D

![](../.gitbook/assets/3d-text-placement.gif)

* Vaya al panel Dynamo en FormIt para Windows y asegúrese de que se encuentra en el directorio de muestras de Dynamo.
* Haga clic en el ejemplo de texto 3D.
* Desplace el cursor al lienzo; verá que el texto 3D aparece en el cursor.
   * Antes de colocarlo, puede situar el cursor sobre la geometría para orientar el texto 3D de forma diferente, por ejemplo, en una superficie vertical para que el texto se alinee verticalmente. También puede pulsar la tecla Tab para alternar entre las orientaciones.
* Haga clic para colocar el texto 3D, que se generará dentro de un grupo de FormIt.
* Después de colocarlo, aparecerá el panel Propiedades, en el que se muestran las opciones disponibles para el texto 3D.

## Iteración in situ

La ventaja de utilizar Dynamo para generar texto 3D es que editarlo es muy sencillo y mantiene el texto en su posición actual para una iteración rápida.

Las opciones de texto 3D están disponibles en el panel Propiedades cuando se selecciona el grupo de texto 3D o al modificarlo.

Después de colocar inicialmente el texto 3D, el panel Propiedades se mostrará automáticamente. También puede seleccionar el grupo y cambiar a Propiedades o hacer doble clic en el grupo para cambiar automáticamente al panel Propiedades.

![](../.gitbook/assets/3d-text-options.png)

### Texto

Escriba el texto que desea que se muestre en la geometría de texto 3D. En este campo, también se muestra una vista preliminar del tipo de letra y la justificación seleccionados. Pulse Intro/Retorno para usar varias líneas.

### Tipo de letra

Seleccione el tipo de letra del texto 3D. En esta lista, se mostrarán los tipos de letra disponibles en el equipo y, al seleccionar un nuevo tipo, se actualizará el campo de texto.

Tenga en cuenta que algunos tipos de letra presentan geometría más compleja y puede que tarde más en generarse con Dynamo.

### Justificación

Esta opción desplazará el texto que se va a alinear en relación con el origen del sistema de coordenadas local del grupo.

* La opción "Left" garantizará que el texto comience en el origen del grupo y se expanda hacia la derecha.
* La opción "Center" garantizará que el texto esté siempre centrado en torno al origen del grupo.
* La opción "Right" garantizará que el texto termine en el origen del grupo.

![](../.gitbook/assets/3d-text-justification-combined.png)

### Tamaño de texto

![](../.gitbook/assets/3d-text-text-size.png)

La altura del texto expresada en las unidades actuales de FormIt.

### Extrusion Depth

La cantidad de extrusión 3D del texto expresada en las unidades actuales de FormIt. El texto 3D se ha diseñado para que sea uniforme, por lo que este valor no puede ser cero, pero puede utilizar un valor próximo a 0 para que sea menos obvio que está extruido.

### Interletraje

![](../.gitbook/assets/3d-text-tracking.png)

El interletraje es útil para ajustar el espaciado por defecto entre letras de un tipo determinado. Utiliza las unidades de FormIt actuales y puede ser positivo o negativo. Por ejemplo, en pies, 0,25 añadirá 3" de espaciado entre cada letra. Por el contrario, -0,25 hará que todas las letras estén 3" más cerca.

### Multi-Line Spacing

![](../.gitbook/assets/3d-text-multi-line.png)

Si tiene varias líneas en el campo de texto, este valor controla el espacio que hay entre cada línea de texto. Utiliza las unidades actuales de FormIt.

### Invert Text

![](../.gitbook/assets/3d-text-inverted.png)

Si se establece en "True", esta opción crea un sólido alrededor del texto y elimina el texto de él, lo que da como resultado texto "invertido", como si el texto se hubiera cortado de un material.

### Inverted Text Border

![](../.gitbook/assets/3d-text-inverted-border.png)

Solo se aplica cuando la opción "Invert Text" se ha establecido como "True". Permite especificar la cantidad de borde alrededor del texto que se va a utilizar para el sólido del que se ha eliminado el texto. Utiliza las unidades actuales de FormIt.

### Calidad de facetado de curva

Las curvas de tipos de letra se convierten en segmentos de línea mediante texto 3D, por lo que este valor controla la precisión con la que se facetan las curvas.

Los números más bajos darán como resultado un facetado más grueso \(segmentos más largos\) y los números más altos darán como resultado un facetado más fino \(segmentos más cortos\). Este valor modifica los parámetros de facetado de curva y superficie de FormIt en Preferencias.

### Ejecutar

Después de editar las opciones, haga clic en el botón Ejecutar para ejecutar el gráfico subyacente de Dynamo y generar nuevos resultados. Este botón se colorea de azul cuando se han modificado los parámetros, por lo que debe hacer clic en Ejecutar para ver las actualizaciones en la geometría final.‌

### Editar gráfico incrustado

Al hacer clic en este botón, se inicia el entorno del editor de gráficos de Dynamo, por lo que puede ver y editar el gráfico subyacente de Dynamo para cambiar los parámetros y ver las actualizaciones directas de forma rápida o para inspeccionar o ajustar la lógica. Esto no es necesario, pero puede ser útil para solucionar problemas o agilizar la edición. Consulte a continuación para obtener más información.

## Iteración más rápida en Dynamo

Si está realizando iteraciones en las opciones de texto 3D, puede que sea más rápido iniciar el editor de gráficos de Dynamo, que le permitirá ajustar los parámetros y ver los cambios en tiempo real. Esto también permite inspeccionar la lógica tras el gráfico, en caso de que haya problemas.

![](../.gitbook/assets/3d-text-edit-embedded.png)

Puede hacer clic en el botón Editar gráfico incrustado en el panel Propiedades para iniciar el editor de gráficos de Dynamo.

![](../.gitbook/assets/3d-text-edit-embedded-windows.png)

## Solución de problemas

La función de texto 3D utiliza Dynamo entre bastidores y Dynamo usa un núcleo de modelado denominado ASM para generar su geometría, que se transfiere de nuevo a FormIt.

Algunos tipos de letra pueden crear "curvas intersecantes" u otra geometría problemática, lo que puede provocar errores en ASM.

Si se produce un error al intentar ejecutar la función de texto 3D o si desaparecen las letras, es recomendable hacer clic en Editar gráfico incrustado para ver qué sucede con el gráfico y dónde puede estar el error.

Algunos tipos de letra también presentan problemas conocidos que impiden que se conviertan en geometría adecuada. Bahnschrift es un ejemplo de esto. Si encuentra otro tipo de letra que sea problemático, [infórmenos de ello en los foros](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=es). Haremos todo lo posible para solucionar problemas con tipos de letra específicos.





