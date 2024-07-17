---
{"dg-publish":true,"dg-path":"Code/Git/gitignore - Indicar a Git que ignore un archivo.md","permalink":"/code/git/gitignore-indicar-a-git-que-ignore-un-archivo/","created":"2024-03-27T16:18","updated":"2024-05-10T22:44"}
---

Si no quieres añadir algún archivo a los commits, y no quieres que [[Learning/Code/Git/Git\|Git]] te indique que no lo has añadido, puedes indicar que lo ignore añadiendo su ruta al fichero `.gitignore`. Si no lo tienes, primero créalo:
```shell
touch .gitignore
```
- `touch`. Comando de [[Learning/Wiki/Linux\|Linux]] que permite crear nuevos archivos.
- `.gitignore`. Fichero de Git que registra ficheros a ignorar.

Ya con el fichero creado, añade las rutas dentro:
```git
**/NOMBRE_FICHERO_A_IGNORAR
```
- `**/`. Indica que se buscará ficheros con ese nombre en la carpeta principal y en todas sus sub-carpetas.