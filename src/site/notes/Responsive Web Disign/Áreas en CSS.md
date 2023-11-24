---
{"dg-publish":true,"dg-path":"Áreas en CSS.md","permalink":"/areas-en-css/","hide":true,"tags":["programation","CSS","DVC/RWD/2","publish"]}
---


[^1]: [[Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 2

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
   ```{ #a3dc50}



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/responsive-web-disign/elementos-basicos-en-css/#8e818e" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **Estructura de los elementos en CSS**. La estructura de un documento CSS define a un elemento y entre `{}` las propiedades de este elemento. El valor de cada propiedad justo a continuación de `:`, y cada propiedad cerrada por `;`[^1].
   ```CSS
   element1, element2 {
     property: value;
   }
   ```
 

</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/responsive-web-disign/textos-en-css/#993faf" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **`height` - Cambiar la altura de un elemento**. Propiedad que modifica la altura de un elemento.
   ```CSS 
   hr {
     height: 3px; /* Cambia la altura de la linea a 3px */
   }
   ```


</div></div>


- **`width` - Modificar el ancho de un elemento**. Esta propiedad modifica cuanto espacio ocupará el elemento en pantalla. Se define en pixeles `px` o en porcentaje `%`.
   ```CSS 
   #gato {
     width: 250px; /* Ocupará 250px del espacio disponible */
   }

   #perro {
     width: 80%; /* Ocupará el 80% del espacio disponible */
   }
   ```


- **`max-width` - Añadir un ancho máximo en CSS**. Propiedad que fija en un máximo el espacio que puede existir para un elemento.
   ```CSS
   #gato {
     width: 80%; /* Ocupará el 80% del espacio disponible */
     max-width: 500 px; /* Ocupará máximo 500px a pesar de que el espacio disponible es mayor */
   }
   ```



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/responsive-web-disign/elementos-basicos-en-css/#1af052" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **`#` - Llamar a un ID en vez de un elemento en HTML**. Si quieres modificar elementos específicos puedes usar el atributo `id` en la etiqueta HTML de apertura llamando al valor de ese ID con un `#`.
   ```HTML 
   <div id="gato">
   ```
   ```CSS 
   #gato {
     propiedad: valor;
   }
   ```
 

</div></div>


- **`margin-left: auto` - Añade un margen a la izquierda**. Esta propiedad con el valor `auto` añade un espacio vacío a la izquierda del elemento moviendolo todo lo posible al otro lado.
   ```CSS
   margin-left: auto;
   ```

- **`margin-right: auto` - Añade un margen a la derecha**. Esta propiedad con el valor `auto` añade un espacio vacío a la derecha del elemento moviendolo todo lo posible al otro lado.
   ```CSS
   margin-right: auto;
   ```

- **Centrar un elemento en CSS**. Se usan las 2 propiedades `margin-left` y `margin-right` lo que añade espacios a los 2 lados del elemento centrándolo.
   ```CSS 
   margin-left: auto; /* Agrega un margen a la izquierda */
   margin-right: auto; /* Agrega un margen a la derecha */
   margin-top: auto;  /* Agrega un margen arriba */
   margin-bottom: auto; /* Agrega un margen abajo */
   ```

- **`ulr()` - Agrega un enlace en CSS**. Valor que permite agregar enlaces, el enlace debe ir dentro de `()`.
   ```CSS 
   body {
     background-image: url(enlace.com);
   }
   ```

- **`padding` - Agrega espacio en los bordes a tus elementos**. Propiedad que agrega espaciado interno a los elementos[^1].
   ```CSS 
   .menu {
     padding-left: 20px; /* Agrega un espacio a la izquierda */
     padding-right: 20px; /* Agrega un espacio a la derecha */
     padding-top: 20px; /* Agrega un espacio arriba */
     padding-bottom: 20px; /* Agrega un espacio abajo */
   }
   .gato {
     padding: 20px; /* Agrega un espacio a todos los bordes */
}
   ```
