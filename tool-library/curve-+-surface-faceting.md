# Facetado de curva + superficie

FormIt es un sistema de modelado poliédrico, por lo que objetos como círculos, arcos y splines se representan mediante una serie de bordes rectos. De forma similar, una superficie curva como la pared de un cilindro o una cúpula se compone de una serie de caras planas con aristas de borde ocultas.

Por defecto, FormIt utiliza 40 bordes o facetas para representar un círculo y 24 facetas para representar un objeto curvo 3D como un cilindro. Para superficies más complejas como una cúpula, un valor de 24 establece el recuento de facetas del perímetro y también afecta a la densidad del facetado del resto de la forma.

En FormIt para Windows v18 y versiones posteriores, los valores de facetado de curvas y superficies se pueden personalizar, como se muestra a continuación:

![](../.gitbook/assets/faceting\_planter.gif)

![](<../.gitbook/assets/faceting (1).png>)

**Calidad de facetado de curva**

El cambio de la calidad de facetado de curva afectará al número de facetas que se utilizan al dibujar nuevos círculos y arcos en FormIt, así como al colocar formas primitivas. Por ejemplo, si se establece en 64, se creará un círculo completo de 64 lados o un arco de cuarto de círculo con 16 facetas.

Este valor también afectará a la calidad de los círculos y los arcos importados de archivos SAT, así como al crear geometría desde Dynamo. Puede definir este valor para los bocetos nuevos o solo para el actual.

Para las curvas existentes, también puede utilizar el módulo de extensión Regenerar curva para regenerar de forma retroactiva un arco o un círculo **existentes** con un nuevo recuento de facetas, como se muestra a continuación:

![](../.gitbook/assets/screen-shot-2020-01-10-at-1.20.53-pm.png)

![](../.gitbook/assets/faceting\_rebuild-curve.gif)

**Calidad de facetado de superficie**

El cambio de este parámetro global afectará a la calidad de las superficies curvas 3D importadas desde archivos SAT y cuando se crean desde Dynamo.

Por ejemplo, si se establece en 64 y, a continuación, se crea una esfera desde Dynamo, se utilizarán 64 caras alrededor del ecuador de la esfera, más 64 facetas en cada uno de los círculos que van a los polos de la esfera, por lo que el recuento aumenta rápidamente. Utilice valores más altos con precaución, ya que puede afectar al rendimiento de FormIt en algunos casos. Una vez que haya obtenido un resultado de alta calidad, puede [convertirlo en una malla](meshes.md) para mejorar el rendimiento.

Al trabajar con Dynamo, puede modificar la calidad de facetado y pulsar Ejecutar gráfico en el panel Propiedades sin cambiar ningún parámetro para aprovechar los nuevos recuentos de facetas, como se muestra a continuación:

![](../.gitbook/assets/faceting\_column.gif)

Al igual que con las curvas, puede definir la calidad de facetado de la superficie para los nuevos bocetos o solo para el actual.

Tenga en cuenta que los valores de facetado están limitados actualmente a múltiplos de 4, por lo que, al introducir números manualmente, FormIt redondeará al múltiplo más cercano. Puede utilizar los controles deslizantes y las flechas para recorrer cíclicamente los valores aceptados.

![](../.gitbook/assets/units-+-precision.png)
