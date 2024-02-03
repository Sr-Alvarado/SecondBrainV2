---
{"dg-publish":true,"dg-path":"Lanzar programas desde la terminal.md","permalink":"/lanzar-programas-desde-la-terminal/","tags":["linux","terminal","bash"]}
---

## Vamos de frente a lo bueno
Existen varios comandos que podemos usar para este fin, sin embargo mi preferido es:
```bash
nohup nombre_programa &
```
El comando `nohub` abre el programa independientemente de la terminal, al cerrar la terminal el programa sigue funcionando. Ademas al añadir `&` al final el programa se abre en segundo plano sin cambiar el foco de atención en la terminal.
## Otros comandos...
### `gksu NOMBRE_PROGRAMA`
Abre un programa con privilegios de superusuario.
### `./NOMBRE_PROGRAMA`
Abre cualquier programa que esté en el directorio actual donde nos encontramos.
