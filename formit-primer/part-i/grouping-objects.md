# 1.5 - Agrupar objetos

_Los grupos en FormIt funcionan de forma similar a las familias de Revit y los componentes de SketchUp. La agrupación de objetos distintos impide que se una su geometría. Las copias de un grupo actúan como ejemplar de la geometría original, lo que significa que los cambios realizados en una copia afectarán a todas ellas._

_Si no ha completado la última sección, descargue y abra el archivo_ _**1.5 - Group Objects.axm**_ _de los_ _**conjuntos de datos de la parte 1 de FormIt Primer**._

## **Crear un grupo**

1 - Haga doble clic en la masa de terraza superior para seleccionarla.

2 - Haga clic con el botón derecho y seleccione **Grupo \(G\)** o simplemente pulse **G**.

![](../../.gitbook/assets/0%20%281%29.jpeg)

3 - Observe que después de crear un grupo, se incluye automáticamente en la herramienta Mover.

## **Desplazar un grupo**

1 - Para facilitar el proceso de modelado, active la opción **Forzar cursor a rejilla \(SG\)** si estaba desactivada.

![](../../.gitbook/assets/1%20%2814%29.png)

2 - Para empezar a mover el objeto seleccionado, mientras sigue en el comando **Mover \(M\)**, haga clic una vez en cualquier esquina inferior de la masa. A continuación, desplace el cursor hacia arriba y verá que aparece una línea de eje \(Z\) azul. Esta línea le ayudará a mover el objeto en línea recta.

3 - Con el eje azul visible, escriba **4'-6"**; aparecerá un cuadro de diálogo de cota. Después de introducir la cota, haga clic en **Aceptar** o pulse **Intro** en el teclado. De este modo, se desplazará toda la masa hacia arriba fuera del plano de suelo a lo largo del **eje Z**.

_**Nota:**_ _Al igual que en Revit, también puede especificar_ _**4'6**,_ _**4'6'',**_ _o_ _**4,5**, y el programa interpretará el valor como 4 \(pies\) 6 \(pulgadas\) al utilizar unidades imperiales._

![](../../.gitbook/assets/2%20%282%29.png)

## **Editar un grupo**

1 - Para acceder al **modo de edición de grupo**, haga doble clic en la masa.

1. En la **paleta Propiedades**, cambie el nombre del grupo **Masa - Edificio principal**.
2. Para guardar los cambios y salir del **modo de edición de grupo**, haga clic en el icono de marca de verificación **Finalizar edición de grupo** en la esquina superior izquierda del lienzo o haga doble clic fuera del espacio.

![](../../.gitbook/assets/3%20%2812%29.png)

_**Notas**:_

* _Para obtener información sobre las opciones de_ _**Categoría**_ _, vaya al capítulo_ _**Trabajar con Revit**_ _._‌
* _Cada grupo tiene su propio historial de deshacer/rehacer distinto al del proyecto general; puede hacer clic en las flechas_ _**Deshacer**_ _y_ _**Rehacer**_ _del_ _**Asistente para editar grupos**_ _en la esquina superior izquierda del lienzo._

## **Aplicar niveles a un grupo**

_**Nota:**_ _La agrupación de una geometría reemplaza la configuración anterior que es posible que se haya aplicado a la geometría. Por ello, deberá volver a aplicar los niveles del ejercicio anterior._

1 - Para aplicar niveles a un grupo, realice lo siguiente:

1. Haga clic una vez en el grupo **Massing** **- Main Building** para seleccionarlo.
2. Vaya a la **paleta Propiedades** y active **Utilizar niveles.**
3. Mantenga solo el nivel del **edificio principal**. Para eso, desactive todos los demás.
4. En el campo **Área por nivel**, se mostrará el área bruta de los objetos seleccionados actualmente. El área de cada **nivel** se muestra delante del nombre de cada **nivel**.
5. Si no aparece una línea de nivel azul que cruce el objeto horizontalmente, active la visualización del nivel en el**menú Configuración &gt; Estilo visual &gt; Mostrar niveles \(DL\).**

_**Nota**: Si no se ha notificado ningún área para el nivel del_ _**edificio principal**_ _, es posible que la geometría no se interseque con el nivel, debería encontrarse a una altura de 4'-6''. Para solucionar los problemas, cambie la posición de la geometría o la altura del_ _**nivel**_ _para que se intersequen._

![](../../.gitbook/assets/levels-to-groups.png)

2 - Anule la selección del grupo. Para ello, pulse la tecla **Esc** o haga clic fuera del espacio. Sin ningún objeto seleccionado, la **paleta Propiedades** informará del área bruta general del boceto en lugar del área de un objeto específico.

![](../../.gitbook/assets/5%20%2815%29.png)

## **Administrar grupos**

1 - Para ver y administrar todos los grupos del boceto, realice lo siguiente:

1. Vaya a la **paleta Árbol de grupos**. En esta, aparecerá lo siguiente:
   * **Grupo Terreno**: grupo creado automáticamente cuando se importó la **imagen de satélite**.
   * **Masa - Edificio principal**: el grupo de geometría de masa de construcción que acabamos de crear.
   * **grupo 2**: grupo sin nombre que contiene la imagen del plano de planta.
2. Para cambiar el nombre del **grupo 2**, mediante la paleta Árbol de grupos, haga doble clic en **grupo 2** y, a continuación, escriba **Imagen del plano**.

![](../../.gitbook/assets/6%20%284%29.png)

_**Notas:**_

* _Para mantener un modelo organizado, es recomendable que los nombres de grupo sean descriptivos._
* _Este es un método útil para administrar y editar todos los grupos del modelo desde una ubicación._

2. Con el grupo **Imagen del plano** seleccionado, vaya a la **paleta Propiedades**. Tenga en cuenta que el nombre del grupo también se ha actualizado en el campo **Grupo**.

![](../../.gitbook/assets/7.png)

## **Ocultar contexto del grupo**

_Esta herramienta permite ocultar rápidamente toda la geometría fuera del grupo que está modificando. Es muy útil cuando se tiene un modelo grande y complejo y otras geometrías se interponen en el camino._

1 - Para aislar un grupo, realice lo siguiente:

1. Haga doble clic en su geometría para editar el grupo.
2. Desplácese a **Configuración** en el **menú principal** y active la opción **Ocultar contexto del grupo** o simplemente pulse **H** en el teclado. Observe cómo desaparece la **imagen del plano**.
3. Termine de editar el grupo. Tenga en cuenta que el modo **Ocultar contexto del grupo \(H\)** solo está activo mientras se encuentra en el **Asistente para editar grupos**.
4. Para desactivar de nuevo este modo, simplemente pulse **H**. Esta opción se puede activar o desactivar en cualquier momento, dentro o fuera de un grupo.

![](../../.gitbook/assets/8%20%285%29.png)

