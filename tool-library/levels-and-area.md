# Niveles y área

Después de crear la geometría en FormIt, puede aplicar Niveles para indicar dónde están las elevaciones de suelo y generar cálculos de área.

Consulte [FormIt Primer](../formit-primer/part-i/adding-floors-with-levels.md) para ver los niveles en acción.

## Creación y configuración de niveles

Encontrará el panel Niveles en el lado derecho de FormIt para Windows, como se muestra a continuación:

![](../.gitbook/assets/20191217-levels-panel-1.png)

#### Crear y suprimir niveles

* Para crear un nivel, haga clic en el botón "+".
* Para crear un serie de niveles, haga clic en el botón "++".
   * Esto permitirá especificar los niveles que se van a crear y la distancia vertical entre ellos.
* Seleccione uno o más niveles y haga clic en "-" para suprimirlos.

#### Cambiar nombre, establecer elevaciones y volver a numerar niveles

* Cambie el nombre de un nivel. Para ello, haga doble clic en el nombre o haga clic con el botón derecho y seleccione Editar nombre.
* Ajuste la elevación de un nivel. Para ello, haga doble clic en el número o haga clic con el botón derecho y seleccione Editar elevación.
* Haga clic en el icono Actualizar en la parte superior para cambiar la numeración de los niveles.
   * Esto resulta útil si ha añadido o eliminado niveles y el esquema de nombres por defecto no está sincronizado \(por ejemplo, Nivel 1, Nivel 2, Nivel 5\).
   * Este botón omitirá los niveles con nombres personalizados, pero volverá a numerar los niveles con el nombre que se encuentre después de la sintaxis "Nivel 1".

## Aplicación de niveles

Para aplicar niveles a un objeto, deberá seleccionar el objeto y pasar al panel Propiedades.

Tenga en cuenta que, para aplicar niveles a un objeto, este debe ser sólido, sin problemas de caras posteriores o hermeticidad. [Obtenga información sobre cómo comprobar si el modelo presenta problemas de hermeticidad y caras posteriores](https://formit.autodesk.com/blog/post/repairing-solid-models).

Con un objeto sólido seleccionado en el lienzo \(en este ejemplo, un vaciado de edificio simple\), el grupo Propiedades presentará la casilla de verificación Utilizar niveles.

* Si el boceto de FormIt ya tiene niveles definidos \(como se muestra arriba\), al activar esta casilla, se utilizarán todos los niveles que se intersequen con esta forma \(y se omitirán los que sean demasiado altos o bajos\).
* Si el boceto de FormIt no tiene niveles, al activar esta casilla, se crearán suficientes niveles por defecto\(altura de suelo a suelo de 12'\) para intersecar toda la forma y se aplicarán automáticamente esos niveles a este objeto.

![](../.gitbook/assets/20191217-properties-panel.png)

## Niveles + Revit

Si se aplican niveles a la geometría de FormIt, esos niveles se enviarán a Revit cuando se utilice el [complemento FormIt](https://formit.autodesk.com/page/formit-revit).

En Revit, puede utilizar los niveles de FormIt para crear suelos de masa, suelos por cara y planos de planta asociados a ellos.



