---
{"dg-publish":true,"permalink":"/learning/dev/git/buenas-practicas-para-mensajes-de-commits-en-git/","created":"2024-12-10T13:32","updated":"2024-12-10T14:27"}
---

## Resumen
- [[Learning/Dev/Git/Buenas prácticas para mensajes de commits en Git#Escríbelo en inglés\|#Escríbelo en inglés]]. Hazlo mas accesible para todos sin importar el idioma.
- [[Learning/Dev/Git/Buenas prácticas para mensajes de commits en Git#Máximo 50 caracteres\|#Máximo 50 caracteres]]. Permite que se vea bien en diferentes visualizadores.
- [[Learning/Dev/Git/Buenas prácticas para mensajes de commits en Git#Comienza con el verbo\|#Comienza con el verbo]]. Ve directo a la acción realizada.
- [[Learning/Dev/Git/Buenas prácticas para mensajes de commits en Git#Usa el modo imperativo\|#Usa el modo imperativo]]. Es claro, formal, y directo.
- [[Learning/Dev/Git/Buenas prácticas para mensajes de commits en Git#Cambios atómicos\|#Cambios atómicos]]. Solo un cambio por commit.

## Buenas practicas
### Escríbelo en inglés
El inglés es el idioma internacional por excelencia, y en programación esto es doblemente cierto, sin importar el idioma nativo de cada programador, todos debemos en algún momento toparnos con el inglés. Cada commit que hagas es mejor escribirlo en inglés.

### Máximo 50 caracteres
En general los commits son vistos por diferentes personas en diferentes entornos, al escribir mensajes muy largos, en algunos entornos, dificulta la correcta visualización del mensaje. Es una buena practica limitar el mensaje a 50 caracteres, garantiza que el mensaje se pueda ver bien en diferentes entornos.

### Comienza con el verbo
Un buen mensaje siempre comienza con el verbo, va directo a la acción, lo que hayas hecho. Ejemplo: modificar, implementar, arreglar, resolver, etc.

### Usa el modo imperativo
En pocas palabras, el modo imperativo es, hablar de forma directa y en segunda persona para describir el cambio hecho, para este caso creo que es mejor explicar con ejemplos:
- Add user authentication module
- Implement search functionality
- Fix login form validation issue
- Resolve typo in README.md
- Optimize image loading performance
- Add usage examples for CLI tool

### Cambios atómicos
Este es un consejo mas para tus commits que para los mensajes con los que los guardas, pero es un muy buen consejo así que va. Si tu mensaje tiene que explicar mas de un cambio, es decir, hay mas de un verbo, ese commit esta mal, en ves de uno deberían ser dos commits. Recuerda que por buena practica se debe hacer un commit por cada cambio.