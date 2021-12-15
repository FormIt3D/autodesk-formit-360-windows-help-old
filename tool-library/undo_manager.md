# Administrador de deshacer

FormIt presenta un sistema exclusivo de Deshacer/Rehacer, que se puede utilizar de dos formas diferentes para deshacer por grupo o de forma cronológica y global, como se indica a continuación:

* Las acciones Deshacer/Rehacer al editar un grupo anidado solo afectarán a los cambios dentro de ese grupo.
   * Esto significa que puede realizar un cambio en este grupo, realizar muchos cambios en otros grupos, volver al grupo original y tener la opción de deshacer el último cambio realizado en este grupo sin que ello afecte a los cambios realizados más recientemente en cualquier otro lugar.
* El comportamiento de Deshacer/Rehacer desde el boceto principal \(no mientras se edita un grupo\) es igual al de los sistemas tradicionales; se deshará el último cambio realizado en **cualquier** grupo según el orden cronológico.

El Administrador de deshacer registra todos los cambios realizados en cada grupo del modelo de FormIt, incluidos los cambios realizados en el boceto principal. Esto resulta útil para conocer visualmente las operaciones que se han deshecho en cualquier grupo del modelo.

![](../.gitbook/assets/undo-manager.png)

El Administrador de deshacer indicará en **negrita** el estado actual, las operaciones anteriores a este estado y las operaciones que existían, pero que se han deshecho desde entonces.

Puede hacer clic con el botón derecho en un estado y seleccionar Pasar a para deshacer o rehacer de forma eficaz según sea necesario a fin de volver a ese estado del modelo.

Los grupos que se han suprimido explícitamente o que ya no existen debido a una acción Deshacer o Rehacer se muestran como \*Inactivo\*. Se pueden restablecer mediante la acción Deshacer o Rehacer dentro de su grupo principal hasta que vuelvan a existir.

