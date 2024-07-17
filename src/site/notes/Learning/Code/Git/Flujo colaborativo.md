---
{"dg-publish":true,"dg-path":"Code/Git/Flujo colaborativo.md","permalink":"/code/git/flujo-colaborativo/","created":"2024-04-04T14:22","updated":"2024-04-10T17:41"}
---


> [!info]-
>> [!cite]+ **Fuentes y enlaces de interés:**
>> - [Curso de GIT y GITHUB desde CERO para PRINCIPIANTES - YouTube](https://youtube.com/watch?v=3GymExBkKjE)
>> - [What is the best Git branch strategy? | Git Best Practices](https://www.gitkraken.com/learn/git/best-practices/git-branch-strategy)

## Como contribuidor

- Hacer un [[Learning/Code/Git/fork - Copiar un repo remoto a mi propio repo remoto\|fork]] de un repo 
- [[Learning/Code/Git/clone - Descargar un proyecto de un repo remoto en Git\|Clonar]] el repo remoto desde tu fork
- Trabajar con el [[Learning/Code/Git/Trabajo local con Git#^ce8d5e\|flujo local con repo remoto]]
   
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/git/trabajo-local-con-git/#ce8d5e" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



![Pasted image 20240405200141.png|100%](/img/user/Engine/Attachments/Pasted%20image%2020240405200141.png) 

</div></div>

- Sincroniza tu repo remoto con el repo remoto original en [[Learning/Code/GitHub/GitHub\|GitHub]] con `sync fork`. Trae los últimos [[Learning/Code/Git/commit - Hacer una fotografía en Git\|cambios]] a tu remo remoto.
- Hacer una [[pull request\|pull request]]. Añadir un título que describa claramente los cambios y una descripción que aclare a detalle estos cambios. Especificar el repositorio de destino.

## Como propietario
Si eres el propietario de un repo tu proceso de flujo colaborativo comienza luego de que otro usuario envíe una [[pull request\|pull request]].
- Debes aceptar, pedir cambios o denegar los cambios
- Si aceptas los cambios. Lo siguiente es [[Learning/Code/Git/merge - Fusionar la rama actual con otra rama en Git\|merge]]ar los cambios en la rama principal.

### Resolución de conflictos
Si hay algún conflicto Git no permitirá [[Learning/Code/Git/merge - Fusionar la rama actual con otra rama en Git\|merge]]ar. Lo que debes hacer es:

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/git/resolver-conflictos-en-git/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




## En local
Si tienes conflictos y estas usando el editor de código [[vscode\|vscode]], en el mismo editor te aparecerán las lineas de código en conflicto. Lo único que tienes que hacer es:
- Modificar tu código borrando el código que has modificado y manteniendo el modificado por la rama principal.
- Guardar el archivo y añadirlo a los archivos a fotografiar con `add`.
- Hacer una nueva fotografía del proyecto.
- Y ahora si usar `merge` para actualizar tu rama a la última versión de la rama principal

## En GitHub
Si tienes conflictos de [[pull request\|pull request]] porque el repo de origen está des-actualizado puedes usar:
- Ir a la parte de conflicto de la [[pull request\|pr]] 
- Editar directamente en [[Learning/Code/GitHub/GitHub\|GitHub]] con su editor integrado
- Marcar como resuelto y [[Learning/Code/Git/commit - Hacer una fotografía en Git\|commit]]ear el archivo editado
- Ahora si ya puedes [[Learning/Code/Git/merge - Fusionar la rama actual con otra rama en Git\|merge]]ar la [[pull request\|pr]] 

</div></div>
 
