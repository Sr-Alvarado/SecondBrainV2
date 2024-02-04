---
{"dg-publish":true,"dg-path":"Elementos básicos en HTML.md","permalink":"/elementos-basicos-en-html/","hide":true,"tags":["programation","HTML","DVC/RWD/1","publish"],"created":"2024-01-25T19:06","updated":"2024-01-10T19:24"}
---

[^1]: [[Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 1
[^2]: [[Responsive Web Disign/Imágenes en HTML\|Imágenes en HTML]]
[^3]: [`<head>`: The Document Metadata (Header) element - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/head)
[^4]:[`<figure>`: The Figure with Optional Caption element - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figure)
[^5]: [[Responsive Web Disign/Formularios en HTML\|Formularios en HTML]]
[^6]: [HTML Block and Inline Elements | W3schools](https://www.w3schools.com/html/html_blocks.asp#:~:text=A%20block%2Dlevel%20element%20always%20takes%20up%20the%20full%20width,paragraph%20in%20an%20HTML%20document.)
[^7]: [Aprende HTML y CSS - Curso Desde Cero | Youtube](https://www.youtube.com/watch?v=XqFR2lqBYPs)
[^8]: [[Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 2
[^9]: [`<div>`: The Content Division element - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/div)

- **Elementos y etiquetas**. Los elementos son los componentes básicos en [[Brain/Programation/HTML\|HTML]]. Las etiquetas definen el tipo de elemento[^7], su estructura es de apertura `<etiqueta>` y de cierre `</etiqueta>`[^1].
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


- **`<meta>` - Añadir meta-información de la página**. Este elemento es un [[Responsive Web Disign/Elementos básicos en HTML#^4af022\|self-closing tag]] que permite añadir información de la página web que no están contenidos en otros elementos del HTML. Pueden haber varios, cada uno añade información diferente.

- **`<meta name="value" content="value">` - declarar el alto y el ancho**. Este atributos declaran el alto y el ancho de página en la pantalla renderizada. `name` define que se hablará del viewport y `content` define el ancho y el alto. En conjunto permiten que la página se vea similar en web y en móvil.
   ```HTML 
   <meta 
     name="viewport" 
     content="width=device-width, initial-scale=1.0" 
   /> 
   ```

- **`<meta charset="UTF-8">` - Declarar caracteres especiales**. Por defecto el navegador usa los caracteres en inglés, para declarar caracteres de otros idiomas de usa la etiqueta `meta` con el atributo `charset`.
   ```HTML
   <head>
     <meta charset="UTF-8">
   </head> 
   ```

- **`<title>` - Añadir un titulo de la pestaña**. Se usa la etiqueta `<title>` dentro del elemento `<head>`[^1]. Este elemento es usado por los buscadores para indexar tu página web[^8].
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

- **Atributos o propiedades**. Son palabras especiales dentro de la etiqueta de apertura de un elemento para controlar su comportamiento definiendo funciones o valores[^1].
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


- **`<div>` - Crea un contenedor genérico**. Elemento que crea un contenedor sin propiedades[^9]. Se usa principalmente para agregar diseños en CSS[^8].
   ```HTML 
   <div>
   </div>
   ```

- **`class` - Añadir clases a un elemento HTML**. Atributo que agrega clases, estilos CSS, a un elemento HTML.
   ```HTML 
   <p
     class="spacious clase_2" <! Este elemento tiene 2 clases >
   >holi!</p>
   ``` { #f68674}



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/responsive-web-disign/elementos-basicos-en-css/#09fbc3" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **`.class` - Agregar clases en CSS**. Para crear un elemento de tipo `class` se usa el `.` antes del elemento. De esta forma puedes usar esa clase en otros elementos CSS[^1][^2].
   ```CSS 
   /* Todos los elementos <li> con clase spacious */
   li.spacious {
     margin: 2em;
   }
   /* Todos los elementos <li> anidados en cualquier elemento con clase spacious */
   .spacious li {
     margin: 2em;
   }

   ```
 

</div></div>

