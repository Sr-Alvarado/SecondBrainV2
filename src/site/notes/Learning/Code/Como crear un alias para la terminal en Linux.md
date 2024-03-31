---
{"dg-publish":true,"dg-path":"Code/Como crear un alias para la terminal en Linux.md","permalink":"/code/como-crear-un-alias-para-la-terminal-en-linux/","tags":["linux","terminal","bash"],"created":"2024-01-27T22:11","updated":"2024-03-02T22:05"}
---

## Vamos directo a lo bueno
Para crear un alias usamos el comando `alias NOMBRE_ALIAS='COMANDO'`. Sin embargo el alias solo estará activo mientas está abierta esa terminal. Para guardarlo y usarlo cuando queramos ejecutamos:

```bash
echo "alias NOMBRE_ALIAS='COMANDO'" >> .bashrc
```
- **`echo`** devuelve el resultado de todo lo que está en comillas dobles (").
- **`>>`** informa al sistema que todo lo anterior debe ser enviado a la ubicación que esta a la derecha.
- **`.bashrc`** es una carpeta oculta[^1] donde el sistema guarda los comandos de terminal, aquí enviaremos el resultado del `echo`.

Si lo pruebas, **aún no funcionará**. Para que los cambios surtan efecto debes reiniciar la terminal, cerrando y volviendo a abrirla.

Listo! Ahora ya sabes como crear un alias reusable en la terminal.

[^1]: Las carpetas ocultas en [[Learning/Wiki/Linux\|Linux]] se identifican por tener un punto (.) al inicio del nombre.