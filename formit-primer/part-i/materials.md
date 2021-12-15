# 1.7 - Pintar con materiales

Como vimos en un **ejercicio anterior**, puede crear sus propios materiales y, a continuación, pintar las caras con esos materiales en FormIt. En este ejercicio, creará y editará más materiales, además de importar materiales de la Biblioteca de materiales de Autodesk.

_Si no ha completado la última sección, descargue y abra el archivo_ _**1.7 - Paint with Materials.axm**_ _de los_ _**conjuntos de datos de la parte 1 de FormIt Primer**._

## **Crear los muros de cristal**

1 - Para ver el plano que contiene las cotas a las que vamos a hacer referencia, vaya a la **paleta Capas** y active la capa **Plan Image**.

2 - Seleccione la **herramienta Rectángulo \(R\)**. Vamos a crear un rectángulo directamente encima del grupo de suelos existente. Asegúrese de que no está editando el grupo de suelos, sino que está dibujando encima del objeto agrupado existente.

![](../../.gitbook/assets/0%20%283%29.png)

3 - Para iniciar el rectángulo del área de cristal, realice lo siguiente:

1. Haga clic en la esquina posterior del suelo existente y mueva el cursor del ratón por su borde más corto.
2. Escriba **28'-8"** para definir la longitud del primer borde y haga clic en **Aceptar**. Debe tener la misma longitud que el borde corto existente del suelo.
3. Para definir el segundo borde, empiece a mover el cursor del ratón a lo largo del borde más largo del suelo existente. Escriba **55'-5 ½"** para definir la longitud del segundo borde y, a continuación, haga clic en **Aceptar**.
4. Haga clic en **Esc** para salir de la herramienta Rectángulo. Haga clic una vez dentro del nuevo rectángulo para seleccionar la cara y empiece a arrastrarla hacia arriba.

![](../../.gitbook/assets/1%20%283%29.png)

4 - Para definir la altura, mueva el cursor del ratón hacia arriba a lo largo del **Eje Z**, pulse la tecla **Tab** y escriba **11'-2"**.

![](../../.gitbook/assets/2%20%284%29.png)

_**Nota:**_ _Siempre que utilice una herramienta para la que pueda introducir una cota, puede pulsar_ _**Tab**_ _o simplemente empezar a escribir números._

5 - Haga doble clic en **Grupo \(G\)** para agrupar la nueva geometría.

6 - Haga doble clic en el grupo para editarlo. En la **paleta Propiedades**, asigne al grupo el nombre **Glass Walls.**

![](../../.gitbook/assets/3%20%283%29.png)

7 - Para definir el grosor de la pared de cristal, realice lo siguiente:

1. Haga clic con el botón derecho en la cara superior y seleccione la **herramienta Desfasar cara \(OF\).**
2. Mueva el cursor del ratón hacia dentro y escriba **4".**
3. Haga clic dos veces en **Esc** para desactivar la herramienta y borrar la selección.

![](../../.gitbook/assets/4%20%2817%29.png)

​_**Nota:**_ _La unidad por defecto para proyectos con unidades imperiales es pies, igual que en Revit. Si introduce un único número sin una unidad especificada como_ _**4**, obtendrá_ _**4 pies\(4'\)**_ _y no_ _**4 pulgadas\(4"\)**._

8 - Para tallar el área interior, haga clic una vez en la cara superior interior para seleccionarla y, a continuación, haga clic de nuevo para iniciar la operación de **arrastre de cara**. Empuje la cara hacia abajo hasta que desaparezca y haga clic en el espacio para completar el proceso.

![](../../.gitbook/assets/5%20%2812%29.png)

_**Nota:**_ _En FormIt, a diferencia de otros programas, no se puede empujar accidentalmente la cara que se intenta suprimir "demasiado lejos" de modo que se forme una nueva extrusión negativa._

9 - Salga del modo **Editar grupo**. Para ello, haga doble clic fuera en el espacio o pulse **Esc.**

10 - Seleccione el grupo **Glass Wall** con un solo clic y colóquelo en la capa **Main Building Floor**.

![](../../.gitbook/assets/6%20%2813%29.png)

## **Importar un material de la Biblioteca de materiales de Autodesk**

1 - Vuelva a editar el grupo **Glass Wall**. Para ello, haga doble clic en él.

2 - Para importar un material nuevo al modelo, realice lo siguiente:

1. Vaya a la **paleta Materiales**.
2. Seleccione **Muestras de materiales** en el menú desplegable de la parte superior de la paleta para desplazarse por la **Biblioteca de materiales de Autodesk.** ​
3. Haga clic en la carpeta **Glass+Glazing** para abrirla.
4. Busque el material **Glass – Blue Tint** y haga clic una vez en él para añadirlo a la biblioteca de materiales **En el boceto**.
5. Observe que debería haber regresado a la biblioteca **En el boceto**, que ahora incluye el material recién seleccionado.

![](../../.gitbook/assets/7%20%288%29.png)

![](../../.gitbook/assets/8%20%288%29.png)

3 - Después de añadir el material, debe encontrarse automáticamente en la herramienta **Pincel**. De lo contrario, haga clic de nuevo una vez en el material **Glass – Blue Tint**. Para pintar todos los muros, haga doble clic en la geometría con la herramienta **Pincel**. Esta acción aplicará el material seleccionado a todo el objeto. ![](../../.gitbook/assets/9%20%281%29.png)​

4 - Haga clic en **Esc** para salir de la herramienta **Pincel**. Haga clic en **Esc** de nuevo o haga doble clic fuera en el espacio para salir del grupo.

## **Copia rápida del suelo para crear la cubierta**

1 - Para crear rápidamente la cubierta en función de la geometría del suelo:

1. Seleccione el grupo **Floor** con un solo clic.
2. Haga clic en una de las esquinas inferiores para iniciar la herramienta **Mover**.
3. Empiece a mover el suelo hacia arriba a lo largo del eje azul \(**Eje Z**\). Cree una **copia rápida**. Para ello, pulse la tecla **Ctrl**. Debe aparecer una vista preliminar fantasma de la copia. ​
4. Mientras se desplaza por el eje azul \(**Eje Z**\), comience a escribir **12' 2"**; aparecerá el **cuadro de diálogo Cota**. Haga clic en **Aceptar** o pulse **Intro** para finalizar la colocación.

![](../../.gitbook/assets/10%20%281%29.png)

![](../../.gitbook/assets/11%20%281%29.png)

## **Editar la cubierta**

1 - Con el grupo copiado seleccionado, utilice el comando **Establecer como exclusivo \(MU\)** para disociar este grupo del grupo de suelos.

2 - Haga doble clic en el grupo para editarlo. Cambie el nombre del grupo a **Roof** en la **paleta Propiedades**. Para salir del grupo, haga doble clic fuera del espacio.

3 - En la **paleta Capas**, cree una nueva **capa** denominada **Roof** y añádale el grupo **Roof**. Puede activar y desactivar la capa para comprobar que los elementos correctos se encuentren en la cubierta. Consulte el **capítulo 6** para obtener más información sobre cómo trabajar con **capas**.

4 - Regrese a la **paleta Materiales** e importe el material **Concrete - Broom Finish - Colorized 1** de la carpeta **Concrete+Asphalt** en la biblioteca **Muestras de materiales** **\(producción\)**. Tenga en cuenta que, al hacer clic en el material, la geometría seleccionada se pintará automáticamente y el nuevo material se añadirá a la biblioteca de materiales **En el boceto**.

![](../../.gitbook/assets/12.jpeg)

_**Nota:**_ _Pintar un grupo fuera del_ _**modo de edición de grupos**_ _es una técnica útil que permite pintar diferentes ejemplares del mismo grupo con distintos materiales._

## **Crear la terraza inferior**

1 - En función de la **imagen del plano**, cree la terraza interior con la herramienta **Rectángulo \(R\)** con una longitud de **55' 3"** y una anchura de **22'-7 3/4"** y extruya la forma en 1'. Coloque el nuevo rectángulo de forma que se encuentre a 8 5/8" de distancia del borde sur del edificio principal \(la profundidad de los pilares que crearemos más adelante\).

_**Notas**:_

* _Consulte los capítulos anteriores para obtener información sobre cómo dibujar y extruir rectángulos._
* _Es posible que deba activar o desactivar_ _**Forzar cursor a rejilla \(SG\)**_ _para hacer clic en_ la esquina de la terraza.

2 - Para finalizar la terraza inferior, realice lo siguiente:

1. Utilice la herramienta **Grupo \(G\)** para agrupar la geometría y asígnele el nombre **Lower Terrace Floor**.
2. **Desplace** el grupo hacia arriba **2'-2"** del plano de suelo.
3. Cree una nueva **capa** denominada **Lower Terrace** y y añádale el grupo.
4. Añada **Terrace Level Floor** al grupo

![](../../.gitbook/assets/13%20%281%29.png)

_**Nota:**_ _Esta imagen no representa el proceso paso a paso para crear y asignar la geometría a grupos, niveles y capas. Para obtener más información sobre estos procesos, consulte los capítulos anteriores de FormIt Primer._

3 - Importe el material **Stone &gt; Stone - Travertine**.

4 - En la **paleta Materiales**, busque el material **Travertine** y modifíquelo, como se indica a continuación:

1. Haga doble clic en el mosaico de vista preliminar para abrir el menú emergente **Editor de materiales**.
2. Haga clic en el mosaico de vista preliminar **Color** para abrir el menú emergente **Editor de colores**.
3. Cambie el campo **Val** a **190** para oscurecer el matiz del material.

![](../../.gitbook/assets/14%20%282%29.png)

5 - **Pinte** los grupos **Floor** y **Lower Terrace Floor** con el material **Travertine** modificado.

![](../../.gitbook/assets/15.jpeg)

