---
{"dg-publish":true,"permalink":"/learning/code/git/","created":"2024-03-14T13:56","updated":"2024-03-16T15:54"}
---

Esta guía está diseñada para ser seguida de forma lineal, más hacia el principio se explican conceptos básicos y necesarios para entender lo que sigue luego, más hacia el final se da por sentado que se comprende ciertos conceptos y ya no se explican cosas que fueron explicadas antes. Sin embargo la estructura permite que encuentres justo lo que estas buscando.

**Fuentes**: 
- [Curso de GIT y GITHUB desde CERO para PRINCIPIANTES - YouTube](https://youtube.com/watch?v=3GymExBkKjE)
## ¿Qué es?
Es un [[Learning/Wiki/Sistema de control de versiones\|Sistema de control de versiones]] [[Learning/Wiki/distribuido\|distribuido]], es decir, es:

<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



Historial de todos los cambios de un proyecto. Documenta cada cambio hecho en una linea del tiempo que permite movernos entre cambios. 

</div></div>


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



Permite tener una copia local del contenido. No existe un repositorio central único, cada usuario tiene una copia local y modificable del repositorio. 

</div></div>


El sistema de control de versiónes usa la idea de [[Learning/Wiki/Rama\|rama]]s, y de [[Learning/Wiki/Fotografía\|Fotografía]]s de un proyecto es decir, es:

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/rama/#200880" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Bifurcación de un proyecto, puede existir infinitas ramas, cada rama tiene un nombre específico que la identifica. Todas comparten un único origen pero cada una es independiente y puede ser modificada de cualquier forma. La rama origen o principal se le conoce regularmente con el nombre de [[Learning/Wiki/main\|main]]. 

</div></div>


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/fotografia/#3dcda9" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Graba/Guarda la estructura, características y datos que un proyecto tenía en un determinado momento en el tiempo. 

</div></div>


## Historia
Creado por [[Linus Torvalds\|Linus Torvalds]] para facilitar el desarrollo de [[Linux\|Linux]].

## Instalación
Descarga la última versión para tu [[OS\|OS]] desde la página oficial Git.

## Uso
Para trabajar con Git necesitas 2 cosas básicas: un usuario y un email.
### Terminal `git`
Todos los comandos usados por Git funcionan el todos los OS de la misma forma. 

Los comandos más comunes de Git son:

#### Versión de Git
Una forma fácil de saber si tenemos instalado Git, y que versión tenemos, es usar:
```shell
git -v
```

#### Configurar Git
Toda configuración de Git se registra en el [[fichero\|fichero]] `.gitconfig`. Podrías añadir o modificar cualquier configuración directamente editando este fichero.

Cualquier configuración en Git sigue esta estructura:
```shell
git config --global
```
- `git`. Declara que se usará el programa Git.
- `config`. Declara que se usará el [[comando\|comando]] `config` del programa Git.
- `--global`. Es una [[etiqueta\|etiqueta]] del comando `config` que indica a que nivel se harán los cambios. En este caso los cambios afectarán a todos los usuarios del equipo.

#### Configurar el usuario en Git
Definir a tu usuario junto con el email es lo primero que debes hacer para usar Git.
```shell
git config --global user.name "TU_NOMBRE"
```
- `user.name`. Es la [[propiedad\|propiedad]] a modificar, en este caso el nombre del usuario.
- `"TU NOMBRE"`. Es el valor que se le asignará a esa propiedad.

#### Configurar el email en Git
```shell
git config --global user.email "TU_EMAIL"
```
- `user.email`. Es la [[propiedad\|propiedad]] a modificar, en este caso el email del usuario.
- `"TU NOMBRE"`. Es el valor que se le asignará a esa propiedad.

#### Usar Git en un proyecto
En la ruta de la carpeta de ese proyecto ejecuta:
```shell
git init
```
- `init`. Este comando crea una carpeta oculta `.git` que nos permite comenzar a trabajar con el control de versiones de Git y asigna nuestra carpeta como la [[Learning/Wiki/Rama\|Rama]] [[Learning/Wiki/main\|main]] del proyecto. Se puede cambiar el nombre de la rama.

#### Modificar el nombre de una rama en Git
En la ruta de la carpeta de ese proyecto ejecuta:
```shell
git branch -m NUEVO_NOMBRE
```
- `branch`. Propiedad de Git que indica que se modificarán las características de la rama.
- `-m`. Etiqueta de la propiedad `branch` que indica que se modificará el nombre de la rama.
- `NUEVO_NOMBRE`. Es el valor que se le asignará al nombre de la rama. 

#### Ver el estado del control de versiones en Git
```shell
git status
```
- `status`. Permite ver que ficheros incluidos si se hace una [[Learning/Wiki/Fotografía\|Fotografía]] y cuales no, cuales ficheros se han modificado.

#### Añadir ficheros a la fotografía en Git
```shell
git add NOMBRE_FICHERO
```
- `add`. Propiedad de Git que permite seleccionar que ficheros se agregarán a la [[Learning/Wiki/Fotografía\|Fotografía]].

#### Hacer una fotografía en Git
Si ya definiste que ficheros se agregarán a la [[Learning/Wiki/Fotografía\|Fotografía]] de tu proyecto es momento de hacerla:
```shell
git commit -m "COMENTARIO"
```
- `commit`. Propiedad que graba los cambios de una rama en Git. Todo cambio necesita un comentario. Crea un [[Learning/Wiki/hash\|hash]].
- `-m`. Etiqueta que declara que se hará un comentario para la grabación.

#### Mostrar el registro de fotografías Git
```shell
git log
```
- `log`. Muestra el registro de commits. Con el autor, email, hash, comentario, fecha y rama que se modificó.

#### Volver a la última fotografía de un fichero
Si luego de hacer una fotografía, modificas el fichero y quieres volver a como estaba antes, puedes usar:
```shell
git checkout NOMBRE_FICHERO
```
- `chekout`. Devuelve los datos de como estaba un fichero o todo el proyecto en la última fotografía.

#### Volver atrás una fotografía
Si hiciste una fotografía pero quieres volver a la anterior ejecuta:
```shell
git reset
```
- `reset`. Retrocede una fotografía. Modifica el proyecto o fichero dejándolo tal como estaba en la penúltima fotografía.

