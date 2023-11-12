---
{"dg-publish":true,"dg-path":"Imágenes en HTML.md","permalink":"/imagenes-en-html/","hide":true,"tags":["programation","HTML","DVC/RWD/1","publish"]}
---

[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 1
[^2]: [[Inputs/Course/Responsive Web Disign/Enlaces en HTML\|Enlaces en HTML]]
[^3]: [[HTML Basics\|HTML Basics]]
[^4]:[`<figure>`: The Figure with Optional Caption element - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figure)

- **`<img>` - Añadir una imagen**. Se usa la etiqueta `<img>`, esta es una [[Inputs/Course/Responsive Web Disign/Elementos básicos en HTML#^4af022\|self-closing tag]][^1].
   ```HTML 
   <img>
   ```



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/elementos-basicos-en-html/#4af022" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **Self-closing tag**. Son etiquetas que no necesitan otra etiqueta de cierre[^1]. Estas etiquetas representan el segundo tipo de elementos en HTML, elementos reemplazables por otro contenido al ser remplazados no necesitan contenido interno por tanto no usan etiquetas internas.
   ```HTML
   <selftag src="">  
   ```
 

</div></div>



- **`src` - Origen de la imagen**. Para llamar a la fuente de un elemento se usa el [[Inputs/Course/Responsive Web Disign/Elementos básicos en HTML#^4679bb\|atributo]] sourse y se iguala a la URL (ruta interna o externa)[^1].
   ```HTML 
   <img src="Ruta-imagen.svg">
   ```



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/elementos-basicos-en-html/#4679bb" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **Atributos**. Son palabras especiales dentro de la etiqueta de apertura de un elemento para controlar su comportamiento[^1].
   ```HTML 
   <etiqueta atributo="funcion/valor">
   ```
 

</div></div>



- **`alt` - Texto alternativo en imágenes**. El atributo `alt` se usa para mostrar una descripción de la imagen si esta no carga, debe describir lo que se ve en la imagen[^1].
   ```HTML 
   <img src="Ruta-imagen.svg" alt="descripción de la imagen">
   ```

- **`href` - Convertir el elemento en un enlace**. El atributo hyper reference indica el link de destino. Se usa dentro de la etiqueta [[Inputs/Course/Responsive Web Disign/Enlaces en HTML#^1cbe87\|anchor]], todo lo que esté dentro será un enlace [^2].
   ```HTML
   <a href="link.com">
      <img src="rutaImagen.svg">
   </a>
   ``` { #811e25}



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/enlaces-en-html/#1cbe87" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **`<a>` - Crear un enlace o link**. La etiqueta anchor define un enlace a otra página indicando la ruta con el [[Inputs/Course/Responsive Web Disign/Imágenes en HTML#^811e25\|atributo href]][^1].
   ```HTML 
   <a href="enlace.com"></a>
   ``` 


</div></div>



- **`<figcaption>` - Añadir una descripción a la imagen**. Se anida el elemento `<img>` dentro de la [[Inputs/Course/Responsive Web Disign/Elementos básicos en HTML#^179304\|etiqueta figure]] (`<figure>`), allí se agrega la etiqueta `<figcaption>` para definir la descripción de la imagen[^1], se recomienda que sea la misma del texto alternativo[^4].
   ```HTML 
   <figure>
     <img src="rutaImagen.svg" alt="texto por si no carga">
     <figcaption>Descripción de la imagen</figcaption>
   </figure>
   ```



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/elementos-basicos-en-html/#179304" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **`<figure>` - Definir un bloque**. Declara que un contenido es autónomo. Todos los elementos dentro de esta etiqueta representan una sola unidad[^4]. Permite asociar imágenes con su titulo y su descripción[^2].
   ```HTML 
  <figure>
     <img src="rutaImagen.svg" alt="texto por si no carga">
     <figcaption>Descripción de la imagen</figcaption>
   </figure>
   ```
 

</div></div>


> [!example]-
> <figure><a href="https://img.wattpad.com/6eeff06ff69d65913865d96078c2ddbbe3b2f6f6/68747470733a2f2f73332e616d617a6f6e6177732e636f6d2f776174747061642d6d656469612d736572766963652f53746f7279496d6167652f6158557859636c656d59624f73413d3d2d3337333835393532392e313461343434363232383366663432393530383333353638363634372e6a7067?s=fit&w=720&h=720" target="_blank"><img src="https://img.wattpad.com/6eeff06ff69d65913865d96078c2ddbbe3b2f6f6/68747470733a2f2f73332e616d617a6f6e6177732e636f6d2f776174747061642d6d656469612d736572766963652f53746f7279496d6167652f6158557859636c656d59624f73413d3d2d3337333835393532392e313461343434363232383366663432393530383333353638363634372e6a7067?s=fit&w=720&h=720" alt="Meme de un alumno que tuvo poco tiempo para corregir su proyecto"></a><figcaption>Meme de un alumno que tuvo poco tiempo para corregir su proyecto. <a href="https://www.wattpad.com/373859529-memes-de-programacion-%C2%A9-0101" target="_blank">Fuente</a></figcaption></figure>