---
{"dg-publish":true,"permalink":"/learning/code/git-terminal/moverse-a-una-fotografia-especifica-en-git/","created":"2024-03-27T16:18","updated":"2024-03-27T16:18"}
---

Para moverte a una fotografía específica solo debes copiar su [[Learning/Wiki/Hash\|hash]] como valor para el `checkout`.
```shell
git checkout HASH_DE_LA_FOTOGRAFIA_DESTINO
```
- **Info:** En algunos casos puede no funcionar, debido a que hay archivos que no han sido añadidos a la fotografía.