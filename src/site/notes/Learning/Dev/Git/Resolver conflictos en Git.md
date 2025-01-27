---
{"dg-publish":true,"permalink":"/learning/dev/git/resolver-conflictos-en-git/","created":"2024-03-27T20:38","updated":"2024-04-10T16:40"}
---

## En local
Si tienes conflictos y estas usando el editor de código [[vscode\|vscode]], en el mismo editor te aparecerán las lineas de código en conflicto. Lo único que tienes que hacer es:
- Modificar tu código borrando el código que has modificado y manteniendo el modificado por la rama principal.
- Guardar el archivo y añadirlo a los archivos a fotografiar con `add`.
- Hacer una nueva fotografía del proyecto.
- Y ahora si usar `merge` para actualizar tu rama a la última versión de la rama principal

## En GitHub
Si tienes conflictos de [[pull request\|pull request]] porque el repo de origen está des-actualizado puedes usar:
- Ir a la parte de conflicto de la [[pull request\|pr]] 
- Editar directamente en [[Learning/Dev/GitHub/GitHub\|GitHub]] con su editor integrado
- Marcar como resuelto y [[Learning/Dev/Git/commit - Hacer una fotografía en Git\|commit]]ear el archivo editado
- Ahora si ya puedes [[Learning/Dev/Git/merge - Fusionar la rama actual con otra rama en Git\|merge]]ar la [[pull request\|pr]] 