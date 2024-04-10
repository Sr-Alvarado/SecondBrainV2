---
{"dg-publish":true,"dg-path":"Code/GitFlow.md","permalink":"/code/git-flow/","created":"2024-04-10T17:42","updated":"2024-04-10T17:42"}
---


![Pasted image 20240405213140.png|100%](/img/user/Engine/Attachments/Pasted%20image%2020240405213140.png)
El sistema GitFlow está basado en ramas específicas con roles muy bien definidos, las ramas principales son:
- La rama **[[Learning/Wiki/Main\|Main]]** es el proyecto en producción. Es la versión a la que tienen acceso los usuarios. En ningún caso deberías estar en esta rama, solo se usa para guardar las cosas.
- La rama **Development** es donde realmente se desarrollará el proyecto. Aquí es donde se hacen cambios y se desarrollan características sin afectar a los usuarios. Se [[Learning/Code/Git Terminal/merge - Fusionar la rama actual con otra rama en Git\|merge]]a a la rama principal [[Learning/Wiki/Main\|Main]].
- Las ramas **Feature** son aquellas ramas donde se desarrollan características. Es útil crear una rama para cada característica para mantener ordenado y limpio el proyecto. Permite que varios equipos trabajen en su característica sin que se afecten entre ellos. Se [[Learning/Code/Git Terminal/merge - Fusionar la rama actual con otra rama en Git\|merge]]a a la rama Development.

Adicionalmente existen 2 ramas extra entre las ramas [[Learning/Wiki/Main\|Main]] y Development.

 ![Pasted image 20240410171329.png](/img/user/Engine/Attachments/Pasted%20image%2020240410171329.png)
 - La rama **Release** es un adelanto de lo que vendrá luego. Añade las características "estables" de la rama Development al proyecto en producción. Se abre en Development porque tomará los cambios más recientes, se [[Learning/Code/Git Terminal/merge - Fusionar la rama actual con otra rama en Git\|merge]]a en [[Learning/Wiki/Main\|Main]] porque llevará esos cambios a producción y se cierra en Development porque ya actualizó la versión de producción con los últimos cambios de Development.
 - La rama **Hotfix** se usa para arreglar errores que aparezcan en el proyecto en producción. Se abre directamente de la rama [[Learning/Wiki/Main\|Main]] porque va a arreglar un problema y se cierra en la misma porque ya arregló el problema.

GitFlow permite mantener actualizadas todas las ramas. Puedes [[Learning/Code/Git Terminal/branch - Crear y eliminar ramas en Git\|crear, eliminar]], [[Learning/Code/Git Terminal/merge - Fusionar la rama actual con otra rama en Git\|merge]]ar, [[Learning/Code/Git Terminal/tag - Añadir una etiqueta a una fotografía en Git\|añadir tags]], [[Learning/Code/Git Terminal/switch - Moverse entre ramas en Git\|moverse]] entre ramas según el flujo establecido sin necesidad de hacerlo manualmente usando un plugin para [[Learning/Code/Git\|Git]]. 
```sh
brew install git-flow
```

Para comenzar a trabajar con GitFlow debes iniciarlo y configurarlo con:
```sh
git flow init
```
