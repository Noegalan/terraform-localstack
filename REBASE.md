## Comando Rebase

En esta tarea el objetivo ha sido limpiar el historial de commits del repositorio, ya que se habían creado dos commits con mensajes poco claros (`cosas` y `cambios`).

Para ello se ha utilizado el comando `git rebase -i HEAD~2`, que permite volver a los dos últimos commits y modificarlos desde una pantalla interactiva.

En este caso se ha usado la opción `reword` para cambiar el mensaje del primer commit y la opción `squash` para fusionar el segundo commit con el primero.

Después de guardar los cambios, Git abre una segunda ventana donde se puede escribir un nuevo mensaje más claro para el commit resultante. En este caso el mensaje final ha sido:

`Añade archivos de prueba para práctica de rebase`

Una vez completado el rebase, se ha utilizado el comando `git push --force` para actualizar también el repositorio remoto en GitHub y dejar el historial limpio tanto en local como en remoto.
