---
{"dg-publish":true,"dg-path":"Code/Git/checkout HEAD - Definir la fotografía como la cabeza del proyecto en Git.md","permalink":"/code/git/checkout-head-definir-la-fotografia-como-la-cabeza-del-proyecto-en-git/","created":"2024-03-27T16:18","updated":"2024-03-27T20:01"}
---

Si quieres que la fotografía a la que te moviste sea reconocida por git como la cabeza del proyecto usa:
```shell
git checkout HEAD
```
- `HEAD`. Declara a la fotografía actual como la última. Aún se conservan las fotografías siguientes pero la rama ahora crecerá desde esta fotografía.