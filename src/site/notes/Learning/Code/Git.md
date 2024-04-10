---
{"dg-publish":true,"dg-path":"Code/Git.md","permalink":"/code/git/","created":"2024-03-14T13:56","updated":"2024-04-10T16:56"}
---


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



Permite tener una copia local completa del contenido. No existe un repositorio central único, cada usuario tiene una copia local y modificable del repositorio que puede actualizar.![Pasted image 20240405172045.png|50%](/img/user/Engine/Attachments/Pasted%20image%2020240405172045.png) 

</div></div>


**y usa [[Learning/Wiki/Fotografía\|Fotografía]]s:** 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/fotografia/#3dcda9" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



Conocida en Git como [[Learning/Code/Git Terminal/commit - Hacer una fotografía en Git\|commit]], una fotografía es una instantánea de un proyecto. Graba/Guarda la estructura, características y datos de un proyecto en un determinado momento en el tiempo. Si no hubo cambios entre fotografías Git no guarda nuevamente la estructura si que almacena un enlace a la fotografía anterior.![Pasted image 20240404191110.png|100%](/img/user/Engine/Attachments/Pasted%20image%2020240404191110.png) 

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
{ #96012c}


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
- [[Learning/Code/Git Terminal/log - Mostrar el registro de fotografías del proyecto en Git\|log - Mostrar el registro de fotografías del proyecto en Git]] 
- [[Learning/Code/Git Terminal/checkout - Moverse entre fotografías o archivos específicos en Git\|checkout - Moverse entre fotografías o archivos específicos en Git]] 
- [[Learning/Code/Git Terminal/checkout tags - Moverse entre fotografías usando los tags en Git\|checkout tags - Moverse entre fotografías usando los tags en Git]] 
- [[Learning/Code/Git Terminal/checkout HEAD - Definir la fotografía como la cabeza del proyecto en Git\|checkout HEAD - Definir la fotografía como la cabeza del proyecto en Git]] 
- [[Learning/Code/Git Terminal/restore - Restaurar un archivo a la última versión en Git\|restore - Restaurar un archivo a la última versión en Git]] 
- [[Learning/Code/Git Terminal/reset - Restaurar los cambios a una fotografía anterior en  Git\|reset - Restaurar los cambios a una fotografía anterior en  Git]] 
- [[Learning/Code/Git Terminal/diff - Ver diferencias entre un commit y ahora en Git\|diff - Ver diferencias entre un commit y ahora en Git]] 
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
- [[Learning/Code/Git Terminal/config pull - Configurar el tipo de modificación de ficheros con pull en Git\|config pull - Configurar el tipo de modificación de ficheros con pull en Git]] 
- [[Learning/Code/Git Terminal/clone - Descargar un proyecto de un repo remoto en Git\|clone - Descargar un proyecto de un repo remoto en Git]] 
- [[Learning/Code/Git Terminal/fork - Copiar un repo remoto a mi propio repo remoto\|fork - Copiar un repo remoto a mi propio repo remoto]] 

### Usando Git con plataformas online 
- [[Learning/Code/GitHub\|GitHub]]. Se puede usar en todas las plataformas (web, móvil, desktop, [[consola\|CLI]]). ~~A mi me gusta [[GitHub CLI\|GitHub CLI]] sin embargo tu debes usar lo que a ti te sirva mejor.~~ 
- GitLab

### Usando Git con Interfaz gráfica
- [GitHub Desktop](https://desktop.github.com/). Herramienta útil para entender los conceptos básicos, se queda corta con flujos más complicados. Es gratuita.
- [GitKraken](https://www.gitkraken.com/). Herramienta muy completa y preparada para flujos completos, útil para visualizar proyectos muy grandes. Es gratuita para repos públicos y de pago para repos privados. 

## Flujos de trabajo en Git
- [[Learning/Code/GitFlow - Trabajo local con Git\|GitFlow - Trabajo local con Git]] 
- [[Learning/Code/GitHub Flow - Flujo colaborativo\|GitHub Flow - Flujo colaborativo]] 