---
{"dg-publish":true,"dg-path":"Como contribuir a un proyecto con Git.md","permalink":"/como-contribuir-a-un-proyecto-con-git/","title":"Como contribuir a un proyecto con Git","tags":["git","github","terminal","publish"]}
---

Basado en el video de [midudev](https://github.com/midudev) en [Youtube](https://www.youtube.com/watch?v=niPExbK8lSw) 
## Donde encontrar proyectos para contribuir
Existen varias páginas web que recopilan proyectos (issues) para poder contribuir:
- [For Good First Issue](https://forgoodfirstissue.github.com/): Página oficial de GitHub con proyectos Open Source y de apoyo a la sociedad en los que contribuir.
- [Good First Issue](https://goodfirstissue.dev/): Página enfocada en issues para personas que están comenzado, recopila issues "fáciles" de solucionar para que puedas hacer tus primeras contribuciones.
- [Good First Issues](https://goodfirstissues.com/): Está enfocada en el mismo objetivo que la anterior, busca todas las Issues con la etiqueta `good-first-issue` y las recopila en su página.
### Tips:
- Busca Issues de proyectos que te interesen.
- Revisa los comentarios para verificar que la Issue aún no ha sido resuelta.
- Para mejorar tus posibilidades que el ownership añada tus cambios sigue la guía de como contribuir al proyecto. Todos los proyectos añaden un post (markdown) en sus proyectos sobre como contribuir.
## Diferencias entre un fork y un clon del proyecto
- Un fork es copiar un proyecto completo, con todo su contenido a tu perfil de GitHub. Por lo tanto puedes modificar y subir esos cambios con Git a tu propio perfil.
- Un clon es copiar de forma local una parte o todo el proyecto, sin embargo no puedes subir tus cambios al proyecto porque no eres el Owner del proyecto.
### Tips
- Antes de hacer un clon o un fork revisa la licencia del proyecto, dependiendo del tipo de licencia podrás hacer una, otra o las dos.
## Hacer un fork de un proyecto
El fork se hace desde la página del proyecto en GitHub.
- Haz click en el botón `fork` que está en la barra al nivel del nombre del proyecto al lado izquierdo.
- Te cargará una página donde puedes modificar los datos del proyecto, como estás creando una copia hacia tu perfil, puedes modificar el nombre y la descripción del proyecto.
- Haz click en el botón `Create Fork` y listo.
- Una vez con el proyecto en tu perfil puedes clonarlo y trabajar con el de forma local, cuando quieras subir esos cambios a GitHub se subirán al proyecto dentro de tu perfil.
### Tips
- Puedes ir actualizando el proyecto para que se modifiquen los cambios que el owner original haga en su repositorio.
## Clonar un proyecto
Debes dirigirte al GitHub del proyecto y hacer click en el botón verde que dice `<> Code`. Encontrarás que hay varias maneras de clonar el proyecto, aquí repasaremos las más comunes. 
- **Con HTTPS**. No es muy recomendable hacerlo de esta manera, te pedirá un usuario y una contraseña.
- **Con SSH**. Es una mejor opción, sin embargo requiere una [configuración previa](https://docs.github.com/es/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account). Una vez configurada tu llave de acceso solo debes copiar el enlace que te da GitHub y pegarlo en la terminal: `git clone ENLACE_SSH`, añadir tu clave si te la pide y listo.
- **Con GitHub CLI**. Es la mejor opción, automáticamente añade una conexión entre tu repositorio y el repo original de donde hiciste el fork, permitiendo actualizar tu repo y el repo original con solo un comando. Para usar este método solo debes copiar el comando que te da GitHub en tu terminal.
### Tips:
- Si usas solo `git clone ENLACE_SSH` te descargará todo el histórico del proyecto, lo que demorará más. Pero, si usas `git clone ENLACE_SSH --depth=1` te descargará solo la ultima versión.
- Para usar el último método, GitHub CLI, primero debes haber instalado la Linea de Comandos de GitHub y haberte loggeado.
- GitHub CLI es  una forma más "simple". Una vez configuras que método usarás (HTTPS, SSH) y te loggeas obtienes automáticamente muchos pequeños detalles que de otra forma deberías configurar a mano y usando una sintaxis más legible.

