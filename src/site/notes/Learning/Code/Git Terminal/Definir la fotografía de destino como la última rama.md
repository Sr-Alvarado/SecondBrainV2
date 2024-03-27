---
{"dg-publish":true,"permalink":"/learning/code/git-terminal/definir-la-fotografia-de-destino-como-la-ultima-rama/","created":"2024-03-27T16:18","updated":"2024-03-27T16:18"}
---

Si quieres que la rama a la que te moviste sea reconocido por git como la última rama (fotografía).
```shell
git checkout HEAD
```
- `HEAD`. Declara a la rama actual como la última fotografía. Aún se conservan las ramas siguiente pero el árbol ahora crecerá desde esta rama.