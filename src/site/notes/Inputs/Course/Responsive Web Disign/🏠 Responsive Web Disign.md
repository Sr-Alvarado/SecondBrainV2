---
{"dg-publish":true,"permalink":"/inputs/course/responsive-web-disign/responsive-web-disign/","tags":["programation","HTML","CSS"]}
---

## About
Aprenderás los lenguajes que los desarrolladores usan para construir páginas web: [[Programation/HTML\|HTML]] para el contenido, y CSS para el diseño.
## Learn HTML by Building a Cat Photo App
### HTML Basics
- **Etiquetas**. Los elementos en [[Programation/HTML\|HTML]] tienen etiquetas de apertura `<etiqueta>` y de cierre `</etiqueta>`.
   ```html
   <h1>Titulo</h1>
   ```
- **Títulos**. La etiqueta `<h>` se usa para títulos e indican importancia (1-6), a menor el número mayor importancia. Solo debe haber un `<h1>` por página.
   ```HTML 
   <h1>Titulo 1</h1>
   ⁝
   <h6>Titulo 6</h6>
   ```
- **Párrafos**. La etiqueta `<p>` se usa para definir un párrafo.
   ```HTML 
   <p>Párrafo 1</p>
   ```
- **Comentarios**. La etiqueta `<!--` define un comentario, dentro puede haber tantas lineas de texto como quieras.
   ```HTML 
   <!-- Comentarios -->
   ```
- **Sección principal**. La etiqueta `<main>` define el contenido principal del cuerpo de una página, se usa para mejorar el [[Search Engine Optimization\|posicionamiento]] en [[Buscadores web\|buscadores]].
   ```HTML 
   <main>Tema central del documento o Funcion principal de aplicación</main>
   ```
- **Indentación**. Los elementos contenidos dentro de otro se anidan usando 2 espacios antes de comenzar (sangría), se usa para mejorar la lectura del código.
   ```HTML 
   <main>
     <h1>CatPhotoApp</h1>
   </main>
   ```
- **Atributos**. Son palabras especiales en la etiqueta de apertura de un elemento para controlar su comportamiento.
- **Self-closing tag**. Son etiquetas que no necesitan otra etiqueta de cierre.
### Imágenes en HTML
- **Añadir una imagen**. Se usa la etiqueta `<img>`, esta es una *self-closing tag*.
   ```HTML 
   <img>
   ```
- **Enlazar un elemento externo**. Para llamar a un elemento externo se usa el atributo `src` y se debe igualar (=) a la URL donde se localiza entre comillas (").
   ```HTML 
   <img src="Ruta-imagen.jpg">
   ```
- **Texto alternativo en imágenes**. Se usa el atributo `alt` si la imagen no carga, debe describir lo que se aprecia en la imagen.
   ```HTML 
   <img src="Ruta-imagen.jpg" alt="descripción de la imagen">
   ```
### Enlaces en HTML
- **Enlazar con otra página**. Se define con la etiqueta `<a>` (anchor) y se usa el atributo `href` para especificar la dirección.
   ```HTML 
   <a href="enlace.com"></a>
   ```
-  **Texto de un enlace**. Se coloca entre la etiqueta anchor.
   ```HTML 
   <a href="enlace.com">Texto del enlace</a>
   ```
- **Enlaces en párrafos**. Puedes convertir cualquier texto en un enlace añadiendo la etiqueta `<a>` a la parte que quieras convertir en enlace.
   ```HTML 
   <p>Este es un texto con un <a href="enlace.com">link</a> dentro del texto</p>
   ```
- **Definir donde abrir enlace**. Para definir si quieres que se abra el enlace en una nueva pestaña puedes usar el atributo `target` con el valor `_blank`
   ```HTML 
   <a href="enlace.com" target="_blank">Texto del enlace</a>
   ```