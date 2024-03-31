---
{"dg-publish":true,"dg-path":"Code/Node.js.md","permalink":"/code/node-js/","created":"2024-01-25T19:06","updated":"2024-03-31T14:36"}
---


>[!info]-
>> [!cite]+ Fuentes y enlaces de interés
>> - [Linux para Desarrollo Web, Instalando Programas en Linux Lite 4 - YouTube](https://www.youtube.com/watch?v=526NfikEVCM&t=460s)

## ¿Qué es?
Entorno en tiempo de ejecución multiplataforma, de código abierto, para la capa del servidor creado en JavaScript, asíncrono, con E/S de datos en una arquitectura orientada a eventos y basado en el motor V8 de Google.

## Instalar Node.js a través de [[Learning/Code/NVM\|NVM]]

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/nvm/#instalar-y-o-actualizar-nvm" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



### Instalar y/o actualizar NVM
```shell
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```
- `curl`. Comando de terminal que permite transferir datos desde o hacia un servidor (internet).
- `-o-`. Propiedad de `curl` que indica que el archivo a continuación se enviará a la salida standard en vez de guardarlo en un archivo específico.
- `| bash`. Define la salida standard como la sesión de terminal actual. 
- **Resultado**. El archivo descargado a través de `curl` no se guardará en vez de eso se devolverá a la salida predeterminada que se definió como `bash` es decir, la sesión actual de la terminal.


</div></div>


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/nvm/#activar-nvm-para-linux" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">





> [!info]-
>> [!cite]+ Fuentes y enlaces de interés
>> - [GitHub - nvm-sh/nvm: Node Version Manager](https://github.com/nvm-sh/nvm)

## ¿Qué es?
Programa que permite instalar multiples versiones de [[Learning/Code/Node.js\|Node]] en un solo dispositivo.

## Uso
### Instalar y/o actualizar NVM
```shell
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```
- `curl`. Comando de terminal que permite transferir datos desde o hacia un servidor (internet).
- `-o-`. Propiedad de `curl` que indica que el archivo a continuación se enviará a la salida standard en vez de guardarlo en un archivo específico.
- `| bash`. Define la salida standard como la sesión de terminal actual. 
- **Resultado**. El archivo descargado a través de `curl` no se guardará en vez de eso se devolverá a la salida predeterminada que se definió como `bash` es decir, la sesión actual de la terminal.

### Activar NVM en Linux
Ahora solo queda activar NVM en tu dispositivo [[Learning/Wiki/Linux\|Linux]] con:
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

</div></div>


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/nvm/#instalar-la-ultima-version-de-node" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



### Instalar la última versión de Node
Si quieres instalar la última versión de Node sin especificar su nombre usa:
```shell
nvm install node
```
- `nvm`. Comando de terminal que llama al programa NVM.
- `install`. Propiedad del comando `nmv` que declara que se instalará una versión de NodeJS.
- `node`. Atributo de la propiedad `install` que asume el alias de la última versión de NodeJS.

</div></div>

