---
{"dg-publish":true,"dg-path":"Code/Git/config pull - Configurar el tipo de modificación de ficheros con pull en Git.md","permalink":"/code/git/config-pull-configurar-el-tipo-de-modificacion-de-ficheros-con-pull-en-git/","created":"2024-04-03T21:33","updated":"2024-04-03T21:33"}
---

Hay varias opciones para esta configuración:

Lo más común y recomendado es usar un [[Learning/Code/Git/merge - Fusionar la rama actual con otra rama en Git\|merge]], para definir esta configuración puedes usar:
```bh
git config pull.rebase false
```
- `pull.rebase`. La opción de `rebase` es una operación que en vez de fusionar los cambios entre ramas mueve los [[Learning/Code/Git/commit - Hacer una fotografía en Git\|commit]]s de la rama secundaria directamente a la rama principal sin importar los conflictos. Si se desactiva se usa un [[Learning/Code/Git/merge - Fusionar la rama actual con otra rama en Git\|merge]] por defecto.