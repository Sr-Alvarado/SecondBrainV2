---
{"dg-publish":true,"dg-path":"Code/reflog - Ver todos los cambios del proyecto en el tiempo en Git.md","permalink":"/code/reflog-ver-todos-los-cambios-del-proyecto-en-el-tiempo-en-git/","created":"2024-03-27T19:12","updated":"2024-03-27T19:12"}
---

Si retrocediste a una fotografía anterior con la propiedad `hard` o cambiaste el `HEAD` de tu proyecto y al ejecutar `log` solo te muestra los cambios anteriores a la fotografía actual, puedes usar:
```bash
git reflog
```
- `reflog`. Mostrará todos los cambios en el proyecto en el tiempo, permitiéndote acceder a fotografías "eliminadas". 