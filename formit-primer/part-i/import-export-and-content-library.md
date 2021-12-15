# 1.11 - Importar modelos con la biblioteca de contenido

_En este capítulo, importaremos modelos de SketchUp existentes y utilizaremos la biblioteca de contenido de FormIt para insertar familias OOTB que se han convertido desde Revit. Tenga en cuenta que al abrir archivos SKP con FormIt, estos se suministran con materiales, grupos y componentes, capas \(etiquetas\) y escenas intactos. Puede que sea necesario realizar alguna limpieza para mantener los proyectos ordenados y organizados._

_En este capítulo, utilizaremos archivos de la carpeta_ **Farnsworth House Data Set &gt; Supporting Files**. Si aún no lo ha hecho, asegúrese de descargar las carpetas necesarias o todo el conjunto de datos desde los _**conjuntos de datos de la parte 1 de FormIt Primer**._

## **Importar y editar archivos SKP**

_En primer lugar, vamos a añadir el contenido descargado en su propia biblioteca de contenido personal_. Tenga en cuenta que en este ejercicio solo utilizaremos archivos SKP. Para obtener más información sobre cómo abrir o importar otros formatos de archivo, consulte [**esta entrada del blog sobre las funciones de FormIt 2021.2**](https://formit.autodesk.com/blog/post/formit-2021-2-and-new-revit-add-in-now-available) y **este capítulo sobre** **la importación y la exportación ampliadas de formatos de archivo**.

1 - Asegúrese de utilizar la opción **Guardar \(Ctrl + S\)** para guardar cualquier trabajo abierto y, a continuación, inicie un nuevo boceto de FormIt. Para ello, puede realizar lo siguiente:

1. Abra otra sesión en FormIt en una nueva ventana. Para ello, haga clic con el botón derecho en el icono de FormIt de la **barra de tareas de Windows** y, a continuación, haga clic en el icono de **FormIt**. Esta acción abrirá una nueva ventana de FormIt, que permite ejecutar dos sesiones de FormIt en paralelo.
2. O bien, después de guardar, inicie un **Nuevo boceto \(Ctrl + N\)** desde el menú desplegable **Archivo** de la barra de **Menú principal**.

![](../../.gitbook/assets/0%20%2819%29.png)

2 - Cree una nueva carpeta denominada **Custom FormIt Content** dentro de **Farnsworth House Data Set &gt; Supporting Files &gt; FormIt** en el _**conjunto de datos de Farnsworth House**._

3 - Utilice la opción **Guardar \(Ctrl + S\)** para guardar el nuevo boceto en esa carpeta. Se recomienda asignarle el nombre **Ottoman – Barcelona\_Mies.axm**

4 - En el nuevo archivo de FormIt vacío, realice lo siguiente:

1. **Importe un archivo local \(Ctrl + I\)**. Para ello, seleccione**Importar &gt; localmente...** en el menú desplegable **Archivo** de la barra de **Menú principal**.
2. Seleccione **Ottoman – Barcelona\_Mies.skp** en **Farnsworth House Data Set &gt; Supporting Files &gt; SketchUp** y haga clic en **Abrir**.

_**Nota:**_ _Si no aparece el archivo_ _**Ottoman – Barcelona\_Mise.skp**, asegúrese de que el menú desplegable de formatos de archivo se haya establecido en_ _**Todos los formatos admitidos**._

![](../../.gitbook/assets/1%20%287%29.png)

5 - Cambie el nombre del grupo importado **Ottoman - Barcelona\_Mies**.

6 - Cuando finalmente importemos este modelo en nuestro archivo de Farnsworth House, se colocará mediante el punto de **origen** de este archivo. Para controlar el punto de inserción l, vamos a mover el grupo **Ottoman - Barcelona\_Mies** para que sus esquinas se encuentren en el **origen**. Para:

1. Asegúrese de que **Forzar cursor a rejilla \(SG\)** esté activado. Dibuje una **Línea \(L\)** de referencia que comience en el **origen** \(Los ejes X, Y y Z se intersecan\). Haga clic en cualquier lugar para colocar el segundo punto.
2. Seleccione el grupo "Ottoman" e inicie el comando de desplazamiento haciendo clic una vez en la esquina inferior izquierda de su pata, como se muestra. _Para obtener más información sobre cómo desplazar objetos, consulte los capítulos anteriores._
3. Mueva el grupo al **origen** forzando el cursor al punto inicial de la línea de referencia que acabamos de dibujar.
4. Suprima la línea de referencia.

![](../../.gitbook/assets/2%20%2817%29.png)

7 - Es recomendable suprimir todas las capas no deseadas que se hayan importado con el archivo SKP, ya que cualquier capa que tenga este modelo se importará antes o después a nuestro modelo de la Farnsworth House. Para ello, vaya a la **paleta Capas**, seleccione **Capa 0** y haga clic en el botón **-**. De este modo, se suprimirá la capa manteniendo su geometría.

![](../../.gitbook/assets/3%20%2816%29.png)

_**Nota:**_ _Cuando se suprime una capa, cualquier geometría o grupo que se encontraban en esa capa se asigna a_ _**No hay capas**, que es el valor por defecto para cualquier objeto que no se haya asignado aún a una capa._

## **Crear miniatura de contenido**

_En este paso siguiente, se configurará una escena para que se utilice como la miniatura de_ _**contenido**_ _, que se mostrará en la_ _**paleta Biblioteca de contenido**._

1 - Para definir los parámetros de vista de la escena en miniatura, realice lo siguiente:

1. En la ficha **Entorno** de la **paleta Estilos visuales**, desactive todas las casillas de verificación y establezca el color **Inferior / fondo** en blanco.
2. Asegúrese de que el modo de vista se haya establecido en **Perspectiva** **\(VP\)**.
3. Utilice las **herramientas de navegación de vistas** para ampliar la vista y seleccionar una ubicación de cámara que represente bien el objeto de forma similar a la imagen siguiente.

![](../../.gitbook/assets/4%20%2813%29.png)

2 - Para guardar los parámetros que acaba de definir, cree una escena. Para ello, realice lo siguiente:

1. Vaya a la **paleta Escena**.
2. Haga clic en el botón **+**. Esta acción creará una nueva escena basada en los parámetros actuales.
3. Cambie el nombre de la **miniatura** y asegúrese de que estén activadas al menos las cuatro primeras casillas de verificación \(4\): **Cámara**, **Capas**, **Sol y sombras** y **Estilos visuales**. El resto de los parámetros de escena no son realmente pertinentes para crear la imagen en miniatura.
4. Utilice el botón **Actualizar escena** siempre que desee actualizar la **escena** para que coincida con la vista de cámara y la configuración visual actuales.

![](../../.gitbook/assets/5%20%2811%29.png)

3 - Utilice la opción **Guardar \(Ctrl + S\)** para guardar de nuevo el modelo de otomana completado. Tenga en cuenta que la **miniatura de contenido** se crea a partir de la vista activa al guardar por última vez el modelo, por lo que asegúrese de que se encuentra en la **escena en miniatura** antes de guardar.

_Si lo desea, puede comparar su archivo con el nuestro. Para ello, abra el archivo_ _**Ottoman - Barcelona\_Mies.axm**_ _guardado en_ _**Farnsworth House Data Set &gt; Supporting Files &gt; FormIt &gt; Furniture**_ _en el_ _**conjunto de datos de Farnsworth House**.‌_

_Puede seguir los mismos pasos anteriores con los archivos SKP de banco y silla, ubicados en la misma carpeta que la otomana._

_**Consejo:**_ _Para agilizar el proceso, es recomendable utilizar el archivo_ _**Ottoman - Barcelona\_Mies.axm**_ _que acaba de crear como plantilla. Durante el modelado, es posible que desee activar de nuevo las opciones_ _**Rejilla**_ _y_ _**Ejes**_ _de la_ _**paleta Estilos visuales**. Al ajustar solo la posición de la cámara de la __**escena de miniatura**__ para cada mueble, se garantiza la coherencia de las __**miniaturas de contenido**__entre todos los modelos de contenido._

## **Vincular una biblioteca de contenido**

_Ahora vuelva al proyecto de Farnsworth House. Aprenderemos a vincular la carpeta de **FormIt** en el **conjunto de datos de la Farnsworth House**, para acceder fácilmente a todos sus archivos, incluido el_ **contenido de FormIt personalizado** _que acabamos de crear, desde nuestro proyecto._

1 - Después de regresar al modelo de la Farnsworth House o volver a abrirlo, realice lo siguiente: _Si no ha completado el último capítulo, descargue y abra el archivo_ _**1.11 - Import Models with Content Library.axm**_ _del_ _**conjunto de datos de Farnsworth House**._

1. Abra la **paleta Biblioteca de contenido** y haga clic en el icono **Vincular directorio de biblioteca de contenido**. Aparecerá la ventana **Preferencias** con la ficha **Biblioteca de contenido** abierta.
2. Haga clic en el icono **+** para **Añadir una nueva ubicación de biblioteca de contenido**. Aparecerá una tercera ventana para que se desplace por el directorio del equipo y seleccione una carpeta.
3. En el _**conjunto de datos de Farnsworth House**, desplácese por las carpetas:_ _**Supporting Files > FormIt**. Aquí encontrará las carpetas_ que contienen los archivos **.axm** que hemos creado anteriormente en este capítulo. Haga doble clic en la carpeta **FormIt** para seleccionarla.
4. Haga clic en **Seleccionar carpeta**; la ruta de esa carpeta se mostrará en el panel **Ubicaciones de biblioteca - Local**.
5. De nuevo en la ventana **Preferencias**, haga clic en **Aceptar**; la carpeta vinculada se añadirá a la **Biblioteca de contenido**.
6. Para acceder a esta nueva biblioteca, abra el menú desplegable en la parte superior de la **paleta Biblioteca de contenido** y seleccione **FormIt**.
7. Tenga en cuenta que la estructura de carpetas y todos los archivos **.axm** de la carpeta vinculada se mostrarán en la **paleta Bibliotecas de contenido**. Haga doble clic en cualquier subcarpeta para acceder a los archivos que contiene.

![](../../.gitbook/assets/link-library-content.png)

**Nota:** Si tiene acceso a **Autodesk Docs** \(conocido anteriormente como Autodesk 360\), también puede acceder a los archivos que haya almacenado en este servicio a través del menú desplegable **Biblioteca de contenido**.

## **Colocar contenido desde la biblioteca**

_Ahora colocaremos los elementos de contenido creados dentro del modelo de Farnsworth._

1 - A fin de ver el interior de la casa y colocar los muebles, desactive la capa **Roof** y utilice **Orbitar \(O\)** para orbitar la vista en perspectiva hasta que pueda ver todo el suelo del edificio principal.

2. De nuevo en la **paleta Biblioteca de contenido**, asegúrese de que la lista desplegable siga establecida en **FormIt**. Antes de colocar el mobiliario que acabamos de crear, debemos colocar el "núcleo" de la casa:

1. Haga clic en la carpeta denominada **Other** para abrirla y, a continuación, haga clic en la miniatura de **Farnsworth House – Core** para seleccionarla.
2. Coloque el cursor sobre el **suelo del edificio principal** a fin de hacer clic en el **centroide** del suelo para colocar el **núcleo**.
3. Para volver a la carpeta FormIt, utilice el botón **Desplazarse arriba**.

![](../../.gitbook/assets/7%20%282%29.jpeg)

3 - Establezca la cámara en **Ortogonal \(VO\)**, **Vista superior \(VT\)**, y desactive el **suelo del edificio principal** para ver la **imagen del plano**. Consulte los capítulos anteriores para obtener más información sobre los parámetros de **vistas** y **capas**.

4 - Seleccione **Farnsworth House - Core** y mueva el elemento hasta que se alinee con la imagen del plano.

![](../../.gitbook/assets/8%20%281%29.png)

_**Nota:**_ _Al mover el_ _**núcleo**, tenga cuidado de no cambiar su elevación. Puede utilizar la tecla_ _**Mayús**_ _para restringir el movimiento a fin de que siempre se realice a lo largo de uno de los ejes o asegúrese de que los puntos de referencia inicial y final del comando_ _**Mover \(M\)**_ _se encuentren ambos a la misma altura. Para ello, haga clic en la_ _**imagen del plano**, no en el propio_ _**núcleo**_ _. Consulte los capítulos anteriores para obtener más información sobre la herramienta __**Mover \(M\)**__.‌_

## **Colocar mobiliario desde la biblioteca**

1 - Mediante un proceso similar, ahora puede colocar los muebles que ha creado anteriormente en este capítulo desde la carpeta **Custom FormIt Content**. Si no ha convertido los tres \(3\) archivos SKP, puede utilizar las versiones creadas anteriormente de la carpeta **Furniture**.

_**Notas:**_

* _Vuelva a activar la capa_ _**Main Building Floor**_ _para poder colocar mobiliario directamente en la superficie del_ _**suelo del edificio principal**._
* _Al colocar un nuevo objeto, utilice la tecla_ _**Tab**_ _para alternar entre los planos de colocación._
* _Al colocar un nuevo objeto, utilice la_ _**barra espaciadora**_ _para rotarlo 90 intervalos antes de colocarlo._

![](../../.gitbook/assets/9%20%283%29.png)

2. Del mismo modo, explore las **muestras de la biblioteca de contenido** para insertar contenido OOTB. Tenga en cuenta que varios de estos elementos presentan diversos tamaños entre los que elegir, de modo similar a los tipos de familia en Revit.

![](../../.gitbook/assets/10%20%286%29.png)

## **Uso de la herramienta Escala**

1 - Mediante las técnicas que acaba de aprender, coloque un ejemplar del componente **tree\_pine** desde la carpeta **Farnsworth House Data Set &gt; FormIt &gt; Planting**.

1. Una vez insertado, seleccione el grupo y cámbiele el nombre a **Tree**. Haga clic con el botón derecho para acceder al **menú contextual** y seleccione **Escala no uniforme \(NU\)**.
2. Haga clic en uno de los **botones de Escala no uniforme** para cambiar el tamaño y las proporciones del grupo **Tree** según sea necesario.

![](../../.gitbook/assets/11%20%283%29.png)

![](../../.gitbook/assets/12%20%282%29.png)

_**Nota:**_ _Del mismo modo, la herramienta_ _**Escala \(SC\)**_ _se puede utilizar para volver a ajustar la escala de todo el modelo o grupo de modo uniforme._

2 - Copie este grupo y coloque varios árboles alrededor de la casa mediante las **herramientas de escala** a fin de crear una gran variedad de tamaños y proporciones.

![](../../.gitbook/assets/13%20%286%29.png)

_**Nota:**_ _Aunque los árboles son ejemplares del mismo grupo, hemos podido_ _**ajustar su escala**_ _a diferentes tamaños. Mediante las herramientas_ _**Escala \(SC\)**_ _y_ _**Escala no uniforme \(NU\)**_ _fuera del modo de edición de grupos, puede modificar ejemplares individuales del mismo grupo. Si editamos uno de los grupos_ _**Tree**_ _y modificamos su geometría o material, todos los ejemplares del grupo se actualizarán, pero cada uno conservará su escala personalizada actual. Pruébelo._

### **Mantener el modelo ordenado**

_Recuerde ordenar siempre el contenido añadido en capas. En este ejemplo, es recomendable colocar el núcleo y todo el mobiliario en la capa_ _**Main Building Floor**_ _y los árboles en la capa denominada_ _**Planting**._

