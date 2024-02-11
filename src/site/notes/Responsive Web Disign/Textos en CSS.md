---
{"dg-publish":true,"dg-path":"Textos en CSS.md","permalink":"/textos-en-css/","hide":true,"tags":["programation","CSS","DVC/RWD/2","publish"],"created":"2024-01-25T19:06","updated":"2023-11-24T16:41"}
---


[^1]: [[Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 2


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/responsive-web-disign/areas-en-css/#a3dc50" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **`text-align:` - Alinear un texto**. Propiedad que permite alinear un texto a la derecha, centrarlo o a la izquierda especificando en el valor[^1].
   ```HTML 
   <style>
      h1, h2, h3 {
        text-align: center;
      }
      h5, h6 {
        text-align: right;
      }
      p {
        text-align: left;
      }
    </style>
   ```


</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/responsive-web-disign/elementos-basicos-en-css/#8e818e" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **Estructura de los elementos en CSS**. La estructura de un documento CSS define a un elemento y entre `{}` las propiedades de este elemento. El valor de cada propiedad justo a continuación de `:`, y cada propiedad cerrada por `;`[^1].
   ```CSS
   element1, element2 {
     property: value;
   }
   ```
 

</div></div>


- **`font-family` - Cambia la fuente de un texto en CSS**. Propiedad que permite cambiar la tipografía de un texto.
   ```CSS 
   #perro {
   fond-family: sans-serif;
   }
   ```

- **Añade una fuente de respaldo**. Valor que añade una fuente extra que solo será usada si la fuente principal no se puede aplicar. Se añade la fuente al lado de la principal separada por una coma.
   ```CSS 
   h2 {
     fond-family: Impact, serif; /* Se usará la fuente Impact, en caso de no estar disponible se aplicará serif*/
   }
   ```

- **`font-size` - Cambia el tamaño de un texto**. Propiedad que modifica el tamaño de la letra de un texto usando valores establecidos en px.
   ```CSS 
   h2 {
     fond-family: Impact, serif; /* Se usará la fuente Impact, en caso de no estar disponible se aplicará serif*/
     fond-size: 40px; /* El tamaño de la letra será de 40px */
   }
   ```

- **`height` - Cambiar la altura de un elemento**. Propiedad que modifica la altura de un elemento.
   ```CSS 
   hr {
     height: 3px; /* Cambia la altura de la linea a 3px */
   }
   ```{ #993faf}




<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/responsive-web-disign/colores-en-css/#74451d" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **`border-color` - Cambiar el color del borde de una linea divisoria**. Propiedad que cambia los bordes de un elemento [[Textos en HTML#^f966d7|`<hr>`]].
   ```CSS 
   hr {
     height: 3px; /* Cambia el tamaño de la linea a 3px */
     background-color: brown; /* Cambia el color de la linea */
     border-color: brown; /* Cambia el color del borde de la linea */
   }
   ```


</div></div>


