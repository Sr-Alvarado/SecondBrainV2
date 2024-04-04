---
{"dg-publish":true,"dg-path":"Code/GitHub.md","permalink":"/code/git-hub/","created":"2024-03-29T19:03","updated":"2024-03-30T23:51"}
---


> [!info]-
>> [!cite]+ **Fuentes y enlaces de interés:**
>> - [Curso de GIT y GITHUB desde CERO para PRINCIPIANTES - YouTube](https://youtube.com/watch?v=3GymExBkKjE)
>> - [Hoja de referencia para Git de Github - GitHub Cheatsheets](https://training.github.com/downloads/es_ES/github-git-cheat-sheet/)
>> - [GitHub Docs](https://docs.github.com/es)

## ¿Qué es GitHub?
Plataforma de desarrollo colaborativo, usa el sistema de control de versiones [[Learning/Code/Git\|Git]]. Permite a los desarrolladores almacenar, gestionar y compartir proyectos de software de forma eficiente. Es la red social por excelencia para programadores.

## Historia
Fue fundada en 2008. Actualmente le pertenece a Microsoft.

## Uso
GitHub está presente en todas las plataformas: Web, Android, [[Learning/Wiki/Linux\|Linux]], Windows y IOS. Pero lo más común es usarlo con [[vscode\|vscode]], a través de la [[terminal\|terminal]] y en su versión web. Lo único que necesitas para usarlo es crearte una cuenta.

### Usar comandos `git`
[[Learning/Code/Git\|Git]] 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/git/#dac427" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">





> [!info]-
> Esta es una guía diseñada para seguirse linealmente. Hacia el principio se explican conceptos más básicos, avanzando hacia el final se asume que comprendes esos conceptos y ya no se vuelven a explican. Además, la estructura permite que encuentres justo lo que estas buscando.
> 
>> [!cite]+ **Fuentes y enlaces de interés:**
>> - [Curso de GIT y GITHUB desde CERO para PRINCIPIANTES - YouTube](https://youtube.com/watch?v=3GymExBkKjE)
>> - [Hoja de referencia para Git de Github - GitHub Cheatsheets](https://training.github.com/downloads/es_ES/github-git-cheat-sheet/)
>> - [GitHub - santyjL/30-dias-git-github](https://github.com/santyjL/30-dias-git-github/tree/main)

## ¿Qué es Git?
**Es un [[Learning/Wiki/Sistema de control de versiones\|Sistema de control de versiones]]:** 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/sistema-de-control-de-versiones/#4a1b0e" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Es un historial de todos los cambios de un proyecto. Documenta cada modificación en una linea del tiempo que permite moverse entre cambios. 

</div></div>


**Es [[Learning/Wiki/Distribuido\|Distribuido]]:** 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/distribuido/#703a42" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Permite tener una copia local completa del contenido. No existe un repositorio central único, cada usuario tiene una copia local y modificable del repositorio que puede actualizar. 

</div></div>
![Pasted image 20240402173426.png](/img/user/Engine/Attachments/Pasted%20image%2020240402173426.png)

**Usa [[Learning/Wiki/Rama\|rama]]s:** 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/rama/#200880" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Una rama es una bifurcación de un proyecto. Puede existir infinitas ramas, cada una con infinitas fotografías, cada rama tiene un nombre específico que la identifica. Todas comparten un único origen o rama principal, [[Learning/Wiki/Main\|main]], pero cada una es independiente y puede ser modificada de cualquier forma. 

</div></div>
![Pasted image 20240402173535.png](/img/user/Engine/Attachments/Pasted%20image%2020240402173535.png)

**y usa [[Learning/Wiki/Fotografía\|Fotografía]]s:** 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/fotografia/#3dcda9" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Conocida en Git como [[Learning/Code/Git Terminal/commit - Hacer una fotografía en Git\|commit]], una fotografía es una instantánea de un proyecto. Graba/Guarda la estructura, características y datos de un proyecto en un determinado momento en el tiempo. Si no hubo cambios entre fotografías Git no guarda nuevamente la estructura si que almacena un enlace a la fotografía anterior. 

</div></div>


**Utiliza un [[Learning/Wiki/Hash\|hash]] para confirmar la integridad de los datos e identificar un commit:** 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/hash/#c1dcc8" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Identificador único de 40 dígitos [[Learning/Wiki/hexadecimales\|hexadecimales]] calculado en base al contenido del archivo o la estructura del directorio. Integrada al más bajo nivel, hace imposible la perdida o corrupción de datos durante la transmisión, impide la modificación de los datos sin que el sistema se entere. En proyectos pequeños se puede usar solo los últimos 7 dígitos como identificardor. 

</div></div>
  

Existen otros tipos de sistemas de control de versiones:
- [[Learning/Code/Sistema de control de versiones local\|Sistema de control de versiones local]] 
- [[Learning/Code/Sistema de control de versiones centralizado\|Sistema de control de versiones centralizado]] 
## Historia
Creado por [[Linus Torvalds\|Linus Torvalds]] para facilitar el desarrollo de [[Learning/Wiki/Linux\|Linux]].

## Instalación
Descarga la última versión para tu [[OS\|OS]] desde la [página oficial Git](https://git-scm.com/).

## Uso
Git es un programa para la terminal, sin embargo existen algunas opciones online como [[Learning/Code/GitHub\|GitHub]] y otras con interfaz gráfica como [[GitKraken\|GitKraken]]. Para usar Git siempre vas a necesitar 2 cosas básicas: un usuario y un email.

### Usando git de forma local en la terminal
Todos los comandos de Git tienen el mismo nombre y funcionan igual en todos los [[OS\|OS]]. Los comandos más usados son:
- [[Learning/Code/Git Terminal/v - Versión de Git\|v - Versión de Git]]
- [[Learning/Code/Git Terminal/config - Configurar Git\|config - Configurar Git]]
- [[Learning/Code/Git Terminal/config user name - Configurar el usuario en Git\|config user name - Configurar el usuario en Git]]
- [[Learning/Code/Git Terminal/config user mail - Configurar el email en Git\|config user mail - Configurar el email en Git]]
- [[Learning/Code/Git Terminal/init - Usar Git en un proyecto\|init - Usar Git en un proyecto]]
- [[Learning/Code/Git Terminal/branch -m - Modificar el nombre de una rama en Git\|branch -m - Modificar el nombre de una rama en Git]] 
- [[Learning/Code/Git Terminal/status - Ver el estado del control de versiones en Git\|status - Ver el estado del control de versiones en Git]]
- [[Learning/Code/Git Terminal/add - Añadir ficheros a la fotografía en Git\|add - Añadir ficheros a la fotografía en Git]]
- [[Learning/Code/Git Terminal/gitignore - Indicar a Git que ignore un archivo\|gitignore - Indicar a Git que ignore un archivo]]
- [[Learning/Code/Git Terminal/config alias - Crear alias en Git\|config alias - Crear alias en Git]]
- [[Learning/Code/Git Terminal/commit - Hacer una fotografía en Git\|commit - Hacer una fotografía en Git]]
- [[Learning/Code/Git Terminal/log - Mostrar el registro de fotografías hasta la cabeza del proyecto en Git\|log - Mostrar el registro de fotografías hasta la cabeza del proyecto en Git]] 
- [[Learning/Code/Git Terminal/checkout - Moverse entre fotografías o archivos específicos en Git\|checkout - Moverse entre fotografías o archivos específicos en Git]] 
- [[Learning/Code/Git Terminal/checkout tags - Moverse entre fotografías usando los tags en Git\|checkout tags - Moverse entre fotografías usando los tags en Git]] 
- [[Learning/Code/Git Terminal/checkout HEAD - Definir la fotografía como la cabeza del proyecto en Git\|checkout HEAD - Definir la fotografía como la cabeza del proyecto en Git]] 
- [[Learning/Code/Git Terminal/reset - Retroceder a una fotografía anterior en  Git\|reset - Retroceder a una fotografía anterior en  Git]] 
- [[Learning/Code/Git Terminal/diff - Ver las diferencias entre el estado actual y la última fotografía u otra rama en Git\|diff - Ver las diferencias entre el estado actual y la última fotografía u otra rama en Git]] 
- [[Learning/Code/Git Terminal/reflog - Ver todos los cambios del proyecto en el tiempo en Git\|reflog - Ver todos los cambios del proyecto en el tiempo en Git]] 
- [[Learning/Code/Git Terminal/tag - Añadir una etiqueta a una fotografía en Git\|tag - Añadir una etiqueta a una fotografía en Git]] 
- [[Learning/Code/Git Terminal/branch - Crear y eliminar ramas en Git\|branch - Crear y eliminar ramas en Git]] 
- [[Learning/Code/Git Terminal/switch - Moverse entre ramas en Git\|switch - Moverse entre ramas en Git]] 
- [[Learning/Code/Git Terminal/merge - Fusionar la rama actual con otra rama en Git\|merge - Fusionar la rama actual con otra rama en Git]] 
   - [[Learning/Code/Resolver conflictos en Git\|Resolver conflictos en Git]] 
- [[Learning/Code/Git Terminal/stash - Guardar los cambios de forma temporal en Git\|stash - Guardar los cambios de forma temporal en Git]] 
- [[Learning/Code/Git Terminal/stash pop - Recuperar los cambios guardados temporalmente en Git\|stash pop - Recuperar los cambios guardados temporalmente en Git]] 
- [[Learning/Code/Git Terminal/stash drop - Elimina los cambios guardados de temporalmente en Git\|stash drop - Elimina los cambios guardados de temporalmente en Git]] 

Usando Git en la terminal **con repositorios remotos**: 
- [[Learning/Code/Git Terminal/remote add origin - Conecta tu repositorio local con un servidor remoto en Git\|remote add origin - Conecta tu repositorio local con un servidor remoto en Git]] 
- [[Learning/Code/Git Terminal/push -u origin - Asociar una rama remota con una rama local en Git\|push -u origin - Asociar una rama remota con una rama local en Git]] 
- [[Learning/Code/Git Terminal/push - Subir los cambios a una rama remota\|push - Subir los cambios a una rama remota]] 
- [[Learning/Code/Git Terminal/fetch - Descargar solo el historial de un repo remoto en Git\|fetch - Descargar solo el historial de un repo remoto en Git]] 
- [[Learning/Code/Git Terminal/pull - Descargar los cambios del repo remoto en Git\|pull - Descargar los cambios del repo remoto en Git]] 
- [[Learning/Code/Git Terminal/config pull - Configurar como se modificarán los ficheros al descargar cambios de un repo remoto en Git\|config pull - Configurar como se modificarán los ficheros al descargar cambios de un repo remoto en Git]] 
- [[Learning/Code/clone - Descargar un proyecto de un repo remoto en Git\|clone - Descargar un proyecto de un repo remoto en Git]] 
- fork - Próximamente...

### Usando Git con plataformas online 
- [[Learning/Code/GitHub\|GitHub]] 
- GitLab

### Usando Git con Interfaz gráfica
- GitKraken
- GitHub Desktop
- Sourcetree


</div></div>


### Autenticar tu PC con GitHub
Si quieres comenzar a trabajar con GitHub debes autenticar tu dispositivo para poder subir y bajar repositorios y proyectos de sus servidores, existen algunas formas de hacerlo las más comunes son:
{ #e8e559}

- [[Learning/Code/SSH\|SSH]] 
- HTTP

### Personaliza tu perfil
- [[Learning/Code/Añadir una descripción a mi perfil de GitHub usando README\|Añadir una descripción a mi perfil de GitHub usando README]] 

### Licencias
Es el reglamento legal que indica el nivel de permisos que sede el creador del repositorio. Las más usadas son:
- MIT License
- Apache license 2.0
