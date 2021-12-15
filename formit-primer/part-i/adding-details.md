# 1.9 - Adición de detalles

_FormIt es una excelente herramienta de masa, además de una fantástica herramienta de modelado. Empezaremos a añadir detalles a la Farnsworth House en forma de puertas y montantes para la caja de cristal. A continuación, abordaremos algunas herramientas adicionales y practicaremos el proceso de añadir nueva geometría, capas, materiales y administración de grupos._

_Si no ha completado la última sección, descargue y abra el archivo_ _**1.9 - Adding Details.axm**_ _desde los_ _**conjuntos de datos de la parte 1 de FormIt Primer**._

## **Crear marcos de ventana**

_Vamos a crear montantes y un marco metálico de 2" alrededor de la caja de cristal. Tenga en cuenta que estos montantes se solaparán intencionadamente con la caja de cristal._

1 - Cree una nueva capa denominada **Glass Walls** y desplace el grupo **Glass Wall** a ella.

2 - Para facilitar la visualización, desactive la capa **Roof** para que podamos ver toda la caja de cristal.

3 - Para comenzar a crear el primer marco de ventana, realice lo siguiente:

1. En el lado oeste del edificio, utilice la **herramienta Rectángulo \(R\)** para dibujar una nueva superficie directamente sobre la cara de cristal exterior. Asegúrese de crear la superficie fuera del grupo **Glass Walls**.
2. Seleccione y arrastre la cara recién creada **2"** hacia el interior. Pulse **Esc** para anular la selección. El resultado final debe tener un aspecto similar al de la imagen siguiente.
3. Haga clic una vez en la cara que acaba de crear. Haga clic con el botón derecho para acceder al **menú contextual** y utilizar la **herramienta Desfasar cara \(OF\).**

_**Nota:**_ _Si tiene problemas para seleccionar la nueva cara, pulse la_ _**barra espaciadora**_ _para alternar entre los diferentes objetos seleccionables o desactive temporalmente la capa_ _**Glass Walls**_ _._

![](../../.gitbook/assets/0.jpeg)

4 - Para definir la cota de desfase, mueva el cursor del ratón hacia el interior de la cara e introduzca **2"** para crear un rectángulo más pequeño.

![](../../.gitbook/assets/1%20%289%29.png)

5 - Haga clic una vez para seleccionar el rectángulo interior que acaba de crear. Haga clic de nuevo y arrastre la cara hacia el interior del edificio hasta que desaparezca. Haga clic una vez más para terminar de eliminar el volumen central de la geometría del marco.

![](../../.gitbook/assets/2%20%2821%29.png)

6 - Haga doble clic para seleccionar la geometría que acabamos de crear y utilice la opción **Grupo \(G\)** para agruparla. Asigne al grupo el nombre **Mullion Frame – EW**.

7 - Cree una capa denominada **Mullion** y coloque el nuevo grupo en ella.

8 - Para configurar el material del marco, realice lo siguiente:

1. En la **paleta Materiales**, duplique el material **Metal – Brushed – Colorized**. Para ello, haga clic con el botón derecho en él y seleccione **Duplicar material**.
2. Haga doble clic en el mosaico de vista preliminar del nuevo material para editarlo.
3. Cambie el nombre a **Metal – Brushed – Gray**.
4. Modifique el color del material. Para ello, haga clic en el mosaico **Color** de la sección **Mapas** y oscurezca el gris cambiando el valor **Val:** a **150**.

![](../../.gitbook/assets/3%20%284%29.png)

9 - Haga clic en **Aceptar** para guardar estos cambios en el nuevo material y, a continuación, pinte el grupo **Mullion Frame – EW** con él. Después, la **paleta Propiedades** del grupo debería coincidir con lo que se muestra en la imagen siguiente:

![](../../.gitbook/assets/4.jpeg)

10 - Cree un nuevo ejemplar del marco en el lado este mediante cualquiera de las siguientes herramientas: **Copia rápida**, **Matriz** o **Duplicar**.

11 - Repita los pasos anteriores para los lados norte y sur de la caja de cristal. Asigne al nuevo grupo el nombre **Mullion Frame – NS**. No olvide pintarlos y colocarlos en la capa **Mullion**.

![](../../.gitbook/assets/5%20%2816%29.png)

_**Nota:**_ _Los marcos de los montantes se solapan entre sí en las esquinas. Esto es intencionado. En el resultado de arriba, se muestra la geometría de marco de montante con las capas_ _**Glass Wall**_ _y_ _**Column**_ _desactivadas._

**Crear montantes**

1 - En un plano con la cara de cristal exterior en el lado sur o norte del edificio, dibuje un rectángulo de **2" x 10'-10" \(R\)** que se extienda desde la parte inferior y la parte superior del marco del montante. No se preocupe por la posición exacta del rectángulo a lo largo del marco, lo colocaremos en su lugar en los pasos siguientes.

![](../../.gitbook/assets/6%20%2811%29.png)

2 - Extruya el rectángulo hacia atrás **2"** y, a continuación, **Agrupe \(G\)** y asigne al grupo el nombre **Mullion – Vertical**. Coloque el grupo en la capa **Mullion** y píntelo con el material **Metal – Brushed – Grey**.

**Ubicación de los montantes**

_Ahora vamos a definir la ubicación del primer montante para que se centre en el __**Punto medio**__ de un pilar._

1 - Para volver a ver los pilares, active la capa **Column**, si estaba desactivada. Mientras se encuentra en la **paleta Capas**, también puede desactivar las capas **Lower Terrace** e **Plan Image** para facilitar los pasos siguientes.

2 - Para mover el montante a su nueva ubicación, realice lo siguiente:

1. Haga clic una vez para seleccionar el grupo de montantes verticales que acaba de crear. Utilice la función **Zoom \(Z\)** y haga clic en el **Punto medio** del borde exterior inferior del montante, representado por un triángulo rojo**.**
2. Empiece a mover la geometría horizontalmente hacia un pilar. Pulse **Mayús** para bloquear el movimiento en el eje rojo \(**Eje X**\). Tenga en cuenta que, una vez que el movimiento esté bloqueado, el eje rojo se volverá más grueso.
3. Reduzca la vista hasta que pueda ver la base del pilar. Mientras mantiene pulsada la tecla **Mayús**, haga clic en el **Punto medio** en la base de la cara exterior del pilar. El montante seguirá moviéndose únicamente a lo largo del eje rojo \(**Eje X**\), pero se alineará con el **Punto medio** en el que acaba de hacer clic.

![](../../.gitbook/assets/7%20%281%29.jpeg)

_**Nota:**_ _El montante ahora se encuentra directamente detrás del pilar. Desactive la capa_ _**Column**_ _o utilice_ _**Orbitar \(O\)**_ _para visualizar el montante._

3 - Pulse **Esc** para desactivar la herramienta **Mover**.

4 - Utilice la herramienta **Matriz \(AR\)** o **Copia rápida** para crear cuatro \(4\) montantes verticales más a lo largo del mismo lado con una separación de **11'**. Para obtener información sobre cómo utilizar la **herramienta Matriz**, consulte los capítulos anteriores.

5 - Utilice la tecla Tab para seleccionar todos los grupos de montantes **verticales** y cópielos en el lado opuesto del edificio para que tanto el marco **norte** como el **sur** tengan diseños de montantes idénticos, como se muestra en la siguiente imagen:

![](../../.gitbook/assets/8%20%286%29.png)

## **Crear montantes de puerta**

1 - Utilice la herramienta **Orbitar \(O\)** para orbitar la vista en perspectiva hasta que mire al centro del marco del montante oeste.

2 - De forma similar a la creación de marcos de montantes, dibuje un panel de puerta con una anchura de **3'-6"** y un marco de **2"x 2"**. Conviértalo en un **Grupo \(G\)** con las propiedades: nombre de grupo: **Curtain Wall Door**; capa: **Mullion**, y material: **Metal – Brushed – Grey**.

3 - Copie este grupo para crear el segundo marco de puerta y muévalo para que se centren en el grupo **Mullion Frame – EW**, como se muestra a continuación.

![](../../.gitbook/assets/9.jpeg)

## **Crear cornisa de cubierta con barrido**

_Ahora crearemos la cornisa de la Farnsworth House mediante una de las herramientas avanzadas de modelado de FormIt ,_ _**Barrido**. Para obtener más información sobre el modelado avanzado, consulte el capítulo_ **2.2 -** _**Herramientas avanzadas de modelado** en_ _la_ _**parte 2 de FormIt Primer**._

_El primer paso para crear un __**barrido**__ es dibujar un perfil perpendicular a la "extrusión" del barrido. Para ello, utilizaremos la geometría de la cubierta como guía._

1 - Active la capa **Roof** y amplíe una de sus esquinas.

2 - Con uno de los lados verticales de la cubierta como referencia, dibuje dos rectángulos adyacentes. El primero tendrá una anchura de **6"** por **4 5/8**" y, el segundo, de **2" por 2"**. Suprima la línea que divide los dos rectángulos para crear una única cara. El resultado debe tener el aspecto siguiente.

![](../../.gitbook/assets/10.jpeg)

3 - Para crear el barrido:

1. Sin geometría seleccionada, haga clic en el botón **Herramientas avanzadas de modelado** de la **barra de herramientas estándar** y seleccione **Barrido \(SW\)**.
2. El **Asistente para la selección de barridos** se iniciará y le solicitará que **Seleccione una cara \(o bordes\) para el perfil de barrido**. Seleccione la cara del perfil que acabamos de crear.
3. Una vez seleccionado el perfil, se le solicitará que **Seleccione una cara \(o bordes\) para el camino de barrido y, a continuación, haga clic en Finalizar**. Seleccione la cara superior de la cubierta. FormIt utilizará automáticamente los contornos de la cara seleccionada como camino del barrido y el barrido se creará alrededor de toda la cubierta.

_**Nota:**_ _Si tiene problemas para seleccionar una de las caras, utilice la herramienta_ _**Orbitar \(O\)**_ _para ver la cara un poco mejor y vuelva a intentarlo. Como opción alternativa, seleccione todos los bordes de la cubierta en lugar de la cara superior de la cubierta para completar el barrido._

![](../../.gitbook/assets/11%20%282%29.png)

4 - Mantenga el modelo organizado mediante la creación de un grupo **Roof - Cornice**, la adición a la capa **Roof** y la asignación del material **Metal – Brushed – Colorized** a él.

![](../../.gitbook/assets/12%20%281%29.png)

5 - Para terminar, active la capa **Column** y verá que el barrido recién creado se interseca con la parte superior de los pilares. Resuelva esto mediante la edición de cualquiera de los grupos **Column Tall** y arrastrando la cara superior hacia abajo hasta que se alinee con la parte superior de la cornisa.

![](../../.gitbook/assets/13%20%285%29.png)

