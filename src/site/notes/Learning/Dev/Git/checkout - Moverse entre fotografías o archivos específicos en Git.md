---
{"dg-publish":true,"permalink":"/learning/dev/git/checkout-moverse-entre-fotografias-o-archivos-especificos-en-git/","created":"2024-03-27T16:18","updated":"2024-04-02T17:14"}
---


Si quieres moverte a una rama o [[Learning/Dev/Git/commit - Hacer una fotografía en Git\|commit]] anterior puedes usar:
```shell
git checkout VALOR
```
- `chekout`. Devuelve los datos de como estaba un fichero o todo el proyecto en la última fotografía.
- `VALOR`. Admite ficheros o hash:
   - `NOMBRE_FICHERO`. Regresa un fichero específico al estado que tenía en la anterior fotografía.
   - `HASH_FOTOGRAFIA`. Regresa todo el proyecto al estado que tenía en una fotografía específica.