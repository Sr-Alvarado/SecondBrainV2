---
{"dg-publish":true,"dg-path":"Dev/Git/rm --cached - Sacar archivos de la fotografía en Git.md","permalink":"/dev/git/rm-cached-sacar-archivos-de-la-fotografia-en-git/","created":"2024-08-14T12:35","updated":"2024-08-14T12:35"}
---

Esta función permite hacer lo contrario a [[Learning/Dev/Git/add - Añadir ficheros a la fotografía en Git\|git add]], en ves de agregar archivos al stage, permite eliminar esos archivos del stage.
```bash
git rm --cached <NOMBRE_DEL_ARCHIVO_A_ELIMINAR_DEL_STAGE>
```
- `rm`. Comando para eliminar archivos del repositorio.
- `--cached`. Flag que modifica a `rm`, en ves de eliminar los archivos solo deja de rastrearlos.