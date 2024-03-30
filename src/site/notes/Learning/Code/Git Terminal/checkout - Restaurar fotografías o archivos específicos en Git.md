---
{"dg-publish":true,"dg-path":"Code/Git Terminal/checkout - Restaurar fotografías o archivos específicos en Git.md","permalink":"/code/git-terminal/checkout-restaurar-fotografias-o-archivos-especificos-en-git/","created":"2024-03-27T16:18","updated":"2024-03-29T18:53"}
---


Si luego de hacer una fotografía, modificas el fichero y quieres volver a como estaba antes, puedes usar:
```shell
git checkout VALOR
```
- `chekout`. Devuelve los datos de como estaba un fichero o todo el proyecto en la última fotografía.
- `VALOR`. Admite ficheros o hash:
   - `NOMBRE_FICHERO`. Regresa un fichero específico al estado que tenía en la anterior fotografía.
   - `HASH_FOTOGRAFIA`. Regresa todo el proyecto al estado que tenía en una fotografía específica.