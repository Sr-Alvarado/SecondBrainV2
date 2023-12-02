---
{"dg-publish":true,"dg-path":"Colores en CSS.md","permalink":"/colores-en-css/","hide":true,"tags":["programation","CSS","DVC/RWD/2","publish","DVC/RWD/3"]}
---


[^1]: [[Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 2
[^2]: [[Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 3
[^3]: [linear-gradient() - CSS | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/gradient/linear-gradient)

- **`color` - Cambia el color a un elemento**. Propiedad que cambia el color de un elemento.
   ```CSS 
   a {
     color: black;
   }
   ```

- **`background-color` - Cambiar el color de fondo**. Esta propiedad permite cambiar añadir un color personalizado al fondo usando el nombre del color o también con la estructura RGB.
   ```CSS 
   body {
     background-color: #FFFFFF;
   }
   ```


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/responsive-web-disign/elementos-basicos-en-css/#8e818e" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **Estructura de los elementos en CSS**. La estructura de un documento CSS define a un elemento y entre `{}` las propiedades de este elemento. El valor de cada propiedad justo a continuación de `:`, y cada propiedad cerrada por `;`[^1].
   ```CSS
   element1, element2 {
     property: value;
   }
   ```
 

</div></div>


- **`border-color` - Cambiar el color del borde de una linea divisoria**. Propiedad que cambia los bordes de un elemento [[Textos en HTML#^f966d7|`<hr>`]].
   ```CSS 
   hr {
     height: 3px; /* Cambia el tamaño de la linea a 3px */
     background-color: brown; /* Cambia el color de la linea */
     border-color: brown; /* Cambia el color del borde de la linea */
   }
   ```{ #74451d}



