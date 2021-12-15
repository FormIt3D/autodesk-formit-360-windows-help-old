# Guardado automático

A partir de la versión v17.3, FormIt para Windows incluye la función Guardado automático, que realiza una copia de seguridad del modelo de FormIt mientras trabaja. Este archivo de copia de seguridad se puede utilizar para recuperar datos si FormIt se cierra con cambios no guardados.

### Activación y desactivación de Guardado automático

Las opciones de configuración de la función Guardado automático se encuentran en Editar &gt; Preferencias &gt; Guardado automático.

![](../.gitbook/assets/20190613-autosave.png)

La función Guardado automático está activada por defecto, pero puede desactivarla por completo. Para ello, solo tiene que anular la selección de la casilla.

Establezca el intervalo \(en minutos\) en el que la función Guardado automático realizará una copia de seguridad. Para ello, especifique un valor en el cuadro de número Intervalo de guardado automático.

Tenga en cuenta que estas preferencias son de nivel de aplicación y no cambiarán al abrir archivos diferentes.

### Funcionamiento de Guardado automático

Cuando la función Guardado automático está activada, esta determina si el archivo de FormIt actual tiene cambios sin guardar. Si hay cambios sin guardar, la función Guardado automático crea una copia de seguridad del archivo en el intervalo especificado.

Los archivos de copia de seguridad se almacenan junto al archivo original y presentan la extensión `.axmb`.

Por ejemplo, si el archivo de FormIt original se almacena en `C:/Users/<user>/FormIt/MyProject.axm`, el archivo de copia de seguridad se encuentra en `C:/Users/<user>/FormIt/MyProject.axmb`.

Si inicia una nueva sesión de FormIt sin abrir un archivo existente, los cambios no guardados se encuentran en `C:/Users/<user>/Documents/Untitled.axmb`. Una vez que guarde el nuevo modelo en una ubicación diferente, la copia de seguridad comenzará a añadir cambios sin guardar junto a la nueva ubicación, como se ha indicado anteriormente.

Al guardar cambios en el archivo original, la función Guardado automático suprime el archivo de copia de seguridad ya que esta copia es ahora más antigua que el archivo original. Sin embargo, si se realizan posteriormente cambios en el archivo guardado, la función Guardado automático volverá a iniciar el proceso de copia de seguridad en el intervalo especificado.

Si el archivo de trabajo tiene cambios sin guardar y decide cerrar FormIt y descartar los cambios, se suprimirá la copia de seguridad de Guardado automático. Sin embargo, si se fuerza el cierre de FormIt, al apagar el equipo o debido a un bloqueo de la aplicación, el archivo de copia de seguridad de Guardado automático se conservará y se podrá utilizar más adelante para recuperar los datos.

### Trabajar con la función Guardado automático activada

FormIt minimiza los posibles efectos en el rendimiento de la función Guardado automático al ejecutar la copia de seguridad en un proceso independiente. En archivos de tamaño pequeño a mediano, no se debería notar el proceso de copia de seguridad de la función Guardado automático. En archivos muy grandes \(~400 MB y superiores\), es posible que observe una pausa momentánea mientras FormIt copia todo el modelo y comienza a realizar una copia de seguridad en un proceso independiente.

Si se pregunta si se está realizando una copia de seguridad de Guardado automático, puede consultar la barra de estado en la parte inferior izquierda de la aplicación para ver si aparece el mensaje corto "Guardando automáticamente...":

![](../.gitbook/assets/20190613-autosave-status-bar.png)

Si la barra de estado está desactivada, puede activarla en la barra de estado de Windows &gt; o mediante el método abreviado HS.

### Recuperación de datos con Guardado automático

Al abrir un archivo de FormIt con una copia de seguridad disponible, FormIt le avisará de que el archivo de copia de seguridad existe. Como se ha indicado anteriormente, esto puede deberse simplemente a que cerró FormIt sin optar por guardar los cambios realizados en este proyecto la última vez que se modificó o a que FormIt se cerró de forma inesperada.

![](../.gitbook/assets/20190613-autosave-notification.png)

Al hacer clic en el hipervínculo "¿Desea abrirla?", se cargará el archivo de copia de seguridad `.axmb`.

De forma similar, puede utilizar &Archivo gt; Abrir y seleccionar manualmente el archivo `.axmb` en el explorador de archivos para abrir una copia de seguridad.

Una vez abierto el archivo de copia de seguridad, la próxima vez que guarde, FormIt le pedirá que seleccione un archivo de FormIt \(`.axm`\) diferente para sobrescribirlo. No se pueden sobrescribir los archivos de copia de seguridad de FormIt \(`.axmb`\).



