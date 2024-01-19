---
{"dg-publish":true,"dg-path":"Lanzar programas desde la terminal linux.md","permalink":"/lanzar-programas-desde-la-terminal-linux/","tags":["linux","terminal","bash"]}
---

## Vamos de frente a lo bueno
Existen varios comandos que podemos usar para este fin, sin embargo mi preferido es:
```bash
nohub nombre_programa &
```
El comando `nohub` abre el programa independientemente de la terminal, al cerrar la terminal el programa sigue funcionando. Ademas al añadir `&` al final el programa se abre en segundo plano sin cambiar el foco de atención en la terminal.
## Otros comandos...
### `gksu nombre_programa`
Abrir un programa con privilegios de superusuario.
### `./nombre_programa`
Abre cualquier programa que esté en el directorio actual donde nos encontramos.
