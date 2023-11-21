---
{"dg-publish":true,"dg-path":"Area de un elemento en CSS.md","permalink":"/area-de-un-elemento-en-css/","hide":true,"tags":["programation","CSS","DVC/RWD/2","publish"]}
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
   ```


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/responsive-web-disign/elementos-basicos-en-css/#8e818e" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **Estructura de los elementos en CSS**. La estructura de un documento CSS define a un elemento y entre `{}` las propiedades de este elemento. El valor de cada propiedad justo a continuación de `:`, y cada propiedad cerrada por `;`[^1].
   ```CSS
   element1, element2 {
     property: value;
   }
   ```
 

</div></div>


- **`width` - Modificar el ancho de un elemento**. Esta propiedad modifica cuanto espacio ocupará el elemento en pantalla. Se define en pixeles `px` o en porcentaje `%`.
   ```CSS 
   #gato {
     width: 250px;
   }

   #perro {
     width: 80%;
   }
   ``` 

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
   margin-left: auto;
   margin-right: auto;
   ```