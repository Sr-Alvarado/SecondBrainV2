---
{"dg-publish":true,"permalink":"/learning/nvm/","created":"2024-01-25T19:06","updated":"2024-03-19T16:30"}
---

**Fuentes**: 
- [GitHub - nvm-sh/nvm: Node Version Manager](https://github.com/nvm-sh/nvm)

## ¿Qué es?
Programa que permite instalar multiples versiones de Node en un solo dispositivo.

## Uso

### Instalar y/o actualizar NVM
```shell
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```
- `curl`. Comando de terminal que permite transferir datos desde o hacia un servidor (internet).
- `-o-`. Propiedad de `curl` que indica que el archivo a continuación se enviará a la salida standard en vez de guardarlo en un archivo específico.
- `| bash`. Define la salida standard como la sesión de terminal actual. 
- **Resultado**. El archivo descargado a través de `curl` no se guardará en vez de eso se devolverá a la salida predeterminada que se definió como `bash` es decir, la sesión actual de la terminal.

### Activar NVM para Linux
Ahora solo queda activar NVM con:
```shell
source ~/.bashrc
```
- `source`. Comando de terminal que permite ejecutar comandos desde un archivo script.

### Instalar la última versión de Node
Si quieres instalar la última versión de Node sin especificar su nombre usa:
```shell
nvm install node
```
- `nvm`. Comando de terminal que llama al programa NVM.
- `install`. Propiedad del comando `nmv` que declara que se instalará una versión de NodeJS.
- `node`. Atributo de la propiedad `install` que asume el alias de la última versión de NodeJS.