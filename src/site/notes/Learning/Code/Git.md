---
{"dg-publish":true,"dg-path":"Code/Git.md","permalink":"/code/git/","created":"2024-03-14T13:56","updated":"2024-03-29T19:00"}
---


> [!info]
> Esta es una guía diseñada para seguirse linealmente. Hacia el principio se explican conceptos más básicos, avanzando hacia el final se asume que comprendes esos conceptos y ya no se vuelven a explican. Además, la estructura permite que encuentres justo lo que estas buscando.
> 
>> [!cite]- **Fuentes:**
>> - [Curso de GIT y GITHUB desde CERO para PRINCIPIANTES - YouTube](https://youtube.com/watch?v=3GymExBkKjE)

## ¿Qué es Git?
**Es un [[Learning/Wiki/Sistema de control de versiones\|Sistema de control de versiones]]:** 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/sistema-de-control-de-versiones/#4a1b0e" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Es un historial de todos los cambios de un proyecto. Documenta cada modificación en una linea del tiempo que permite moverse entre cambios. 

</div></div>


**Es [[Learning/Wiki/Distribuido\|Distribuido]]:** 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/distribuido/#703a42" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Permite tener una copia local del contenido. No existe un repositorio central único, cada usuario tiene una copia local y modificable del repositorio. 

</div></div>


**Usa la idea de [[Learning/Wiki/Rama\|rama]]s:** 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/rama/#200880" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Una rama es una bifurcación de un proyecto. Puede existir infinitas ramas, cada una con infinitas fotografías, cada rama tiene un nombre específico que la identifica. Todas comparten un único origen o rama principal, [[Learning/Wiki/Main\|main]], pero cada una es independiente y puede ser modificada de cualquier forma. 

</div></div>


**Y de [[Learning/Wiki/Fotografía\|Fotografía]]s:** 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/fotografia/#3dcda9" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Una fotografía es una instantánea de un proyecto. Graba/Guarda la estructura, características y datos de un proyecto en un determinado momento en el tiempo. 

</div></div>


## Historia
Creado por [[Linus Torvalds\|Linus Torvalds]] para facilitar el desarrollo de [[Linux\|Linux]].

## Instalación
Descarga la última versión para tu [[OS\|OS]] desde la página oficial Git.

## Uso
Git es un programa para la terminal, sin embargo existen algunas opciones con interfaz gráfica. Para usar Git necesitas 2 cosas básicas: un usuario y un email.
### Usando git en la terminal
Todos los comandos de Git tienen el mismo nombre y funcionan igual en todos los OS. Los comandos más usados son:
- [[Learning/Code/Git Terminal/Versión de Git\|Versión de Git]]
- [[Learning/Code/Git Terminal/config - Configurar Git\|config - Configurar Git]]
- [[Learning/Code/Git Terminal/config user.name - Configurar el usuario en Git\|config user.name - Configurar el usuario en Git]]
- [[Learning/Code/Git Terminal/config user.mail - Configurar el email en Git\|config user.mail - Configurar el email en Git]]
- [[Learning/Code/Git Terminal/init - Usar Git en un proyecto\|init - Usar Git en un proyecto]]
- [[Learning/Code/Git Terminal/-m branch - Modificar el nombre de una rama en Git\|-m branch - Modificar el nombre de una rama en Git]] 
- [[Learning/Code/Git Terminal/status - Ver el estado del control de versiones en Git\|status - Ver el estado del control de versiones en Git]]
- [[Learning/Code/Git Terminal/add - Añadir ficheros a la fotografía en Git\|add - Añadir ficheros a la fotografía en Git]]
- [[Learning/Code/Git Terminal/gitignore - Indicar a Git que ignore un archivo\|gitignore - Indicar a Git que ignore un archivo]]
- [[Learning/Code/Git Terminal/config alias - Crear alias en Git\|config alias - Crear alias en Git]]
- [[Learning/Code/Git Terminal/commit - Hacer una fotografía en Git\|commit - Hacer una fotografía en Git]]
- [[Learning/Code/Git Terminal/log - Mostrar el registro de fotografías hasta la cabeza del proyecto en Git\|log - Mostrar el registro de fotografías hasta la cabeza del proyecto en Git]] 
- [[Learning/Code/Git Terminal/checkout - Restaurar fotografías o archivos específicos en Git\|checkout - Restaurar fotografías o archivos específicos en Git]] 
- [[Learning/Code/Git Terminal/checkout HEAD - Definir la fotografía como la cabeza del proyecto en Git\|checkout HEAD - Definir la fotografía como la cabeza del proyecto en Git]] 
- [[Learning/Code/Git Terminal/reset - Retroceder a una fotografía anterior en  Git\|reset - Retroceder a una fotografía anterior en  Git]] 
- [[Learning/Code/Git Terminal/diff - Ver las diferencias entre el estado actual y la última fotografía u otra rama en Git\|diff - Ver las diferencias entre el estado actual y la última fotografía u otra rama en Git]] 
- [[Learning/Code/Git Terminal/reflog - Ver todos los cambios del proyecto en el tiempo en Git\|reflog - Ver todos los cambios del proyecto en el tiempo en Git]] 
- [[Learning/Code/Git Terminal/tag - Añadir una etiqueta a una fotografía en Git\|tag - Añadir una etiqueta a una fotografía en Git]] 
- [[Learning/Code/Git Terminal/checkout tags - Moverse entre fotografías usando los tags en Git\|checkout tags - Moverse entre fotografías usando los tags en Git]] 
- [[Learning/Code/Git Terminal/branch - Crear y eliminar ramas en Git\|branch - Crear y eliminar ramas en Git]] 
- [[Learning/Code/Git Terminal/switch - Moverse entre ramas en Git\|switch - Moverse entre ramas en Git]] 
- [[Learning/Code/Git Terminal/merge - Fusionar la rama actual con otra rama en Git\|merge - Fusionar la rama actual con otra rama en Git]] 
   - [[Learning/Code/Resolver conflictos en Git\|Resolver conflictos en Git]]
- [[Learning/Code/Git Terminal/stash - Guardar los cambios de forma temporal en Git\|stash - Guardar los cambios de forma temporal en Git]] 
- [[Learning/Code/Git Terminal/stash pop - Recuperar los cambios guardados temporalmente en Git\|stash pop - Recuperar los cambios guardados temporalmente en Git]] 
- [[Learning/Code/Git Terminal/stash drop - Elimina los cambios guardados de temporalmente en Git\|stash drop - Elimina los cambios guardados de temporalmente en Git]] 

### Usando Git con Interfaz gráfica
- GitKraken
- GitHub Desktop
- Sourcetree

### Usando Git con plataformas online 
- [[Learning/Code/GitHub\|GitHub]] 
- GitLab
