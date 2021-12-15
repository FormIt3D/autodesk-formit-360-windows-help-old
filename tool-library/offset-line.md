# Línea de desfase

Dibuje líneas paralelas o de desfase mediante la herramienta Línea de desfase. Esto resulta útil para crear formas 2D que posteriormente se pueden extruir para que tengan un aspecto similar al de los muros 3D.

![](../.gitbook/assets/image%20%283%29.png)

La herramienta **Línea de desfase** funciona como la [**Línea** ](https://windows.help.formit.autodesk.com/tool-library/line-tool):

* Haga clic para definir el primer punto y, a continuación, mueva el cursor y coloque los puntos posteriores, ajustando la geometría existente o los ejes de inferencia.
* Se muestra una vista preliminar de la forma resultante. Los puntos segundo y tercero determinan el plano que seguirán los demás puntos, por lo que el resultado es plano.
* Continúe añadiendo puntos y pulse **Esc** o haga doble clic para finalizar la herramienta.
* Las autointersecciones se limpiarán y se fusionarán, dejando una cara extruible.

![Después de colocar dos puntos y arrastrar el tercer punto](../.gitbook/assets/walls1.png)

La línea de entrada se dibuja en rojo y, por defecto, se coloca en el centro de las líneas de desfase.

Puede cambiar la alineación de las líneas de desfase y su grosor. Para ello, pulse la tecla **Tab**. Se abre el cuadro de diálogo de **Opciones de herramientas**:

![Opciones de la herramienta Línea de desfase](../.gitbook/assets/walls2.png)

Por ejemplo, cambie la **Alineación** a **Izquierda** y el **Grosor** a 6"; las líneas de desfase se dibujarán a la izquierda de las líneas de entrada a 6 pulgadas de distancia.

![](../.gitbook/assets/walls3.png)

## Consejos útiles

Puede dibujar una forma cerrada forzando el cursor al primer punto colocado. La esquina resultante se limpiará automáticamente, como se muestra a continuación:

![](../.gitbook/assets/walls4.png)

Puede dibujar de forma libre las líneas de entrada unas encima de otras. Una vez finalizada la herramienta, se limpian las intersecciones resultantes.

![](../.gitbook/assets/walls5.png)

![](../.gitbook/assets/walls6.png)

Por lo tanto, la herramienta Línea de desfase debe generar geometría en un plano, por lo que los primeros puntos determinarán el plano que seguirán los puntos restantes.

Por ejemplo, inicie el dibujo en un lado de un cubo para usar el plano de esa cara. Después de colocar tres puntos no colineales, el plano de entrada se fija para el resto de la entrada. Tenga en cuenta que, al dibujar en una cara, la forma resultante se inserta en la cara, dividiéndola en varias caras. Para evitar la inserción, la cara en la que dibuje deberá formar parte de un [grupo](https://windows.help.formit.autodesk.com/tool-library/groups).

![Dibujo en una cara vertical](../.gitbook/assets/walls7.png)

![Una vez finalizada la herramienta, se insertan las líneas y las caras divididas se pueden manipular de forma adicional.](../.gitbook/assets/walls8.png)

También puede utilizar la herramienta Línea de desfase para trazar desde un dibujo de plano. Importe el plano como una imagen.

* Cambie el tamaño de la imagen para que el plano tenga la escala correcta. Esto se describe con más detalle [aquí](https://windows.help.formit.autodesk.com/building-the-farnsworth-house/work-with-images-and-the-ground-plane). 
* Puede utilizar la [Cámara ortogonal](orthographic-camera.md) para trazar en una [vista superior](orthographic-views.md) ortogonal.

![](../.gitbook/assets/walls9.png)

![](../.gitbook/assets/walls10.png)



