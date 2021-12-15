# Módulos de extensión

Utilice el Plugin Manager para instalar módulos de extensión útiles del equipo de FormIt o aprenda a [**crear sus propios módulos de extensión de FormIt**](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html)**.**

#### Plugin Manager de FormIt

Plugin Manager de FormIt funciona como un centro para descubrir y administrar los módulos de extensión de FormIt.

Plugin Manager se carga automáticamente cuando se inicia FormIt, siempre que este tenga acceso a Internet.

Para acceder a Plugin Manager, haga clic en el icono de ficha ubicado a la derecha de la ventana de la aplicación:

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/PluginManagerTab.PNG)

#### Plugin Manager clasifica los distintos tipos de módulos de extensión:

* **Módulos de extensión instalados**
* **Módulos de extensión recomendados**
   * Módulos de extensión que el equipo de FormIt recomienda para expandir las funciones principales de FormIt y descubrir nuevos flujos de trabajo.
   * Los módulos de extensión desarrollados por la comunidad aparecerán aquí después de que los apruebe el equipo de FormIt. Se proporcionará más información sobre esto en el futuro.
* **Módulos de extensión públicos**
   * Módulos de extensión creados por la comunidad, pero que no ha revisado o aprobado el equipo de FormIt.

#### Plugin Manager se ha diseñado mediante una serie de interfaces extensibles y contraíbles, lo que facilita la administración de módulos de extensión y sus repositorios:

* **Administración de módulos de extensión:**
   * Haga clic en el nombre de un módulo de extensión para ver su descripción.
   * Active o desactive el conmutador para instalarlo o desinstalarlo.
      * El módulo aparecerá como una barra de herramientas en la parte superior de la aplicación, un panel en el lado derecho o un cuadro de diálogo en el centro, según el tipo de módulo.
* Si está [desarrollando su propio módulo de extensión](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html), puede añadir su dirección URL privada en el campo de la parte inferior y pulsar \(+\), como se muestra a continuación:

![Plugin Manager de FormIt](https://formit3d.github.io/FormItExamplePlugins/docs/images/addNew.png)

#### Funcionamiento de los módulos de extensión

* Los módulos de extensión están basados en la Web y disponibles en FormIt para Windows y FormIt para Web.
* Los módulos de extensión están formados por una serie de archivos y carpetas alojados en GitHub o en un servidor local cuando se crea uno propio.
* Los módulos de extensión externos \(aquellos no hospedados localmente\) requieren una conexión a Internet para cargarse inicialmente. Esto implica lo siguiente:
   * Los módulos de extensión externos no se cargarán si no se detecta conexión a Internet al iniciar FormIt.
   * Una vez cargados, algunos módulos de extensión externos pueden seguir trabajando en modo sin conexión en esa sesión, pero es posible que otros no funcionen hasta que se restablezca la conectividad.
   * Los módulos de extensión externos cargan el código más reciente del servidor en cada ejecución, por lo que sus funciones se actualizarán cada vez que el autor publique un cambio.
* Los módulos de extensión se cargan de forma asíncrona, lo que significa que su orden en la interfaz de FormIt puede cambiar en cada nueva sesión.
* Plugin Manager utiliza claves del Registro de Windows para almacenar los repositorios y los módulos instalados.
   * Si necesita restablecer Plugin Manager a sus valores por defecto, elimine la siguiente clave del Registro:
      * Computer\HKEY\_CURRENT\_USER\Software\Autodesk\FormIt 360\Plugins
      * Tenga en cuenta que esto desinstalará todos los repositorios y los módulos de extensión añadidos por el usuario, lo que restablecerá Plugin Manager para incluir solo los repositorios y los módulos de extensión integrados.

