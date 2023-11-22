---
{"dg-publish":true,"dg-path":"Elementos Basicos en CSS.md","permalink":"/elementos-basicos-en-css/","hide":true,"tags":["programation","CSS","DVC/RWD/2","publish"]}
---


[^1]: [[Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 2
[^2]: [Class selectors - CSS | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Class_selectors)

- **Estructura de los elementos en CSS**. La estructura de un documento CSS define a un elemento y entre `{}` las propiedades de este elemento. El valor de cada propiedad justo a continuación de `:`, y cada propiedad cerrada por `;`[^1].
   ```CSS
   element1, element2 {
     property: value;
   }
   ```

{ #8e818e}

 
- **`<style>` - Estilos dentro de HTML**. Esta etiqueta agregada en el elemento [[Responsive Web Disign/Elementos básicos en HTML#^2d7802\|head]] permite dar estilos de diseño a la página web. Varios elementos pueden tener las mismas propiedades, solo se deben separar por una coma[^1].
   ```HTML
   <head>
      <style>
        element1, element2 {
          property: value;
        }
      </style>
   </head>
   ```{ #3fe98c}



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/responsive-web-disign/elementos-basicos-en-html/#613cad" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **Elementos y etiquetas**. Los elementos son los componentes básicos en [[Programation/HTML\|HTML]]. Las etiquetas definen el tipo de elemento[^7], su estructura es de apertura `<etiqueta>` y de cierre `</etiqueta>`[^1].
   ```html
   <etiqueta>Contenido del elemento</etiqueta> --> El conjunto reprecenta un elemento
   ```
 

</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/responsive-web-disign/elementos-basicos-en-html/#4679bb" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **Atributos o propiedades**. Son palabras especiales dentro de la etiqueta de apertura de un elemento para controlar su comportamiento definiendo funciones o valores[^1].
   ```HTML 
   <etiqueta atributo="funcion/valor">
   ```
 

</div></div>


- **`style` - Estilos en un archivo .ccs**. Se usa la misma estructura que en HTML, sin embargo ya no se usa la etiqueta `style`.
   ```CSS
   element1, element2 {
     property1: value1;
     property2: value2;
     property3: value3;
   }
   ```


- **`<link rel="stylesheet">` - Vincular CSS**. Este elemento [[Responsive Web Disign/Elementos básicos en HTML#^4af022\|self-closing tag]] permite vincular la página `.html` con el archivo de estilos `.css` donde estarán todos los estilos de la página.
   ```HTML 
   <head>
     <link rel="stylesheet" href="archivo de estilos.css">
  </head>
   ```


- **`#` - Llamar a un ID en vez de un elemento en HTML**. Si quieres modificar elementos específicos puedes usar el atributo `id` en la etiqueta HTML de apertura llamando al valor de ese ID con un `#`.
   ```HTML 
   <div id="gato">
   ```
   ```CSS 
   #gato {
     propiedad: valor;
   }
   ```

{ #1af052}

- **`/* text */` - Añadir comentarios en CSS**. Esta estructura permite añadir texto que no se tomará en cuenta para modificar la página web.
   ```CSS 
   /* Holi! Soy un comentario en CSS */
   ```

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

{ #09fbc3}



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/responsive-web-disign/elementos-basicos-en-html/#f68674" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **`class` - Añadir clases a un elemento HTML**. Atributo que agrega clases, estilos CSS, a un elemento HTML.
   ```HTML 
   <p
     class="spacious clase_2"
   >holi!</p>
   ``` 


</div></div>


- **`display: inline-block` - Hacer que varios elementos ocupen la misma linea**. La propiedad `display` con el valor `inline-block` permite que varios bloques ocupen la misma linea y solo el ancho de su contenido[^1].
   ```CSS 
   p {
     display: inline-block;
   }
   ```

