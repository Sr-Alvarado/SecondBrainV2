---
{"dg-publish":true,"dg-path":"Code/Git Terminal/merge - Traer la última actualización de la rama principal a una rama secundaria en Git.md","permalink":"/code/git-terminal/merge-traer-la-ultima-actualizacion-de-la-rama-principal-a-una-rama-secundaria-en-git/","created":"2024-03-27T20:22","updated":"2024-03-27T20:37"}
---

Si estas trabajando con una rama secundaria y la rama principal se actualiza, puedes actualizar tu rama con los últimos cambios de la rama principal con:
```bash
git merge NOMBRE_RAMA_PRINCIPAL
```
- `merge`. Combina los cambios de 2 ramas. Debes estar en la rama a que quieres traerte los cambios.

## ¿Qué pasa si hay conflictos?

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/learning/code/resolver-conflictos-en-git/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Si tienes conflictos y estas usando el editor de código [[vscode\|vscode]], en el mismo editor te aparecerán las lineas de código en conflicto. Lo único que tienes que hacer es:
- Modificar tu código borrando el código que has modificado y manteniendo el modificado por la rama principal.
- Guardar el archivo y añadirlo a los archivos a fotografiar con `add`.
- Hacer una nueva fotografía del proyecto.
- Y ahora si usar `merge` para actualizar tu rama a la última versión de la rama principal

</div></div>
