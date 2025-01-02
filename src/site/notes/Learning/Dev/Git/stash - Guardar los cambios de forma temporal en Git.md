---
{"dg-publish":true,"dg-path":"Dev/Git/stash - Guardar los cambios de forma temporal en Git.md","permalink":"/dev/git/stash-guardar-los-cambios-de-forma-temporal-en-git/","created":"2024-03-29T18:21","updated":"2024-03-29T18:21"}
---

Si tienes que suspender tu trabajo en el proyecto pero no has terminado lo que querías hacer como para hacer un [[Learning/Dev/Git/commit - Hacer una fotografía en Git\|commit]] puedes usar:
```bash
git stash
```
- `stash`. Comando de Git que guarda los cambios de una [[Learning/Wiki/Rama\|rama]], pero no crea una nueva fotografía, solo los almacena de forma temporal.

Para ver si tienes cambios temporalmente puedes usar:
```bash
git stash list
```
- `list`. Propiedad de `stash` que lista todos los cambios guardados temporalmente del proyecto.