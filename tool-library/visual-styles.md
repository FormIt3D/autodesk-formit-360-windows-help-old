# Estilos visuales

Personalice el aspecto visual del modelo, incluidos los estilos de borde, la iluminación general y los efectos ambientales. Para acceder al panel Estilos visuales, haga clic en el icono de gafas de sol de la barra de paletas, como se indica a continuación:

![](../.gitbook/assets/20200307-visual-styles-icon.png)

Los estilos visuales [se pueden establecer por escena ](https://windows.help.formit.autodesk.com/building-the-farnsworth-house/visual-settings), lo que le permite guardar sus parámetros de estilo favoritos y aplicarlos a otras escenas.

## Superficies

Administre la forma en que se muestran y se sombrean las superficies.

![](../.gitbook/assets/visual_styles%20%281%29.png)

La opción **Brillo ambiental** controla el brillo general de todos los materiales de la escena. El valor 100 indica que los materiales expuestos a la luz se mostrarán con el brillo completo definido en el color o la textura del material. Los valores superiores a 100 sobreexpondrán los materiales, pero pueden ser útiles para los modelos de SketchUp que aún aparecen oscuros en FormIt. El valor por defecto es 100.

La opción **Contraste ambiental** controla el grado de oscuridad de las caras en la sombra en comparación con las caras expuestas a la luz solar directa. El valor 0 indica que la iluminación no tiene ningún efecto \(todos los materiales aparecerán con su brillo completo, independientemente de la orientación\), mientras que los valores más altos harán que las caras sombreadas parezcan cada vez más oscuras. El valor por defecto es 25.

Active o desactive **Sombras** para ver cómo el diseño [se sombrea a la hora actual del día](https://windows.help.formit.autodesk.com/tool-library/shadows).

La opción **Intensidad de sombra** controla el modo en que se dibujan las sombras oscuras en el plano base y en otras caras. El valor 0 hará que las sombras sean realmente invisibles, y el valor 100 hará que las sombras sean negras. El valor por defecto es 20.

La opción **Sombras ambientales** agrega un toque de sombreado a las esquinas para añadir realismo al modelo de FormIt.

La opción **Superficies de un solo tono** desactiva el color y la textura de todos los materiales y hace que el entorno circundante sea blanco. Esta opción es útil para estudios de sombras o sombreado.

La sección Colores de superficie permite definir los colores por defecto para las caras cuando no se aplica ningún material.

La opción **Caras** hace referencia al color por defecto de todas las caras frontales de FormIt \(o de ambos lados, si la opción Caras posteriores está desactivada\) cuando no se aplica ningún material.

La opción **Caras posteriores** se utiliza para mostrar diferentes materiales a cada lado de una sola cara para los modelos de SketchUp que se importan en FormIt y requieren esta función. Esta opción está desactivada por defecto, pero está activada cuando se abren o se importan modelos de SketchUp. En una geometría que no sea de SketchUp, el color de cara posterior especificado se mostrará en los lados posteriores de las caras.

Utilice las secciones Efectos de corte de sección y Efectos poché de sección para administrar los colores por defecto de las caras, las líneas y el efecto poché cuando se utiliza la herramienta [Plano de sección](section-planes.md).

## Planos de suelo

Si la opción Plano de suelo está desactivada en el modo de edición de grupo, la rejilla azul del plano de suelo también está desactivada.

El color del plano de trabajo también se puede personalizar en el panel Estilos visuales.

![](../.gitbook/assets/screen-shot-2020-03-30-at-1.30.16-pm.png)

## Bordes

Administre el estilo de visualización de todos los bordes del modelo.

![](../.gitbook/assets/edges.PNG)

La opción **Contraste** afecta a la visibilidad de todos los bordes. El valor 0 permitirá que los bordes sean realmente invisibles. El valor por defecto es 60.

La opción **Color** afecta al color de todos los bordes del modelo. El color por defecto es el negro.

La opción **Bordes gruesos** aumenta el grosor de todos los bordes, incluidos los de silueta.

La opción **Bordes de boceto** añade un efecto de boceto a todos los bordes para simular un efecto de dibujo a mano.

La opción **Bordes ocultos** muestra los bordes que de otro modo quedarían ocultos por las superficies.

La opción **Bordes extendidos** añade una extensión a algunos bordes para simular un efecto de dibujo a mano.

## Entorno

Active o desactive la visualización de los efectos ambientales y los objetos auxiliares.

![](../.gitbook/assets/environment.PNG)

La opción **Rejilla** controla la visualización de la rejilla en el plano de suelo, así como la rejilla mostrada al editar un grupo. La opción Forzar cursos a rejilla se desactivará cuando la rejilla esté desactivada.

La opción **Ejes** controla la visualización de los ejes XYZ que se muestran en el origen universal o en el origen del grupo si se está modificando un grupo.

La opción **Niveles** controla la visualización de los [**niveles**](levels-and-area.md) establecidos en el panel Niveles.

La opción **Niebla** controla la visualización de la niebla que se dibuja para que la transición entre el plano de suelo y el cielo parezca perfecta. Si desactiva esta opción, se creará una línea de horizonte duro en la ubicación en la que el plano de suelo \(si está activado\) se encuentra con el cielo.

La opción **Flecha de norte** controla la visualización de un pequeño widget gráfico que indica la dirección del norte del proyecto \(según lo determine la ubicación y las imágenes de satélite\).

Los colores ambientales como el cielo, el fondo y el plano de suelo también se pueden personalizar.

El cielo está formado por un degradado de los colores **Inferior / fondo**, **Medio** y **Superior**.

Si la opción **Cielo** está desactivada, solo estará visible el color **Inferior / fondo**.

## Diagnóstico

Active o desactive la visualización de las herramientas de diagnóstico.

![](../.gitbook/assets/diagnostics.PNG)

La opción **Problemas de hermeticidad** resalta en rojo todos los bordes que no formen parte de un objeto sólido hermético.

La opción **Caras posteriores** resalta en rojo todas las caras que están orientadas de forma incorrecta \(las caras posteriores de todos los objetos sólidos deben estar orientadas hacia el interior de la forma sólida\).

[Obtenga más información sobre el uso de los diagnósticos de caras posteriores y hermeticidad para identificar y solucionar problemas con los modelos sólidos](https://formit.autodesk.com/blog/post/repairing-solid-models).

