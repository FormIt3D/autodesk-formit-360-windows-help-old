# Grupos

Una de las técnicas más básicas, aunque importantes, en los flujos de trabajo de FormIt es la agrupación. Los grupos permiten evitar que se una la geometría y permiten establecer relaciones de elemento principal/secundario entre los elementos copiados, por lo que si actualiza un elemento, se actualizarán ambos. Obtenga más información sobre los grupos [aquí](../formit-primer/part-i/grouping-objects.md).

Los grupos se pueden crear y editar de dos formas: desde el menú contextual de un grupo seleccionado o desde la barra de herramientas principal.

## Interacciones de grupos

Para **crear un grupo**, seleccione los elementos que desea agrupar (puede incluir bordes, caras, sólidos u otros grupos) y haga clic con el botón derecho. Seleccione la herramienta **Grupo \(G\)** en el menú contextual. Las imágenes importadas y las imágenes de satélite no se pueden agrupar.

Para **seleccionar un grupo**, haga clic en el grupo una vez. Observe las líneas discontinuas que aparecen al seleccionar un grupo; estas líneas indican el tamaño total del grupo.

Para **editar un grupo**, haga doble clic en el grupo. Se inicia un modo de edición en el que solo se pueden ver elementos fuera del grupo actual y forzar el cursor a ellos, pero no seleccionarlos. También puede ocultar los elementos fuera del grupo actual mediante el método abreviado de teclado **H**.

Puede crear **grupos dentro de grupos**; estos se denominan **grupos anidados** y se pueden crear en el modo de edición de grupo. Para subir un nivel en los grupos anidados, haga clic en cualquier lugar fuera de los grupos.

Para **salir del modo de edición de grupo**, haga doble clic en cualquier lugar fuera del grupo.

Puede **copiar un grupo** para crear una relación entre el grupo original y su copia: si modifica un grupo copiado, los mismos cambios afectarán a todos los grupos relacionados.

Para **interrumpir la relación entre grupos copiados**, seleccione el grupo o los grupos que desea separar, haga clic con el botón derecho y seleccione **Establecer como exclusivo** en el menú contextual. También puede seleccionar Establecer como exclusivo en la barra de herramientas Grupos.

Para **seleccionar todos los grupos relacionados**, coloque el cursor sobre un grupo y pulse la tecla Tab. Cuando todos los grupos relacionados se resalten, haga clic en los grupos para seleccionarlos. A continuación, puede realizar una acción en todos los grupos a la vez.

La opción [**Árbol de grupos**](groups-tree.md) ofrece una única ubicación para ver y administrar todos los grupos de un proyecto.

## Acceso al menú contextual y a la barra de herramientas Grupos

## ![](../.gitbook/assets/grouptoolbar.png)

**Agrupar elementos**

Para crear un grupo desde la barra de herramientas Grupos, seleccione uno o más elementos, haga clic en el icono **Crear grupo** y seleccione el icono **Finalizar**. También puede seleccionar **Crear grupo** en la barra de herramientas Grupos y, a continuación, seleccionar los elementos que desea agrupar y elegir el icono **Finalizar**.

Para **editar un grupo desde la barra de herramientas Grupos**, seleccione el icono **Editar grupo** y, a continuación, haga clic en el grupo que desee modificar. Cuando haya terminado de realizar modificaciones, seleccione el icono **Finalizar**. Esta herramienta permite elegir el grupo específico que desea editar, incluso aunque esté muy anidado.

**Para establecer un grupo como exclusivo desde la barra de herramientas, **seleccione el icono **Establecer como exclusivo** en la barra de herramientas Grupos. Además, puede seleccionar **Establecer como exclusivo** en la barra de herramientas Grupos, elegir el grupo que desea establecer como exclusivo y, a continuación, hacer clic en el icono **Finalizar**.

**Para desagrupar un grupo de la barra de herramientas Grupos, ** seleccione el grupo que desee modificar y elija el icono **Desagrupar** en el menú de la barra de herramientas Grupos. De este modo, se desagrupa la selección actual, pero no se desagrupa ningún grupo anidado. También puede seleccionar **Desagrupar** en la barra de herramientas, seleccionar el grupo que desee modificar y, a continuación, seleccionar el icono **Finalizar**.

**Para desagrupar todos los grupos anidados que se encuentran debajo del grupo seleccionado,** elija un grupo con grupos anidados y, a continuación, seleccione **Desagrupar todos los grupos anidados** en la barra de herramientas Grupos.

**Para desagrupar todos los grupos del modelo, **seleccione la herramienta **Desagrupar todo** de la barra de herramientas Grupos.

## Grupos y Revit

Si conoce las **familias** de Revit, el concepto de grupos en FormIt le resultará muy similar. Los grupos de FormIt tienen funciones que permiten transferirlos de forma inteligente a Revit.

**Categorías de grupos de FormIt**

Puede especificar las **categorías** de grupos en FormIt para que los grupos de FormIt se conviertan en familias de las mismas categorías al importarlos en Revit. Puede asignar categorías a los grupos de FormIt. Para ello, seleccione un grupo, acceda al modo de **edición de grupo** y utilice el panel **Propiedades** para elegir categorías. También puede asignar categorías en el panel **Árbol de grupos**.

**Nombres de grupo de FormIt**

También puede utilizar el panel **Propiedades** para especificar un nombre para el grupo de FormIt. Esto puede ser útil para navegar por su propio modelo y, al importar el modelo a Revit, puede filtrar fácilmente los elementos mediante el nombre del grupo.

Tenga en cuenta que **los grupos anidados en FormIt no se importan en Revit como grupos anidados**. Esto impide que se creen familias de Revit muy anidadas.

