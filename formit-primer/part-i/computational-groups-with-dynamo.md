# 1.10 - Grupos de cálculo con Dynamo

_En este capítulo, aprovecharemos la potencia de cálculo de_ [_**Dynamo**_](http://dynamobim.org/) _para colocar y modificar grupos flexibles vinculados a muestras de gráficos de Dynamo de OOTB._

_Si no ha completado la última sección, descargue y abra el archivo_ _**1.10 – Computational Groups with Dynamo.axm**_ _en los_ _**conjuntos de datos de la parte 1 de FormIt Primer**._

_Puede_ [_**obtener más información aquí**_](http://formit.autodesk.com/page/formit-dynamo) _sobre cómo funcionan juntos FormIt y Dynamo para los flujos de trabajo de diseño computacional._

## **Crear escaleras de terraza interior**

1 - Asegúrese de que las capas **Lower Terrace, Main Building Floor** y **Plan Image** estén activadas, ya que es aquí donde vamos a añadir la escaleras.

2 - Para colocar un grupo de escaleras vinculado a una de las muestras de Dynamo de OOTB:

1. Abra la **paleta Dynamo** en la barra de paletas. Debería ver algunos objetos de Dynamo integrados en el directorio de **muestras de Dynamo**.
2. Haga clic una vez en la muestra de Dynamo **Stairs** para llevarlo al espacio modelo. FormIt ejecutará el gráfico entre bastidores y generará la geometría de escalera a partir de este gráfico.
3. Mueva el cursor sobre el lienzo y, una vez cargada la escalera, se desplazará una vista preliminar fantasma de la geometría de la escalera junto con el ratón. Mueva el cursor sobre el lienzo, cerca de la terraza, y haga clic para colocar la escalera. Pulse **Esc** para anular la selección. Tenga en cuenta que, después de colocar las escaleras, la **paleta Propiedades** se abrirá automáticamente.

![](../../.gitbook/assets/0%20%2815%29.png)

_**Nota:**_ [_**También puede vincular directorios locales**_](https://formit.autodesk.com/page/formit-dynamo#dynamo-getting-started) _que contengan gráficos de Dynamo y ejecutar sus propios gráficos locales de Dynamo como estas muestras._

3 - Para actualizar las cotas de las escaleras, realice lo siguiente:

1. Con el grupo de escaleras seleccionado, modifique las entradas disponibles en la sección **ENTRADAS** de Dynamo en la parte inferior de la **paleta Propiedades** para que coincidan con las que se muestran a continuación. En la mayoría de los grupos creados mediante las secuencias de comandos de Dynamo, se incluirá una sección de Dynamo cuando se seleccionen.
   * Add Top Landing = False
   * Add Middle Landing = False
   * Add Bottom Landing = False
   * Floor-to-Floor Height = 2,6
   * Stair Width = 12
   * Riser Height = 0,6
   * Tread Length = 1,25
   * Tread Overlap = 0,25
   * Tread Thickness = 0,25
   * Height Between Middle Landings = \(no es pertinente porque no se está creando ningún descansillo central\)
   * Middle Landing Length = \(no es pertinente porque no se está creando ningún descansillo central\)
   * Top/Bottom Landing Length = \(no es pertinente porque no se está creando ningún descansillo\)
2. Haga clic en el botón **Ejecutar** para volver a ejecutar la secuencia de comandos de Dynamo con los valores de entrada actualizados.
3. Mueva el grupo según sea necesario para colocar la escalera en la ubicación correcta en consonancia con la **imagen del plano**. Tenga cuidado de no cambiar la elevación del grupo de escaleras al moverlo. Consulte los capítulos anteriores para obtener más información sobre los trucos y las técnicas al mover elementos de modelo.

![](../../.gitbook/assets/1%20%2811%29.png)

_**Nota:**_ _La entrada de_ _**Floor-to-Floor Height**_ _es una aproximación de la altura total de la escalera. El parámetro_ _**Riser Height**_ _define realmente la altura de las escaleras. En este ejemplo, se establece el valor de __**Floor-to-Floor Height**__ en 2,6', pero la altura final de la escalera es de 3,0' \(0,6' de \(**Riser Height**\) x 5 \(número de contrahuellas\)\). Dado que el intervalo entre el suelo y la parte superior del suelo de la terraza es de 3'-2", los 2" restantes se encuentran en la contrahuella superior._

## **Crear las escaleras del edificio principal**

_En los pasos anteriores, hemos creado una escalera sin descansillos. Ahora crearemos una escalera que utiliza un descansillo superior que se alinea con el_ _**suelo del edificio principal**._

1 - Realice primero una copia de las escaleras que acabamos de crear, como se indica a continuación:

1. Seleccione la escalera existente y, a continuación, haga clic en cualquier lugar de la **imagen del plano** para iniciar un comando de desplazamiento. Esta acción permitirá que FormIt utilice la elevación de la **imagen del plano** como la altura de referencia inicial para colocar la nueva copia. Pulse **Ctrl** para realizar una **copia rápida**.
2. Mueva el cursor en una ubicación más próxima al edificio principal por encima de la terraza. Observe que ahora la cara superior de la terraza es el nuevo plano de referencia. Haga clic para colocar el grupo.

![](../../.gitbook/assets/2%20%289%29.png)

_**Nota:**_ _Como la_ _**imagen del plano**_ _se encuentra en el plano de_ _**nivel de suelo**_ _, la_ _**herramienta Mover**_ _utilizará ese plano como referencia para su punto inicial. Obsérvese la información de herramientas_ _**En la cara**_ _de la imagen de arriba, que indica que la cara de la imagen del plano está seleccionada como referencia inicial y la cara superior del_ _**suelo de la terraza superior**_ _está seleccionada como la referencia final._

2. Utilice la herramienta **Establecer como exclusivo \(MU\)** para que, al cambiar las entradas de Dynamo de esta escalera, esto no afecte a la escalera inferior. Cambie la posición del grupo según sea necesario para que esté cerca de su ubicación final. Lo ajustaremos de forma más precisa posteriormente. Puede activar o desactivar la visibilidad de la capa **Lower Terrace** para ver el plano siguiente para ayudarle a colocarla, pero tenga cuidado de no cambiar el alzado de la nueva escalera a medida que la desplaza.

3 - En la **paleta Propiedades**, actualice las **entradas de Dynamo** como se muestra a continuación y ejecute la secuencia de comandos una vez más.

* Add Top Landing = True
* Floor-to-Floor Height = 2,333
* Riser Height = 0,466
* Tread Length = 1,5
* Top/Bottom Landing Length = 2,5

![](../../.gitbook/assets/3%20%281%29.jpeg)

_**Nota:**_ _Si establece_ _**Add Bottom Landing**_ _en_ _**True**_ _y vuelve a ejecutar la secuencia de comandos, la cara superior del descansillo inferior debería alinearse con la cara superior del_ _**suelo de la terraza inferior**. Esto sucede porque, a diferencia de las escaleras anteriores, hemos ajustado el valor de_ _**Riser Height**_ _para que coincida con el valor de_ _**Floor-to-Floor Height**_ _en la verdadera altura que deseamos \(2'-4'' o 2,333'\)._

2 - Vuelva a colocar el grupo en su posición final. El descansillo superior debe estar nivelado con el **suelo del edificio principal**.

3 - Para finalizar las escaleras, añada el material **Stone - Travertine** para que coincida con los suelos. Para obtener más información sobre cómo aplicar materiales, consulte los capítulos anteriores.

