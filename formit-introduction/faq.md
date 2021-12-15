# Preguntas frecuentes

## Acerca de FormIt

**¿Qué son FormIt y FormIt Pro?**

FormIt es un entorno de modelado, visualización, análisis y cálculo en 3D para el diseño arquitectónico.

Funciones de FormIt:

* Un potente motor de modelado de sólidos con eficaces herramientas y flujos de trabajo optimizados para el diseño de edificios.
* Visualización ambiental mejorada para ilustrar las opciones de diseño, incluidos los estados del modelo guardados mediante escenas.
* Ubicación, imágenes de satélite y terreno 3D con Bing Maps.
* Materiales de la Biblioteca de materiales de Autodesk.
* Herramientas de organización de modelos y visibilidad, como grupos, capas y escenas.
* Herramientas de análisis, entre las que se incluyen las siguientes:
   * Validación de hermeticidad y caras posteriores para un diagnóstico y una reparación de modelos eficaces
   * Sol y sombras
   * Análisis solar
   * Análisis energético
* Integraciones de productos de Autodesk:
   * BIM 360 Docs
   * Insight \(Análisis energético\)
   * [Dynamo](https://formit.autodesk.com/page/formit-dynamo)
   * [Revit](https://formit.autodesk.com/page/formit-revit)
* Compatibilidad con formatos de archivo:
   * Abrir/importar
      * AXM, DWG, FBX, SAT, STL, OBJ, WSM, SketchUp, Image
   * Exportar
      * AXM, FBX, OBJ, STL, SAT, DAE, DXF

FormIt está disponible de forma gratuita en [iOS](https://itunes.apple.com/us/app/autodesk-formit-360/id575282599?mt=8) y [en el navegador](https://app.formit.autodesk.com/). Se requiere una suscripción a **FormIt Pro** para utilizar [FormIt para Windows](https://formit.autodesk.com/page/download), la versión más potente y con más funciones de FormIt. La suscripción a **FormIt Pro** también ofrece funciones adicionales en iOS y en la Web, como el análisis solar y energético. **FormIt Pro** se incluye en la [Autodesk AEC Collection](https://www.autodesk.es/collections/architecture-engineering-construction/overview).

**¿Qué ha ocurrido con FormIt para Android?**

En un esfuerzo por optimizar la oferta de productos FormIt, tuvimos que tomar la difícil decisión de dejar de usar la aplicación para Android. Si lo tiene instalado, seguirá ejecutándose, pero ya no estará disponible en la Play Store.

**¿Cómo se obtiene FormIt?**

Para ejecutar la versión para Windows, debe tener acceso a **FormIt Pro**, que forma parte de la suscripción a la [AEC Industry Collection](https://www.autodesk.es/collections/architecture-engineering-construction/overview). Por lo tanto, si su oficina tiene Revit, es muy probable que ya tenga acceso a FormIt. Puede [descargar FormIt para Windows directamente desde nuestro sitio web](https://formit.autodesk.com/page/download) o desde la aplicación de escritorio de Autodesk.

Además, la versión web se puede ejecutar directamente de forma gratuita desde nuestro sitio web: [http://formit.autodesk.com](http://formit.autodesk.com).

La versión para iOS se puede descargar gratis desde la App Store de Apple \(solo para iPad\).

**Si soy estudiante o profesor, ¿puedo obtener acceso a FormIt Pro sin coste alguno?**

Sí. Puede acceder a la suscripción a FormIt Pro a través del [portal de educación de Autodesk](https://www.autodesk.es/).

**¿Cómo puedo aprender a usar FormIt?**

El mejor punto de partida es el [aprendizaje FormIt Primer](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Building-the-Farnsworth-House.html).

Existen varias secciones de FormIt Primer, que van desde el nivel principiante \(creación de una casa moderna completa\) hasta el más avanzado \(trabajar con Revit y Dynamo de formas más avanzadas\).

También disponemos más de 20 videos en nuestra serie de seminarios web "FormIt Friday". Están disponibles en nuestro [canal de YouTube](https://www.youtube.com/playlist?list=PLqumTDi1CVHM7rCHJs83Yb2FyadmuQsiH).

## Trabajar con Revit

**¿Cómo funciona FormIt con Revit?**

FormIt es una aplicación de diseño y dibujo 3D independiente, pero crea datos que se pueden convertir fácilmente a Revit [mediante el complemento FormIt para Revit](https://formit.autodesk.com/page/formit-revit).

**¿Qué ocurre al importar en Revit?**

A partir de la versión 2016, Revit incluye un complemento para trabajar con datos de FormIt. Al importar un archivo AXM de FormIt en Revit, este complemento examina cada objeto del archivo y lo vuelve a crear en Revit mediante la API. Por defecto, todos los elementos de FormIt se consideran como masa.

El Conversor a FormIt utiliza cada objeto de masa y crea una familia de masas en Revit mediante la [API Direct Shape](https://knowledge.autodesk.com/search-result/caas/CloudHelp/cloudhelp/2016/ESP/Revit-API/files/GUID-DF7B9D4A-5A8A-4E39-8721-B7782CBD7730-htm.html).

Direct Shape es un objeto no editable que se utiliza en los flujos de trabajo de IFC. Aunque no se puede editar, tiene la ventaja de transferir texturas de materiales completas entre FormIt y Revit. [A continuación, se muestra un aprendizaje](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Revit-Interop.html) que explica con más detalle el flujo de trabajo de FormIt a Revit.

**¿Puede FormIt crear muros, suelos y otras familias de sistema de Revit?**

No directamente. Como se ha indicado anteriormente, cada objeto se establece por defecto en la categoría Masa. Para crear muros, suelos o elementos similares, debe importar el modelo en Revit mediante el complemento de conversor y utilizar las herramientas nativas de Revit para crear familias de sistema a partir del modelo de masa subyacente.

**¿Revit puede devolver datos a FormIt?**

Sí. Para volver a importar datos en FormIt, exporte todo o, preferiblemente, _parte_ del archivo de Revit al formato de archivo SAT. Normalmente, no es necesario enviar TODOS los datos de Revit a FormIt. En su lugar, cree una vista filtrada en Revit que solo incluya los datos mínimos \(por ejemplo, suelos y muros\) antes de guardarla en SAT.

## Trabajar con otras aplicaciones

**¿Por qué se utiliza el formato de archivo por defecto ".AXM"?**

Antes de que FormIt recibiera su nombre, su designación en clave interna era XModeler, por lo que el formato de archivo que creamos fue Autodesk X Modeler o AXM para abreviar.

**¿Qué tipo de formatos 3D puede importar FormIt? **

* Windows: AXM, DWG, FBX, OBJ, SAT, SKP, STL
* Web: OBJ, STL
* iOS: OBJ, STL, SAT

**¿Qué tipos de formatos se pueden exportar mediante FormIt?**

* Windows: FBX, OBJ, SAT, STL, DAE, DXF
* Web: OBJ, SAT, STL
* iOS: OBJ

**¿Cómo funciona FormIt con Dynamo?**

[Aprenda a trabajar de forma conjunta con FormIt y Dynamo](https://formit.autodesk.com/page/formit-dynamo) para crear flujos de trabajo de diseño computacional.

**¿Qué ventajas ofrece FormIt frente a SketchUp?**

* Mejor [**interoperabilidad con Revit**](../tool-library/revit.md) ****
* [**Integración de Dynamo**](../tool-library/dynamo.md) para el diseño computacional
* Herramientas nativas para el [**análisis solar**](../tool-library/solar-analysis.md) y el [**análisis energético con tecnología**](../tool-library/energy-analysis.md) de Autodesk Insight
* Un núcleo de modelado de sólidos más robusto que permite operaciones avanzadas de modelado
* Herramientas avanzadas de modelado nativas como [**Barrido, Recubrimiento, Solevación**](../tool-library/cover-sweep-loft.md), Desfase/Vaciar sólidos, Fusión/Empalme 3D y [**Aplanar caras**](../tool-library/flatten-face.md)
* Varios [**planos de sección visibles** ](../tool-library/section-planes.md)
* Herramientas de diagnóstico como [**Visualizar: Problemas de hermeticidad y Visualizar: Caras posteriores**](../tool-library/visual-styles.md)
* [**Exportar partes del modelo**](../tool-library/export-data.md) en función de lo que esté seleccionado o visible
* Exportación nativa de OBJ, SAT y STL

**¿Puedo utilizar los métodos abreviados de teclado de SketchUp?**

Sí. FormIt para Windows tiene un mapa de teclado completamente editable. Muchos métodos abreviados comunes de SketchUp ya están disponibles por defecto, pero puede editarlos en el menú Editar &gt; Preferencias.

**¿Puedo utilizar archivos DWG?**

Sí. FormIt importa archivos DWG 2D y 3D.

## Preguntas frecuentes sobre soporte

**¿Cómo puedo obtener soporte?**

Puede ponerse en contacto primero con su distribuidor de Autodesk o buscar información en el [foro de FormIt](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=es). Es recomendable que busque la pregunta primero y, si no se ha respondido, publique un nuevo tema para que el equipo de FormIt le responda.

**¿Qué debo hacer si no puedo iniciar sesión?**

* En esta [entrada del foro](https://forums.autodesk.com/t5/formit-forum/having-trouble-logging-into-formit-for-windows-try-these-steps/td-p/7179572?profile.language=es), se abordan los problemas habituales de inicio de sesión.
* Si tiene un PC con un procesador de gráficos intercambiable \(GPU\), es importante asegurarse de que FormIt siempre utilice la GPU de mayor rendimiento. A continuación, se indican las instrucciones para [AMD](https://community.amd.com/docs/DOC-1581#jive_content_id_Assigning_Applications_to_GPUs) y [NVIDIA](http://nvidia.custhelp.com/app/answers/detail/a_id/2615/kw/manage%203d%20settings/related/1).

**¿Qué debo hacer si el análisis energético de Insight presenta errores?**

Si el análisis energético de Insight informa de un error o no devuelve ningún resultado, [eche un vistazo a la página de análisis energético de Insight](https://formit.autodesk.com/page/formit-insight) para obtener consejos habituales para la resolución de problemas.

