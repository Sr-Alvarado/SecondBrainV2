---
{"dg-publish":true,"permalink":"/learning/dev/git/diff-ver-diferencias-entre-un-commit-y-ahora-en-git/","created":"2024-03-27T16:18","updated":"2024-03-29T18:37"}
---


Si modificas tu proyecto pero no estás seguro de hacer una fotografía y quieres ver que parte del código cambiaste con respecto a la última fotografía puedes usar:
```shell
git diff
```
- `diff`. Propiedad de Git que devuelve los cambios en el código realizados entre la última fotografía y el momento actual. Devuelve: Nombre del archivo modificado, indica si se agregó o se eliminó algo, se especifica el número de lineas afectadas, y se imprime el antes y el después.

Si quieres comprar entre [[Learning/Wiki/Rama\|rama]]s puedes usar:
```bash
git diff NOMBRE_RAMA_A_COMPARAR
```
