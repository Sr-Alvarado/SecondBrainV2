---
{"dg-publish":true,"permalink":"/learning/dev/git/merge-fusionar-la-rama-actual-con-otra-rama-en-git/","created":"2024-03-27T20:22","updated":"2024-03-29T18:40"}
---

Si deseas traerte los cambios de otra rama a tu rama puedes usar:
```bash
git merge NOMBRE_RAMA_PRINCIPAL
```
- `merge`. Combina los cambios de 2 ramas. Debes estar en la rama a que quieres traerte los cambios.

## ¿Qué pasa si hay conflictos?

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/dev/git/resolver-conflictos-en-git/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




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

</div></div>
