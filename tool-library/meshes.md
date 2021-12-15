# Mallas

A partir de la versión v17.0, FormIt ofrece un nuevo tipo de geometría, las mallas.

Las mallas son representaciones ligeras de objetos FormIt estándar y son excelentes para mejorar el rendimiento de la geometría de polígonos altos, por ejemplo, el mobiliario o un entorno 3D, como personas, árboles, coches y señales. Las mallas también son excelentes para la geometría DWG compleja que, de lo contrario, podría afectar al rendimiento de FormIt.

Los objetos se pueden convertir en mallas y las mallas se pueden volver a convertir en objetos sin perder ningún dato. Algunos tipos de archivo se importan automáticamente como mallas, por ejemplo, OBJ, STL y DWG. A continuación, obtenga más información sobre la conversión entre tipos y otras ventajas y limitaciones de las mallas.

### Conversión de objetos en mallas

Cualquier combinación de vértices, bordes, caras o cuerpos sólidos se puede convertir en mallas.

Solo tiene que seleccionar Objetos y utilizar el método abreviado OM \(De objetos a mallas\) o hacer clic con el botón derecho y seleccionar De objetos a mallas en el menú contextual, como se muestra a continuación:

![](../.gitbook/assets/context-menu_object-to-mesh.PNG)

Una vez que los objetos se hayan convertido en mallas, aparecerá un mensaje de confirmación en la parte superior de la pantalla, como se muestra a continuación:

![](../.gitbook/assets/success_object-to-mesh.PNG)

**Tenga en cuenta lo siguientes al convertir objetos en mallas:**

* Los bordes suavizados de los objetos permanecerán suavizados en las mallas resultantes.
* Las orientaciones de los materiales de los objetos permanecerán sin cambios en las mallas resultantes.
* Se crea una malla para cada material aplicado. Por ejemplo, si convierte un cubo pintado con seis colores diferentes, obtendrá seis mallas diferentes.
   * Al convertir de nuevo en un objeto, se volverán a sellar las mallas individuales en un cuerpo sólido.
* Al seleccionar un cuerpo sólido, se convertirá y se reemplazará todo el cuerpo por una malla, pero, al seleccionar bordes o vértices individuales que pertenecen a un sólido, se creará una nueva malla encima de la geometría existente, sin que esto afecte al cuerpo original.
* La conversión de un conjunto de bordes o vértices creará una única malla de línea \(una malla compuesta de bordes\) o una única malla de puntos \(una malla compuesta de puntos\), por lo que no podrá seleccionar bordes o vértices individuales una vez que se hayan combinado en una única malla. Convierta estos elementos de nuevo en objetos si desea ajustar la posición de un único elemento.

**Conversión de geometría agrupada en mallas:**

* Las mallas se vuelven aún más eficaces cuando se puede convertir un grupo completo y todos sus grupos anidados en mallas.
* Los grupos y su contenido anidado se pueden convertir en grupos mediante un módulo de extensión:
   * Busque el icono de Plugin Manager en el lado derecho de la aplicación, como se muestra a continuación:
      * ![](../.gitbook/assets/plugin-manager_icon.PNG)
   * Busque el módulo de extensión Mesh + Unmesh All y haga clic en la casilla de verificación para instalarlo, como se muestra a continuación:
      * ![](../.gitbook/assets/plugin-manager_mesh-unmesh-all.PNG)
   * Se cargará el módulo de extensión Mesh + Unmesh All. Solo tiene que seleccionar un grupo que contenga objetos que desee convertir en mallas y hacer clic en Mesh All.
      * ![](../.gitbook/assets/mesh-unmesh-all-plugin.PNG)
   * Al convertir mallas u objetos anidados con este módulo de extensión, aparecerá un mensaje de actualización en la parte superior de la pantalla que indica cuántos grupos y ejemplares de grupos se han visto afectados por la operación:

![](../.gitbook/assets/success_mesh-all.PNG)

### Interacción con mallas

**Debido a su naturaleza ligera, las mallas presentan determinadas limitaciones y comportamientos:**

* No podrá editar las caras, bordes o vértices individuales de una malla.
   * Sin embargo, puede volver a pintar mallas y desplazar mallas individuales creadas como resultado de distintos materiales aplicados a las caras \(consulte la información mostrada anteriormente\).
* El forzado de cursor a mallas está limitado a las caras y los vértices de las mallas. Para mejorar el rendimiento, el forzado de cursos y las deducciones no funcionarán con los bordes de mallas.
   * Sin embargo, los archivos DWG convertidos en mallas \(un tipo de malla diferente conocido como malla de línea\) conservarán la capacidad de forzar el cursor a los bordes de malla y realizar deducciones sobre ellos.
* No se pueden aplicar niveles a las mallas.
* Las mallas no notificarán problemas de hermeticidad o caras posteriores. Convierta estos elementos de nuevo en objetos para ver si son herméticos o no.
   * Los objetos herméticos antes de la conversión a una malla permanecerán herméticos cuando se vuelvan a convertir en un objeto.
* Las mallas no se pueden utilizar en operaciones avanzadas de modelado, como Unir/Cortar sólido, Vaciado 3D, Desfase 3D, Empalme, Solevación, Barrido o Recubrimiento.

De lo contrario, las mallas se mostrarán y se comportarán como cualquier otro objeto de FormIt. Se pueden incluir en grupos, asignar a capas, visualizar en escenas, utilizar para el análisis, etc.

**Si la información de herramientas indica En la malla o si el panel Propiedades informa de una malla, sabrá que está interactuando con una malla, como se muestra a continuación:**

![](../.gitbook/assets/snap_on-mesh.PNG)

![](../.gitbook/assets/properties-panel_mesh.PNG)

**Algunos tipos de archivo se importan automáticamente como mallas para mejorar el rendimiento, como se indica a continuación:**

* Los archivos STL y OBJ, que pueden contener geometría densa como nubes de puntos de otras aplicaciones, se importan automáticamente como mallas.
* Los archivos DWG, que pueden contener millones de segmentos de borde pequeños en curvas de alta calidad, se importan automáticamente como mallas.

### Conversión de mallas en objetos

Solo tiene que seleccionar Mallas y utilizar el método abreviado MO \(De mallas a objetos\) o hacer clic con el botón derecho y seleccionar De mallas a objetos en el menú contextual:

![](../.gitbook/assets/context-menu_mesh-to-object.PNG)

Una vez que los objetos se hayan convertido en mallas, aparecerá un mensaje de confirmación en la parte superior de la pantalla, como se muestra a continuación:

![](../.gitbook/assets/success_mesh-to-object.PNG)

**Al convertir mallas en objetos, tenga en cuenta lo siguiente:**

* Los objetos que eran sólidos o herméticos antes de convertirlos en mallas se volverán a unir en un sólido hermético cuando se vuelvan a convertir en un objeto.
* Al convertir una serie de bordes \(por ejemplo, de un archivo DWG\) o de una serie de vértices \(por ejemplo, de una nube de puntos\) en una malla y a la inversa, se incluirán automáticamente los objetos sin malla en un grupo.
   * Esto impide que los nuevos bordes o vértices se fusionen con otra geometría, lo que podría tener efectos adversos y afectar al rendimiento.
   * Solo tiene que desagrupar el grupo resultante para liberar los bordes o los vértices.

**Conversión de mallas agrupadas en objetos:**

* Consulte las instrucciones anteriores para utilizar el módulo de extensión Mesh + Unmesh All para convertir los grupos y sus mallas anidadas en objetos.

