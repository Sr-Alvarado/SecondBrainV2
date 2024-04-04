---
{"dg-publish":true,"dg-path":"Code/Git Terminal/push -u origin - Asociar una rama remota con una rama local en Git.md","permalink":"/code/git-terminal/push-u-origin-asociar-una-rama-remota-con-una-rama-local-en-git/","created":"2024-04-03T21:01","updated":"2024-04-03T21:13"}
---

Si quieres definir a que rama de tu repositorio remoto se envirarán los cambios puedes usar:
```sh
git push -u origin NOMBRE_RAMA_REMOTA
```
- `push`. Comando de Git que permite modificar un repositorio remoto desde nuestro repositorio local.
- `-u`. Opción de `push` que indica que se asociará la rama local actual con una rama remota. Permite que en futuros `git push` se modificará la rama que se está definiendo.