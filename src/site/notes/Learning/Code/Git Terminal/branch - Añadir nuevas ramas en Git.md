---
{"dg-publish":true,"dg-path":"Code/Git Terminal/branch - Añadir nuevas ramas en Git.md","permalink":"/code/git-terminal/branch-anadir-nuevas-ramas-en-git/","created":"2024-03-27T20:05","updated":"2024-03-27T20:05"}
---

Si quieres añadir una rama nueva para hacer modificaciones sin que afecten a la rama principal [[Learning/Wiki/Main\|main]] puedes usar:
```bash
git branch NOMBRE_RAMA
```
- `branch`. Propiedad de Git que indica que se modificarán las características de la rama. Si la rama no existe se creará copiando la fotografía principal de la rama anterior como base.
