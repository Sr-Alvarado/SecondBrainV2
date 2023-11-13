---
{"dg-publish":true,"dg-path":"Elementos Basicos en CSS.md","permalink":"/elementos-basicos-en-css/","hide":true,"tags":["programation","CSS","DVC/RWD/2","publish"]}
---


[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 2

- **`<style>` - Estilos dentro de HTML**. Esta etiqueta agregada en el elemento [[Inputs/Course/Responsive Web Disign/Elementos básicos en HTML#^2d7802\|head]] permite dar estilos de diseño a la página web. Varios elementos pueden tener las mismas propiedades, solo se deben separar por una coma[^1].
   ```HTML
   <!DOCTYPE html>
   <html lang="en">
     <head>
       <style>
         element1, element2 {
           property: value;
         }
       </style>
     </head>
   </html>
   ```


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/elementos-basicos-en-html/#613cad" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **Elementos y etiquetas**. Los elementos son los componentes básicos en [[Programation/HTML\|HTML]]. Las etiquetas definen el tipo de elemento[^7], su estructura es de apertura `<etiqueta>` y de cierre `</etiqueta>`[^1].
   ```html
   <etiqueta>Contenido del elemento</etiqueta> --> El conjunto reprecenta un elemento
   ```
 

</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/elementos-basicos-en-html/#4679bb" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **Atributos o propiedades**. Son palabras especiales dentro de la etiqueta de apertura de un elemento para controlar su comportamiento definiendo funciones o valores[^1].
   ```HTML 
   <etiqueta atributo="funcion/valor">
   ```
 

</div></div>


- **`style` - Estilos en un archivo .ccs**. Se usa la misma estructura que en HTML, sin embargo la etiqueta `style` ya no necesita ir dentro de `<>`.
   ```CSS
   style
         element1, element2 {
           property: value;
         }
   /style
   ```


- **`<link rel="stylesheet">` - Vincular CSS**. Este elemento [[Inputs/Course/Responsive Web Disign/Elementos básicos en HTML#^4af022\|self-closing tag]] permite vincular la página `.html` con el archivo de estilos `.css` donde estarán todos los estilos de la página.
   ```HTML 
   <head>
     <link rel="stylesheet" href="archivo de estilos.css">
  </head>
   ```


- Paso 17