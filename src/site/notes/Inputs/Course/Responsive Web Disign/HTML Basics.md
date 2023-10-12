---
{"dg-publish":true,"permalink":"/inputs/course/responsive-web-disign/html-basics/","tags":["programation","HTML","DVC/RWD/1"]}
---

[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 1
[^2]: [[Inputs/Course/Responsive Web Disign/Imágenes en HTML\|Imágenes en HTML]]
[^3]: [head: The Document Metadata (Header) element - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/head)

- **Etiquetas**. Los elementos en [[Programation/HTML\|HTML]] tienen etiquetas de apertura `<etiqueta>` y de cierre `</etiqueta>`[^1].
   ```html
   <etiqueta>Texto</etiqueta>
   ```

{ #613cad}

- **Indentación**. Los elementos contenidos dentro de otro (embebidos) se anidan usando 2 espacios antes de comenzar (sangría), se usa para mejorar la lectura del código[^1]. Los elementos embebidos adquieren las propiedades del elemento de nivel superior.
   ```HTML 
   <body>
     <main>
     </main>
   </body>
   ```

- **`<head>` - Metadatos de la página**. Para indicar datos de la pág (scripts, ccs, title) que no debería ver el usuario se usa la etiqueta `head`[^3].

{ #2d7802}

- **`<title>` - Añadir un titulo de la pestaña**. Se usa la etiqueta `<title>` dentro del elemento `<head>`.
  ```HTML 
  <head>
    <title>Titulo que el navegador mostrará en la pestaña</title>
  </head>
  ```

- **`<body>` - Cuerpo de la página**. Todos los elementos que deben ser renderizados o mostrados en la página deben estar en el elemento `<body>`[^1].
  ```HTML 
  <body>
     <main>
     </main>
  </body>
   ```

{ #02db07}

- **`<main>` - Sección principal**. La etiqueta `<main>` define el contenido principal del cuerpo de una página, se usa para mejorar el [[Search Engine Optimization\|posicionamiento]] en [[Buscadores web\|buscadores]][^1].
   ```HTML 
   <main>
     <h1>Tema central</h1>
   </main>
   ```

- **`<section>` - Sub-secciones**. La etiqueta `<section>` define sub-secciones que se enfocan en temas específicos dentro de la sección principal `<main>`[^1].
   ```HTML 
   <main>
     <h1>Todo sobre los gatos</h1>
     
     <section>
       <h2>Orígen de los gatos</h2>
     </section>
   </main>
   ```

- **Self-closing tag**. Son etiquetas que no necesitan otra etiqueta de cierre[^1].

{ #4af022}

- **Atributos**. Son palabras especiales en la etiqueta de apertura de un elemento para controlar su comportamiento[^1].
   ```HTML 
   <etiqueta atributo="valor">
   ```

{ #4679bb}

- **Elemento Figure**. Declara que un contenido es autónomo. Todos los elementos dentro de esta etiqueta representan una sola unidad. Permite asociar imágenes un titulo y una descripción[^2].
  ```HTML 
  
   ```

- **Inline elements**. Son elementos que aparecen juntos en la página a pesar de añadir cada uno en una nueva linea[^1].

- **Id attribute**. Identifica elementos HTML específicos, cada `id` debe tener un valor único, diferente a cualquiera de la misma página[^1].

- **Orden de los atributos**. Cuando un elemento tiene multiples atributos, el orden de cada uno no es importante[^1].

- **Block-level elements**. Agrupa los elementos anidados dentro en una nueva linea.

