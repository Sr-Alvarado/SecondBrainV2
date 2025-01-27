---
{"dg-publish":true,"permalink":"/learning/dev/git/checkout-tags-moverse-entre-fotografias-usando-los-tags-en-git/","created":"2024-03-27T19:47","updated":"2024-03-27T20:17"}
---

Si quieres volver al estado de una fotografía anterior sin usar el hash de esa fotografía puedes usar su tag si tiene uno con:
```bash
git checkout tags/VALOR_DEL_TAG
```
- `tags/`. Propiedad de `checkout` que permite usar un tag en remplazo del hash.