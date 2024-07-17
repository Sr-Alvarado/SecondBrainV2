---
{"dg-publish":true,"dg-path":"Code/Git/config alias - Crear alias en Git.md","permalink":"/code/git/config-alias-crear-alias-en-git/","created":"2024-03-27T16:18","updated":"2024-03-27T18:55"}
---

Git nos permite crear "alias" al mismo estilo de la terminal, solo debes añadir:
```shell
git config --global alias.ALIAS_NAME "YOUR_GIT_COMMAND"
```
- `alias.tree`. Propiedad de `config` que indica que se creará un alias en git.
- `.ALIAS_NAME`. Valor que tomará el nombre del alias.
- `"YOUR_GIT_COMMAND"`. El comando en git que se ejecutará cuando se llame a ese alias.

**Ejemplo:** `git config --global alias.tree "log --graph --decorate --all --oneline"`