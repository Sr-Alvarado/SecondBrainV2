---
{"dg-publish":true,"permalink":"/learning/dev/git/add-anadir-ficheros-a-la-fotografia-en-git/","created":"2024-03-27T16:18","updated":"2025-01-03T19:00"}
---

Si quieres añadir ficheros al [[Learning/Dev/Git/stash - Guardar los cambios de forma temporal en Git\|stash]] (lista de archivos que serán [[Learning/Dev/Git/commit - Hacer una fotografía en Git\|commit]]eados luego) puedes usar^[Para elimininar archivos del stage (unstage) puedes usar [[Learning/Dev/Git/rm --cached - Sacar archivos de la fotografía en Git\|rm --cached]]]: 
```shell
git add NOMBRE_FICHERO
```
- `add`. Propiedad de Git que permite seleccionar que ficheros se agregarán a la [[Learning/Wiki/Fotografía\|Fotografía]].