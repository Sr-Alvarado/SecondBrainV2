---
{"dg-publish":true,"permalink":"/learning/code/resolver-conflictos-en-git/","created":"2024-03-27T20:38","updated":"2024-03-27T20:38"}
---

Si tienes conflictos y estas usando el editor de código [[vscode\|vscode]], en el mismo editor te aparecerán las lineas de código en conflicto. Lo único que tienes que hacer es:
- Modificar tu código borrando el código que has modificado y manteniendo el modificado por la rama principal.
- Guardar el archivo y añadirlo a los archivos a fotografiar con `add`.
- Hacer una nueva fotografía del proyecto.
- Y ahora si usar `merge` para actualizar tu rama a la última versión de la rama principal