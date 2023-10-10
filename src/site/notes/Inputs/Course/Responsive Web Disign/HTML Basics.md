---
{"dg-publish":true,"permalink":"/inputs/course/responsive-web-disign/html-basics/","tags":["programation","HTML","FreeCodeCamp"]}
---

[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]]
[^2]: [[Inputs/Course/Responsive Web Disign/Imágenes en HTML\|Imágenes en HTML]]

- **Etiquetas**. Los elementos en [[Programation/HTML\|HTML]] tienen etiquetas de apertura `<etiqueta>` y de cierre `</etiqueta>`[^1].
   ```html
   <h1>Titulo</h1>
   ```
- **Títulos**. La etiqueta `<h>` se usa para títulos e indican importancia (1-6), a menor el número mayor importancia. Solo debe haber un `<h1>` por página[^1].
   ```HTML 
   <h1>Titulo 1</h1>
   ⁝
   <h6>Titulo 6</h6>
   ```
- **Párrafos**. La etiqueta `<p>` se usa para definir un párrafo[^1].
   ```HTML 
   <p>Párrafo 1</p>
   ```
- **Comentarios**. La etiqueta `<!--` define un comentario, dentro puede haber tantas lineas de texto como quieras[^1].
   ```HTML 
   <!-- Comentarios -->
   ```
- **Sección principal**. La etiqueta `<main>` define el contenido principal del cuerpo de una página, se usa para mejorar el [[Search Engine Optimization\|posicionamiento]] en [[Buscadores web\|buscadores]][^1].
   ```HTML 
   <main>
     <h1>Tema central</h1>
   </main>
   ```
- **Sub-secciones**. La etiqueta `<section>` define sub-secciones que se enfocan en temas específicos dentro de la sección principal (`<main>`)[^1].
   ```HTML 
   <main>
     <h1>Todo sobre los gatos</h1>
     
     <section>
       <h2>Orígen de los gatos</h2>
     </section>
   </main>
   ```
> [!example]-
>   <main><h1>Todo sobre los gatos</h1><section><h2>Orígen de los gatos</h2></section></main>
- **Indentación**. Los elementos contenidos dentro de otro se anidan usando 2 espacios antes de comenzar (sangría), se usa para mejorar la lectura del código[^1].
   ```HTML 
   <main>
     <h1>CatPhotoApp</h1>
   </main>
   ```
 > [!example]-
>   <main><h1>CatPhotoApp</h1></main>
- **Atributos**. Son palabras especiales en la etiqueta de apertura de un elemento para controlar su comportamiento[^1].
- **Self-closing tag**. Son etiquetas que no necesitan otra etiqueta de cierre[^1].
- **Elemento Figure**. Declara que un contenido es independiente de toda la estructura. Permite asociar una imagen con una descripción[^2].
- **Enfatizar un texto**. Para destacar una parte de un texto podemos usar la etiqueta `<em>`[^1].
  ```HTML 
<p>Los gatos <em>aman</em> la leche</p>
  ```
> [!example]-
> <p>Los gatos <em>aman</em> la leche</p>

- **Indicar importancia de un texto**. Para indicar importancia o urgencia una parte de un texto podemos usar la etiqueta `<strong>`[^1].
  ```HTML 
<p>Los gatos <strong>aman</strong> la leche</p>
  ```
> [!example]-
> <p>Los gatos <strong>aman</strong> la leche</p>