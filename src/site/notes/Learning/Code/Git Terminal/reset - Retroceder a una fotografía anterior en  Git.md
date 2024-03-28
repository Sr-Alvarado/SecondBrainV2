---
{"dg-publish":true,"permalink":"/learning/code/git-terminal/reset-retroceder-a-una-fotografia-anterior-en-git/","created":"2024-03-27T16:18","updated":"2024-03-27T19:37"}
---

[^1]: En realidad este comando tiene trampa, en Git siempre se guardan los cambios y si quieres volver a una fotografía específica solo tienes que usar su [[Learning/Wiki/Hash\|hash]].

Si quieres seguir el desarrollo de tu proyecto desde una fotografía anterior ejecuta:
```shell
git reset
```
- `reset`. Retrocede una fotografía. Modifica el proyecto o fichero dejándolo tal como estaba en la penúltima fotografía. Por defecto los archivos y modificaciones posteriores se guardan pero no se muestran además todos los próximos cambios se harán desde esta fotografía.

Si lo que quieres es no guardar los cambios y resetear todo tu proyecto a un estado anterior puedes usar:
```shell
git reset --hard
```
- `--hard`. Propiedad de `reset` que permite "eliminar"[^1] todos los cambios posteriores.
