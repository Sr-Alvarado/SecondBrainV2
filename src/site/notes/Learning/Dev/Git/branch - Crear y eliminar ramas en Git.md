---
{"dg-publish":true,"dg-path":"Dev/Git/branch - Crear y eliminar ramas en Git.md","permalink":"/dev/git/branch-crear-y-eliminar-ramas-en-git/","created":"2024-03-27T20:05","updated":"2024-04-05T14:28"}
---

Si quieres **añadir una rama nueva** para hacer modificaciones sin que afecten a la rama principal [[Learning/Wiki/Main\|main]] puedes usar:
```bash
git branch NOMBRE_RAMA
```
- `branch`. Propiedad de Git que indica que se modificarán las características de la rama. Si la rama no existe se creará copiando la fotografía principal de la rama anterior como base.

Si quieres **eliminar una rama** porque ya [[Learning/Dev/Git/merge - Fusionar la rama actual con otra rama en Git\|merge]]aste sus cambios o simplemente porque ya no te sirve, puedes usar:
```bash
git branch -d NOMBRE_RAMA
```
- `-d`. Etiqueta de `branch` que indica al sistema que quieres eliminar la rama.

> [!tip]
> En Git nada se elimina realmente, si revisas los [[Learning/Dev/Git/log - Mostrar el registro de fotografías del proyecto en Git\|log]]s y copias el [[Learning/Wiki/Hash\|hash]] de una rama eliminada, puedes acceder a ella con [[Learning/Dev/Git/checkout - Moverse entre fotografías o archivos específicos en Git\|chechout]]. 
> El trabajo de Git es guardar el registro de cambios. Las ramas eliminadas persisten en el tiempo y por eso puedes crear nuevas ramas desde cualquier fotografía del proyecto.
