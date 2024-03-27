---
{"dg-publish":true,"permalink":"/learning/code/git/","created":"2024-03-14T13:56","updated":"2024-03-27T16:27"}
---

> [!info]
> Esta guía está diseñada para ser seguida de forma lineal, más hacia el principio se explican conceptos básicos y necesarios para entender lo que sigue luego, más hacia el final se da por sentado que se comprende ciertos conceptos y ya no se explican cosas que fueron explicadas antes. Sin embargo la estructura permite que encuentres justo lo que estas buscando.
> 
>> [!cite]- **Fuentes:**
>> - [Curso de GIT y GITHUB desde CERO para PRINCIPIANTES - YouTube](https://youtube.com/watch?v=3GymExBkKjE)

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
Para trabajar con Git necesitas 2 cosas básicas: un usuario y un email. Git es un programa para la terminal, sin embargo existen algunas opciones con interfaz gráfica:
- GitKraken
- GitHub Desktop
- Sourcetree
### Usando git en la terminal
Todos los comandos de Git tienen el mismo nombre y funcionan igual en todos los OS. Los comandos más usados son:
- [[Learning/Code/Git Terminal/Versión de Git\|Versión de Git]]
- [[Learning/Code/Git Terminal/Configurar Git\|Configurar Git]]
- [[Learning/Code/Git Terminal/Configurar el usuario en Git\|Configurar el usuario en Git]]
- [[Learning/Code/Git Terminal/Configurar el email en Git\|Configurar el email en Git]]
- [[Learning/Code/Git Terminal/Usar Git en un proyecto\|Usar Git en un proyecto]]
- [[Learning/Code/Git Terminal/Modificar el nombre de una rama en Git\|Modificar el nombre de una rama en Git]] 
- [[Learning/Code/Git Terminal/Ver el estado del control de versiones en Git\|Ver el estado del control de versiones en Git]]
- [[Learning/Code/Git Terminal/Añadir ficheros a la fotografía en Git\|Añadir ficheros a la fotografía en Git]]
- [[Learning/Code/Git Terminal/Indicar a Git que ignore un archivo\|Indicar a Git que ignore un archivo]]
- [[Learning/Code/Git Terminal/Hacer una fotografía en Git\|Hacer una fotografía en Git]]
- [[Learning/Code/Git Terminal/Mostrar el registro de fotografías Git\|Mostrar el registro de fotografías Git]]
- [[Learning/Code/Git Terminal/Volver a la última fotografía de un fichero\|Volver a la última fotografía de un fichero]]
- [[Learning/Code/Git Terminal/Moverse a una fotografía específica\|Moverse a una fotografía específica]]
- [[Learning/Code/Git Terminal/Definir la fotografía de destino como la última rama\|Definir la fotografía de destino como la última rama]]
- [[Learning/Code/Git Terminal/Volver atrás una fotografía\|Volver atrás una fotografía]]
- [[Learning/Code/Git Terminal/Crear alias en git\|Crear alias en git]]
- [[Learning/Code/Git Terminal/Ver los cambios entre el proyecto actual y la última fotografía\|Ver los cambios entre el proyecto actual y la última fotografía]]
