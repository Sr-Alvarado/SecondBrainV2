---
{"dg-publish":true,"dg-path":"Code/Como generar una clave aleatoria en la terminal.md","permalink":"/code/como-generar-una-clave-aleatoria-en-la-terminal/","created":"2024-04-01T18:47","updated":"2024-04-01T18:48"}
---

Generar un [[Learning/Wiki/Hash\|hash]], o cadena de [[strings\|strings]], aleatorio en la terminal [[Learning/Wiki/Linux\|Linux]] es fácil con:
```shell
openssl rand -hex 32
```
- `32` Es el número de caracteres el [[Learning/Wiki/Hash\|hash]] a crear.