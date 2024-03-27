---
{"dg-publish":true,"permalink":"/learning/code/git-terminal/configurar-git/","created":"2024-03-27T16:18","updated":"2024-03-27T16:18"}
---

Toda configuración de Git se registra en el [[fichero\|fichero]] `.gitconfig`. Podrías añadir o modificar cualquier configuración directamente editando este fichero.

Cualquier configuración en Git sigue esta estructura:
```shell
git config --global
```
- `git`. Declara que se usará el programa Git.
- `config`. Declara que se usará el [[comando\|comando]] `config` del programa Git.
- `--global`. Es una [[etiqueta\|etiqueta]] del comando `config` que indica a que nivel se harán los cambios. En este caso los cambios afectarán a todos los usuarios del equipo.