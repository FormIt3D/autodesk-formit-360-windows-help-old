# 1.15 - Trabajo con Revit

_Una de las funciones más interesantes de FormIt es la posibilidad de transferir el modelo de un entorno de modelado flexible como FormIt a un potente entorno paramétrico como Revit. En este capítulo, realizaremos algunos ejercicios que transfieren varios elementos de FormIt a Revit y viceversa._

_En este capítulo, se utilizarán familias de Revit de muestra. Si aún no lo ha hecho, puede descargarlas en el conjunto de datos de **Farnsworth House.** Si no ha seguido todo el aprendizaje hasta este momento, también puede descargar y abrir el archivo **1.15 – Working With Revit.axm** desde los **conjuntos de datos de la parte 1 de FormIt**._

_En estos ejercicios, utilizaremos la versión Revit 2022, en la que se han mejorado las funciones de interoperabilidad con FormIt. Las versiones anteriores de Revit no presentan algunas o ninguna de las funciones que se muestran en este aprendizaje y tienen una interfaz de usuario diferente._

## De Revit a FormIt

### Convertir familias de Revit para su uso en FormIt

Si usted \(o su empresa\) tiene una gran cantidad de familias de Revit que desea utilizar en FormIt, le interesará esta sección, que explica cómo exportar archivos RFA por lotes a FormIt.

_**Nota:**_ _En los pasos siguientes, se muestran la interfaz y las acciones necesarias al utilizar Revit 2022. No obstante, las herramientas de_ _**Convertir RFA a FormIt**_ _llevan disponibles desde Revit 2016._

1 - Abra un nuevo proyecto o familia de Revit. A continuación, realice lo siguiente:

1. En la cinta de opciones **Complementos**, busque el panel **Conversor a FormIt** y haga clic en el botón **Convertir RFA a FormIt**. Se abrirá el cuadro de diálogo **Convertir familias de Revit**.
2. En el campo **Ruta a los archivos de la familia de Revit**, vaya a la ubicación en la que haya guardado la siguiente carpeta en el equipo: **Farnsworth House Data Set &gt; Supporting Files &gt; Revit**.
3. En el campo **Ruta al contenido de FormIt:**, vaya a **Farnsworth House Data Set &gt; Supporting Files &gt; FormIt &gt; Custom FormIt Content**. Si no ha completado el capítulo **1.11 Importar modelos con la biblioteca de contenido**, es posible que deba crear la carpeta **Custom FormIt Content** o elegir otro destino.
4. Haga clic en **Aceptar** para iniciar el proceso de conversión.

![](../../.gitbook/assets/0%20%2823%29.png)

_**Notas:**_

* _Este proceso tardará algo de tiempo en completarse, ya que Revit abre el archivo_ _**RFA**_ _de la primera ruta, lo convierte y, después, lo guarda con el formato_ _**AXMF**_ _para FormIt._
* _En este ejercicio, solo convertiremos un único archivo, pero puede utilizar este proceso para convertir por lotes todos los archivos_ _**RFA**_ _de la carpeta seleccionada \(incluidos todos los archivos_ _**RFA**_ _de las carpetas anidadas\)._

2 - Una vez completado el proceso, regrese a FormIt. Allí verá que el nuevo contenido aparece en la **paleta Biblioteca de contenido**, dentro de la carpeta **FormIt &gt;** **Custom FormIt Content** que hemos vinculado anteriormente. Si ha guardado los archivos **AXMF** convertidos en una ubicación diferente o no ha completado el capítulo **1.11 Importar modelos con la biblioteca de contenido**, es posible que deba añadir esa carpeta a la biblioteca para ver su contenido. Consulte el capítulo 1.11 para obtener instrucciones sobre cómo añadir carpetas a la biblioteca de contenido.

![](../../.gitbook/assets/1%20%2824%29.png)‌

**Nota** _No todas las categorías de Revit se pueden exportar. Se admiten las familias "independientes" o "basadas en niveles", pero no las familias "basadas en anfitrión" como puertas y ventanas. Se admiten Masa, Muebles de obra, Mobiliario, Sistema de mobiliario, Modelo genérico, Aparcamiento, Emplazamiento y Equipos especializado. Todas las familias no admitidas de la carpeta seleccionada simplemente se omitirán._

## De FormIt a Revit

_Existen dos métodos diferentes para llevar la geometría de FormIt a Revit. Puede importar un archivo_ _**.axm** existente en un proyecto de Revit o en un archivo de familia de Revit, que se comportará de forma similar a un modelo importado o un archivo CAD. También puede iniciar FormIt desde Revit y incluir cada grupo de FormIt en Revit como un elemento de modelo genérico individual. El segundo método se describe en el capítulo de la **parte 2**_ _**2.8**_ _**Flujos de trabajo avanzados de Revit**._

### Importación de Farnsworth House a Revit

1 - Para importar un archivo de FormIt \(**.axm**\) a Revit, inicie un nuevo proyecto de Revit y abra la vista 3D por defecto. A continuación, realice lo siguiente:

1. Vaya a la **ficha Insertar** y haga clic en el botón **Importar CAD**. Se abrirá la ventana **Importar formatos CAD**.
2. Asegúrese de que la lista desplegable **Archivos de tipo** se haya establecido en **Archivos de FormIt\(\*.axm\)**.
3. Busque y seleccione el archivo **.axm** de Farnsworth en el que ha estado trabajando. Si no ha seguido la parte 1 de FormIt Primer, también puede abrir el archivo **1.15 – Working With Revit.axm** la carpeta **Farnsworth House Data Set &gt; Chapter Files**.
4. Asegúrese de que la opción **Import. niv. FormIt** esté activada.
5. Una vez definidos los parámetros, haga clic en **Abrir**; la geometría FormIt se incorporará en Revit como un solo elemento.

![](../../.gitbook/assets/2%20%2824%29.png)

Importación de un archivo de FormIt mediante el botón de importación de CAD.

![](../../.gitbook/assets/3%20%2821%29.png)  
Elemento .axm importado. Observe que los niveles del modelo FormIt también se importan a Revit.

_Al igual que otros formatos CAD, las capas del archivo original se importan a Revit. Esta función permite definir diferentes parámetros de visibilidad para cada capa a fin de manipular fácilmente el aspecto gráfico del archivo de FormIt en cualquier vista de Revit._

2 - Para ajustar la visibilidad de la capa del archivo .axm importado:

1. Vaya a la ventana **Modificaciones de visibilidad/gráficos \(VG o VV\)**, ficha **Categorías importadas**, expanda el archivo de FormIt importado y desactive la capa **Planting** para desactivar la capa de la vista actual y haga clic en **Aceptar**.
2. Cambie el **Estilo visual** a **Realista**; verá que todos los materiales FormIt se han importado en Revit.

![](../../.gitbook/assets/4%20%2820%29.png)

3. De hecho, los materiales de FormIt importados estarán disponibles en este proyecto de Revit, etiquetados con la clase **FormIt**. Solo tiene que abrir el **Explorador de materiales** y buscar "FormIt" para ver todos ellos. Ahora se pueden utilizar en el proyecto de Revit como cualquier otro material.

![](../../.gitbook/assets/5%20%2819%29.png)

