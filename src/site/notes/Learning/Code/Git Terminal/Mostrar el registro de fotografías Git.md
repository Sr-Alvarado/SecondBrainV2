---
{"dg-publish":true,"permalink":"/learning/code/git-terminal/mostrar-el-registro-de-fotografias-git/","created":"2024-03-27T16:18","updated":"2024-03-27T16:18"}
---

```shell
git log --graph --decorate --all --oneline
```
- `log`. Muestra el registro de commits. Con el autor, email, [[Learning/Wiki/Hash\|hash]], comentario, fecha y rama que se modificó.
- `--graph`. Etiqueta de `log` que permite ver los commits de forma más gráfica.
- `--decorate`. Etiqueta de `log` que permite modificar el estilo del `log`.
- `--all`. Etiqueta de `log` que indica que se modificará todo el `log`.
- `--oneline`. Etiqueta de `log` que indica que se mostrará el resultado del `log` en una sola linea por commit.