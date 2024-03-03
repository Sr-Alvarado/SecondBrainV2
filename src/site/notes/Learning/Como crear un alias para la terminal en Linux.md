---
{"dg-publish":true,"dg-path":"Como crear un alias para la terminal en Linux.md","permalink":"/como-crear-un-alias-para-la-terminal-en-linux/","tags":["linux","terminal","bash"],"created":"2024-01-27T22:11","updated":"2024-03-02T21:50"}
---

## Vamos directo a lo bueno
Para crear un alias usamos el comando `alias NOMBRE_ALIAS='COMANDO'`. Sin embargo el alias solo estará activo mientas está abierta esa terminal. Para guardarlo y usarlo cuando queramos Usamos la misma estructura descrita arriba y envuelta en comillas dobles. Ejecutemos:

```bash
echo "alias NOMBRE_ALIAS='COMANDO'" >> .bashrc
```
- **`echo`** devuelve el resultado de todo lo que está en comillas dobles (").
- **`>>`** informa al sistema que todo lo anterior debe ser enviado a la ubicación que esta a la derecha.
- **`.bashrc`** es una carpeta oculta[^1] donde el sistema guarda los comandos de terminal, aquí enviaremos el resultado del `echo`.

Si lo pruebas, **aún no funcionará**. Para que los cambios surtan efecto debes reiniciar la terminal, cerrando y volviendo a abrirla.

[^1]: Las carpetas ocultas en Linux se identifican por tener un punto (.) al inicio del nombre.