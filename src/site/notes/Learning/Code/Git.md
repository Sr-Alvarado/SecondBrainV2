---
{"dg-publish":true,"permalink":"/learning/code/git/","created":"2024-03-14T13:56","updated":"2024-03-27T13:13"}
---

> [!info]
> Esta guía está diseñada para ser seguida de forma lineal, más hacia el principio se explican conceptos básicos y necesarios para entender lo que sigue luego, más hacia el final se da por sentado que se comprende ciertos conceptos y ya no se explican cosas que fueron explicadas antes. Sin embargo la estructura permite que encuentres justo lo que estas buscando.

## ¿Qué es?
**Es un [[Learning/Wiki/Sistema de control de versiones\|Sistema de control de versiones]]:**

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/learning/wiki/sistema-de-control-de-versiones/#4a1b0e" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Es un historial de todos los cambios de un proyecto. Documenta cada modificación en una linea del tiempo que permite moverse entre cambios. 

</div></div>


**Es [[Learning/Wiki/Distribuido\|Distribuido]]:**

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/learning/wiki/distribuido/#703a42" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Permite tener una copia local del contenido. No existe un repositorio central único, cada usuario tiene una copia local y modificable del repositorio. 

</div></div>


**Usa la idea de [[Learning/Wiki/Rama\|rama]]s:**

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/learning/wiki/rama/#200880" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Una rama es una bifurcación de un proyecto. Puede existir infinitas ramas, cada rama tiene un nombre específico y un [[Learning/Wiki/Hash\|hash]] que la identifica. Todas comparten un único origen o rama principal, [[Learning/Wiki/Main\|main]], pero cada una es independiente y puede ser modificada de cualquier forma. 

</div></div>


**Y de [[Learning/Wiki/Fotografía\|Fotografía]]s:**

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/learning/wiki/fotografia/#3dcda9" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Una fotografía es una instantánea de un proyecto. Graba/Guarda la estructura, características y datos de un proyecto en un determinado momento en el tiempo. 

</div></div>


## Historia
Creado por [[Linus Torvalds\|Linus Torvalds]] para facilitar el desarrollo de [[Linux\|Linux]].

## Instalación
Descarga la última versión para tu [[OS\|OS]] desde la página oficial Git.

## Uso
Para trabajar con Git necesitas 2 cosas básicas: un usuario y un email.
### Git en la terminal
Todos los comandos de Git tienen el mismo nombre y funcionan igual en todos los OS. Los comandos más usados son:

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
- `init`. Este comando crea una carpeta oculta `.git` que nos permite comenzar a trabajar con el control de versiones de Git y asigna nuestra carpeta como la [[Learning/Wiki/Rama\|Rama]] [[Learning/Wiki/Main\|Main]] del proyecto. Se puede cambiar el nombre de la rama.

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

#### Indicar a Git que ignore un archivo
Si no quieres añadir algún archivo a los commits, y no quieres que Git te indique que no lo has añadido, puedes indicar que lo ignore añadiendo su ruta al fichero `.gitignore`. Si no lo tienes, primero créalo:
```shell
touch .gitignore
```
- `touch`. Comando de Linux que permite crear nuevos archivos.
- `.gitignore`. Fichero de Git que registra ficheros a ignorar.

Ya con el fichero creado, añade las rutas dentro:
```git
**/NOMBRE_FICHERO_A_IGNORAR
```
- `**/`. Indica que se buscará ficheros con ese nombre en la carpeta principal y en todas sus sub-carpetas.
#### Hacer una fotografía en Git
Si ya definiste que ficheros se agregarán a la [[Learning/Wiki/Fotografía\|Fotografía]] de tu proyecto es momento de hacerla:
```shell
git commit -m "COMENTARIO"
```
- `commit`. Propiedad que graba los cambios de una rama en Git. Todo cambio necesita un comentario. Crea un [[Learning/Wiki/Hash\|Hash]].
- `-m`. Etiqueta que declara que se hará un comentario para la grabación.

#### Mostrar el registro de fotografías Git
```shell
git log --graph --decorate --all --oneline
```
- `log`. Muestra el registro de commits. Con el autor, email, [[Learning/Wiki/Hash\|hash]], comentario, fecha y rama que se modificó.
- `--graph`. Etiqueta de `log` que permite ver los commits de forma más gráfica.
- `--decorate`. Etiqueta de `log` que permite modificar el estilo del `log`.
- `--all`. Etiqueta de `log` que indica que se modificará todo el `log`.
- `--oneline`. Etiqueta de `log` que indica que se mostrará el resultado del `log` en una sola linea por commit.

#### Volver a la última fotografía de un fichero
Si luego de hacer una fotografía, modificas el fichero y quieres volver a como estaba antes, puedes usar:
```shell
git checkout NOMBRE_FICHERO_OPCIONAL
```
- `chekout`. Devuelve los datos de como estaba un fichero o todo el proyecto en la última fotografía.

#### Moverse a una fotografía específica
Para moverte a una fotografía específica solo debes copiar su [[Learning/Wiki/Hash\|hash]] como valor para el `checkout`.
```shell
git checkout HASH_DE_LA_FOTOGRAFIA_DESTINO
```
- **Info:** En algunos casos puede no funcionar, debido a que hay archivos que no han sido añadidos a la fotografía.
#### Definir la fotografía de destino como la última rama
Si quieres que la rama a la que te moviste sea reconocido por git como la última rama (fotografía).
```shell
git checkout HEAD
```
- `HEAD`. Declara a la rama actual como la última fotografía. Aún se conservan las ramas siguiente pero el árbol ahora crecerá desde esta rama.

#### Volver atrás una fotografía
Si hiciste una fotografía pero quieres volver a la anterior ejecuta:
```shell
git reset
```
- `reset`. Retrocede una fotografía. Modifica el proyecto o fichero dejándolo tal como estaba en la penúltima fotografía.

#### Crear "alias" en git
Git nos permite crear "alias" al mismo estilo de la terminal, solo debes añadir:
```shell
git config --global alias.ALIAS_NAME "YOUR_GIT_COMMAND"
```
- `alias.tree`. Propiedad de `config` que indica que se creará un alias en git.
- `.ALIAS_NAME`. Valor que tomará el nombre del alias.
- `"YOUR_GIT_COMMAND"`. El comando en git que se ejecutará cuando se llame a ese alias.
- **Ejemplo:** `git config --global alias.tree "log --graph --decorate --all --oneline"`

#### Ver los cambios entre el proyecto actual y la última fotografía
Si modificas tu proyecto pero no estás seguro de hacer una fotografía y quieres ver que parte del código cambiaste con respecto a la última fotografía puedes usar:
```shell
git diff
```
- `diff`. Propiedad de Git que devuelve los cambios en el código realizados entre la última fotografía y el momento actual. Devuelve: Nombre del archivo modificado, indica si se agregó o se eliminó algo, se especifica el número de lineas afectadas, y se imprime el antes y el después.
   ![Pasted image 20240318170923.png|600](/img/user/Engine/Attachments/Pasted%20image%2020240318170923.png)

---
**Fuentes**:
- [Curso de GIT y GITHUB desde CERO para PRINCIPIANTES - YouTube](https://youtube.com/watch?v=3GymExBkKjE)