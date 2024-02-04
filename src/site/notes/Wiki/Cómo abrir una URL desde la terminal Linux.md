---
{"dg-publish":true,"dg-path":"Abrir una URL desde la terminal.md","permalink":"/abrir-una-url-desde-la-terminal/","tags":["#linux","#terminal","bash","Web"],"created":"2024-01-25T19:06","updated":"2024-01-22T14:22"}
---

## Como siempre... Vamos de frente a lo bueno
Existen varios comandos para abrir un enlace web desde la terminal en Linux, sin embargo mi favorito es:
```bash
NOMBRE_NAVEGADOR URL_COMPLETO
```
Este comando funciona llamando al navegador en el que queramos abrir el enlace (`firefox`, `google-chrome`, `brave-browser`,`vivaldi`, etc.) y luego colocando la URL completa, incluyendo `https://`, de la página a la que nos queremos dirigir. 

Este es mi comando favorito porque nos permite escoger el navegador en ves de usar el predeterminado, ademas de dejarnos seguir usando la terminal luego de ejecutar el comando. Postdata: otros comandos se mantienen ejecutando en tanto estés dentro de la pág web.
## Otros comandos
### `x-www-browser URL_COMPLETO`
Al igual que el comando anterior se ejecuta y te permite seguir usando la terminal aún que este abre el enlace en el navegador predeterminado, ademas, este comando no está oficialmente en el manual de Linux.
### `xdg-open URL_COMPLETO`
Este comando abre el enlace en el navegador predeterminado y se mantiene en ejecución en tanto tengas la página abierta.