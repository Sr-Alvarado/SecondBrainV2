---
{"dg-publish":true,"dg-path":"Elementos básicos en HTML.md","permalink":"/elementos-basicos-en-html/","hide":true,"tags":["programation","HTML","DVC/RWD/1","publish"]}
---

[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 1
[^2]: [[Inputs/Course/Responsive Web Disign/Imágenes en HTML\|Imágenes en HTML]]
[^3]: [`<head>`: The Document Metadata (Header) element - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/head)
[^4]:[`<figure>`: The Figure with Optional Caption element - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figure)
[^5]: [[Inputs/Course/Responsive Web Disign/Formularios en HTML\|Formularios en HTML]]
[^6]: [HTML Block and Inline Elements | W3schools](https://www.w3schools.com/html/html_blocks.asp#:~:text=A%20block%2Dlevel%20element%20always%20takes%20up%20the%20full%20width,paragraph%20in%20an%20HTML%20document.)
[^7]: [Aprende HTML y CSS - Curso Desde Cero | Youtube](https://www.youtube.com/watch?v=XqFR2lqBYPs)

- **Elementos y etiquetas**. Los elementos son los componentes básicos en [[Programation/HTML\|HTML]]. Las etiquetas definen el tipo de elemento[^7], su estructura es de apertura `<etiqueta>` y de cierre `</etiqueta>`[^1].
   ```html
   <etiqueta>Contenido del elemento</etiqueta> --> El conjunto reprecenta un elemento
   ```

{ #613cad}

 
- **Self-closing tag**. Son etiquetas que no necesitan otra etiqueta de cierre[^1]. Estas etiquetas representan el segundo tipo de elementos en HTML, elementos reemplazables por otro contenido al ser remplazados no necesitan contenido interno por tanto no usan etiquetas internas.
   ```HTML
   <selftag src="">  
   ```

{ #4af022}

 
- **`index.html` - Nombre del archivo**. Es un estándar que el archivo principal de tu página web se llame `index`[^7].

- **`<!DOCTYPE html>` - Versión de HTML**. Lo primero es informar al navegador la versión de HTML en que se escribió el documento[^7].
   ```HTML 
   <!DOCTYPE html>
   ```

- **`<html>` - Elemento raíz**. La etiqueta `<html>` declara el elemento raíz del archivo, todos los demás elementos van dentro[^7].

- **`lang="es"` - Definir el idioma**. Para definir el idioma de una página web se usa el atributo `lang` en el elemento `<html>` y como valor el código internacional de ese idioma[^7].
   ```HTML 
   <!DOCTYPE html>
   <html lang="es">
   </html>
   ```

- **Indentación**. Los elementos contenidos dentro de otro (embebidos) se anidan usando 2 espacios antes de comenzar (sangría), mejora la lectura del código[^1]. Los elementos embebidos adquieren las propiedades del elemento de nivel superior.
   ```HTML
   <body>
     <main>
     </main>
   </body>
   ```

- **`<head>` - Metadatos de la página**. Para indicar datos de la pág (scripts, ccs, title) que no va a ver el usuario se usa la etiqueta `head`[^3]. Si se omite, el navegador lo añadirá por defecto[^7].

{ #2d7802}


- **`<meta charset="UTF-8">` - Declarar caracteres especiales**. Por defecto el navegador usa los caracteres en inglés, para declarar caracteres de otros idiomas de usa la etiqueta `meta` con el atributo `charset`.
   ```HTML
   <head>
     <meta charset="UTF-8">
   </head> 
   ```

- **`<title>` - Añadir un titulo de la pestaña**. Se usa la etiqueta `<title>` dentro del elemento `<head>`.
   ```HTML 
   <head>
     <meta charset="UTF-8">
     <title>Titulo que el navegador mostrará en la pestaña</title>
   </head>
   ```

- **`<body>` - Cuerpo de la página**. Todos los elementos que deben ser renderizados o mostrados en la página deben estar dentro de la etiqueta `<body>`[^1].
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

- **Atributos**. Son palabras especiales dentro de la etiqueta de apertura de un elemento para controlar su comportamiento[^1].
   ```HTML 
   <etiqueta atributo="funcion/valor">
   ```

{ #4679bb}

- **`<figure>` - Definir un bloque**. Declara que un contenido es autónomo. Todos los elementos dentro de esta etiqueta representan una sola unidad[^4]. Permite asociar imágenes con su titulo y su descripción[^2].
   ```HTML 
   <figure>
     <img src="rutaImagen.svg" alt="texto por si no carga">
     <figcaption>Descripción de la imagen</figcaption>
   </figure>
   ```

{ #179304}

- **Inline elements**. Son elementos que se muestran juntos en la página a pesar de que en el código aparezcan uno debajo del otro[^5].

{ #31cf25}

- **`id` - Identificar elementos**. Atributo que identifica elementos específicos, cada `id` debe tener un valor único, diferente a cualquiera de la misma página[^5].

{ #37ea09}

- **Orden de los atributos**. Cuando un elemento tiene multiples atributos, el orden de cada uno no es importante[^1].

- **Block-level elements**. Agrupa los elementos embebidos en una nueva linea[^1]. Usa todo el ancho disponible, se extiende a la derecha e izquierda tanto como puede[^6].{ #28750b}


