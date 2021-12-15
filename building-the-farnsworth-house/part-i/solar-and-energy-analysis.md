# Análisis solar y energético

Ahora que se ha creado el modelo, podemos utilizarlo para estudiar el **impacto solar y energético** de nuestro diseño. Estas funciones se integran en FormIt para que sus primeros estudios se puedan entender desde una perspectiva de rendimiento del edificio. Estas funciones son solo para **FormIt Pro**; si utiliza la aplicación web, es posible que no tenga acceso.

Si no ha completado la última sección, haga clic en Archivo &gt; Abrir y seleccione **farnsworth08.axm** en la carpeta de FormIt Primer.

## Sombras

Antes de poder utilizar cualquiera de estas herramientas de análisis, debe [establecer la ubicación](). Esto proporciona a FormIt acceso a datos exactos sobre el sol, las sombras y el clima.

1. Haga clic en el icono de sol en la [**barra de herramientas de acciones**](../../formit-introduction/tool-bars.md) y active **Sombras \(DS\)**.

   ![](../../.gitbook/assets/3bdf0e2a-0ad4-4aac-b6fc-5e789643b0d6.png)

2. Ajuste los controles deslizantes **Día** y **Hora** para ver cómo cambian las sombras.

   ![](../../.gitbook/assets/upperterracesketch_32.png)

3. Fíjese en que la terraza cubierta está a la sombra durante las horas más calurosas de los meses de verano; probablemente no sea accidental, sino una cuestión de diseño.

**Nota** Las sombras pueden provocar una reducción del rendimiento de la aplicación. Use estas dos sugerencias para mitigarlo esto: desactive las sombras si nota que la navegación se vuelve lenta o desactive capas como la de **mobiliario** si no son necesarias para estudiar las sombras.

## Análisis solar

Como personas visuales, los diseñadores pueden aprender y comunicar una increíble cantidad de información de diagramas de mapa térmico como el que estamos a punto de crear.

1. En la parte inferior del [**menú Sol**](../../formit-introduction/tool-bars.md), haga clic en el botón **Análisis solar**.
2. Se activa un modo especial en el que las **sombras**, los **métodos abreviados de teclas** y otras **barras de herramientas** están desactivadas.
3. El comportamiento de selección se modifica en el modo **Análisis solar**. Puede seleccionar **a través de grupos**, no es necesario mantener pulsada la tecla **Ctrl** o **Mayús** para añadir elementos al conjunto de selección y puede anular la selección de elementos haciendo clic de nuevo en ellos. Puede **hacer clic** o **doble clic** en la geometría, o bien realizar una **selección de ventana**.
4. Seleccione las caras que desea estudiar. **Haga clic una vez** en la parte superior de la **cubierta** y en la parte superior de las **plantas**. Evite seleccionar elementos pequeños como el mobiliario.

   ![](../../.gitbook/assets/upperterracesketch_33.png)

5. En la esquina superior izquierda del lienzo, busque la barra de herramientas **Análisis solar**. Haga clic en **Analizar**. FormIt calculará y renderizará las superficies. Esta configuración se puede ajustar antes **y** después de que se complete el análisis.

   ![](../../.gitbook/assets/solaranalysis.png)

6. El parámetro **Mes (máxima actividad)** muestra los valores **máximo** \(en BTU / pies cuadrados\) del mes especificado. Esta opción se ha diseñado para **estudios de sombreado**. Puede cambiar el mes y los gráficos se actualizarán al instante. **Coloque el cursor** sobre una superficie analizada para obtener un valor **específico**.

   ![](../../.gitbook/assets/460060a0-ea3b-4095-af45-40045811be22.png)

7. El parámetro **Año (acumulado)** presenta la energía **acumulada** de todo el año \(en KwH / m cuad.\). Esta opción se ha diseñado para **estudios de potencial fotovoltaico**.

   ![](../../.gitbook/assets/a9f61dfb-dfc9-4751-b145-b131a69c53cf.png)

8. Estos estudios de **análisis solar** se pueden exportar. Para ello, haga clic en **Archivo &gt; Exportar \(Ctrl + E\)** y seleccione **Imagen** en la lista de la izquierda.

## Análisis energético con Insight

FormIt ha integrado las mismas herramientas de análisis de rendimiento de construcción que utiliza Revit. **Insight** proporciona un un panel principal de los parámetros del sistema de construcción que se pueden ajustar para reflejar escenarios potenciales sin necesidad de **volver a analizar** la geometría del modelo. Insight funciona mejor con la geometría de **masa** de FormIt.

1. Asegúrese de que ha iniciado sesión en su cuenta de Autodesk Account. Desactive **todas** las capas, **excepto** la capa de **masa**. Se debe haber aplicado al menos un **nivel** a la geometría.
2. FormIt solo enviará geometría **visible** a Insight. Tenga en cuenta que incluso una **masa** simple generará un gran cantidad de datos de **Insight**

   ![](../../.gitbook/assets/energymassing.png)

3. Haga clic en el botón **Información &gt; Generar información**. El análisis se ejecutará en la nube, por lo que pueda seguir modelando durante el cálculo

   ![](../../.gitbook/assets/energymenu.png)

4. Una vez completado el análisis, haga clic en el botón **Ver información** para ver el **modelo energético** y los **factores de rendimiento** \(también puede visitar el sitio web directamente en [**http://insight.autodesk.com**](http://insight.autodesk.com/)\).

   ![](../../.gitbook/assets/energydashboard.png)

5. En el panel principal de Insight, puede definir un valor \(o un intervalo de valores\) para cada widget de **factor de rendimiento**. Para ello, haga clic en el factor y arrastre los puntos azules. El intervalo resulta útil si aún no conoce el sistema específico que utilizará el edificio.
6. Con cada cambio de un **factor**, se actualiza el valor medio de **intervalo de costes energéticos** \(medido en USD / m cuad. / año\). Puede comprobar el rendimiento del diseño con referencias como **Ashrae 90.1** y el desafío de **Architecture 2030**.
7. Si el diseño cambia considerablemente, puede volver a enviar la masa actualizada al mismo centro de controles. Si desea crear un **nuevo** centro de controles para el diseño actualizado, deberá utilizar primero la opción **Guardar como** en FormIt.
8. Si el análisis energético no se ha realizado correctamente, es posible que tenga problemas de hermeticidad basados en geometría \(DW\)**, estos se pueden revisar y corregir en FormIt**.
9. Desactive la capa de **masa** y vuelva a activar todas las demás capas.

