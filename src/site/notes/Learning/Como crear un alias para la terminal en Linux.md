---
{"dg-publish":true,"dg-path":"Como crear un alias para la terminal en Linux.md","permalink":"/como-crear-un-alias-para-la-terminal-en-linux/","tags":["linux","terminal","bash"],"created":"2024-01-27T22:11","updated":"2024-03-02T21:50"}
---

## Vamos directo a lo bueno
Para crear un alias usamos el comando `alias NOMBRE_ALIAS='COMANDO'`. Sin embargo el alias solo estará activo mientas está abierta esa terminal. Para guardarlo y usarlo cuando queramos ejecutamos:

```bash
echo "alias NOMBRE_ALIAS='COMANDO'" >> .bashrc
```
- Usamos la misma estructura descrita arriba y envuelta en comillas dobles.
- El comando `echo` nos devuelve el resultado de todo lo que está en comillas dobles.
- Los `>>` informan al sistema que todo lo anterior debe enviarlo a la ubicación que esta a ala derecha.
- El `.bashrc` indica que enviaremos el resultado del `echo` a la carpeta oculta bashrc que es donde el sistema guarda los comandos de terminal.

Si lo pruebas, **aún no funcionará**. Para que los cambios surtan efecto debes reiniciar la terminal, cerrando y volviendo a abrirla.