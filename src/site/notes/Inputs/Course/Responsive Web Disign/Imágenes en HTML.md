---
{"dg-publish":true,"permalink":"/inputs/course/responsive-web-disign/imagenes-en-html/","tags":["programation","HTML","DVC/RWD/1"]}
---

[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]]
[^2]: [[Inputs/Course/Responsive Web Disign/Enlaces en HTML\|Enlaces en HTML]]
[^3]: [[Inputs/Course/Responsive Web Disign/HTML Basics\|HTML Basics]]
[^4]:[`<figure>`: The Figure with Optional Caption element - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figure)

- **`<img>` - Añadir una imagen**. Se usa la etiqueta `<img>`, esta es una [[Inputs/Course/Responsive Web Disign/HTML Basics#^4af022\|self-closing tag]][^1].
   ```HTML 
   <img>
   ```

- **`sourse` - Llamar una imagen externa**. Para llamar a un elemento externo se usa el [[Inputs/Course/Responsive Web Disign/HTML Basics#^4679bb\|atributo]] `src` (sourse) y se iguala a la URL (ruta interna o externa)[^1].
   ```HTML 
   <img src="Ruta-imagen.svg">
   ```

- **`alt` - Texto alternativo en imágenes**. Se usa el atributo `alt` que se muestra si la imagen no carga, debe describir lo que se aprecia en la imagen[^1].
   ```HTML 
   <img src="Ruta-imagen.svg" alt="descripción de la imagen">
   ```

- **`href` - Convertir el elemento en un enlace**. Se embebe la etiqueta `<img>` en un [[Inputs/Course/Responsive Web Disign/Enlaces en HTML#^1cbe87\|elemento anchor]] (`<a>`) con el el atributo `href`[^2]. Cada ves que se haga click en la imagen se dirigirá al enlace especificado[^1].
   ```HTML
   <a href="link.com"><img src="rutaImagen.svg"></a>
   ```

{ #7d2cf2}

- **`<figcaption>` - Añadir una descripción a la imagen**. Se anida el elemento `<img>` dentro de un [[Inputs/Course/Responsive Web Disign/HTML Basics#^179304\|elemento figure]] (`<figure>`).  Dentro agregamos la etiqueta `<figcaption>` para colocar una descripción de la imagen[^1], se recomienda que sea la misma del texto alternativo[^4].
   ```HTML 
   <figure>
     <img src="rutaImagen.svg" alt="texto por si no carga">
     <figcaption>Descripción de la imagen</figcaption>
   </figure>
   ```

> [!example]-
>   <figure><img src="https://img.wattpad.com/6eeff06ff69d65913865d96078c2ddbbe3b2f6f6/68747470733a2f2f73332e616d617a6f6e6177732e636f6d2f776174747061642d6d656469612d736572766963652f53746f7279496d6167652f6158557859636c656d59624f73413d3d2d3337333835393532392e313461343434363232383366663432393530383333353638363634372e6a7067?s=fit&w=720&h=720" alt="Meme de un alumno que tuvo poco tiempo para corregir su proyecto"><figcaption>Meme de un alumno que tuvo poco tiempo para corregir su proyecto. <a href="https://www.wattpad.com/373859529-memes-de-programacion-%C2%A9-0101">Fuente</a>.</figcaption></figure>
