---
{"dg-publish":true,"dg-path":"Dev/Git/log - Mostrar el registro de fotografías del proyecto en Git.md","permalink":"/dev/git/log-mostrar-el-registro-de-fotografias-del-proyecto-en-git/","created":"2024-03-27T16:18","updated":"2024-03-29T18:52"}
---

Si quieres ver los cambios o fotografías de tu proyecto desde el inicio hasta la cabeza de tu proyecto o la versión más actual puedes usar: 
```shell
git log --graph --decorate --all --oneline
```
- `log`. Muestra el registro de commits hasta la cabeza del proyecto. Con el autor, email, [[Learning/Wiki/Hash\|hash]], comentario, fecha y rama que se modificó.
- `--graph`. Etiqueta de `log` que permite ver los commits de forma más gráfica.
- `--decorate`. Etiqueta de `log` que permite modificar el estilo del `log`.
- `--all`. Etiqueta de `log` que indica que se modificará todo el `log`.
- `--oneline`. Etiqueta de `log` que indica que se mostrará el resultado del `log` en una sola linea por commit.
