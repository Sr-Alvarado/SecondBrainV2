---
{"dg-publish":true,"permalink":"/inputs/course/responsive-web-disign/imagenes-en-html/","tags":["programation","HTML","DVC/RWD/1"]}
---

[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]]
[^2]: [[Inputs/Course/Responsive Web Disign/Enlaces en HTML\|Enlaces en HTML]]
[^3]: [[Inputs/Course/Responsive Web Disign/HTML Basics\|HTML Basics]]

- **Añadir una imagen**. Se usa la etiqueta `<img>`, esta es una [[Inputs/Course/Responsive Web Disign/HTML Basics#^4af022\|self-closing tag]][^1].
   ```HTML 
   <img>
   ```

- **Llamar una imagen externa**. Para llamar a un elemento externo se usa el [[Inputs/Course/Responsive Web Disign/HTML Basics#^4679bb\|atributo]] `src` (sourse) y se iguala a la URL[^1].
   ```HTML 
   <img src="Ruta-imagen.svg">
   ```

- **Texto alternativo en imágenes**. Se usa el atributo `alt` si la imagen no carga, debe describir lo que se aprecia en la imagen[^1].
   ```HTML 
   <img src="Ruta-imagen.svg" alt="descripción de la imagen">
   ```
- **Convertir una imagen en un enlace**. Se envuelve al tag `<img>` con el elemento `<a>` con el el atributo `href`[^2] para que cada ves que se haga click en la imagen te dirija a un enlace externo[^1].
   ```HTML
   <a href="link.com"><img src="rutaImagen.svg"></a>
   ```

- **Añadir una descripción a la imagen**. Primero se anida el elemento `<img>` dentro de un tag `<figure>`[^3].  Dentro de la etiqueta `<figure>` agregamos la etiqueta `<figcaption>` para colocar una descripción de la imagen[^1].
   ```HTML 
   <figure>
     <img src="rutaImagen.svg" alt="texto por si no carga">
     <figcaption>Descripción de la imagen</figcaption>
   </figure>
   ```

> [!example]-
>   <figure><img src="https://img.wattpad.com/6eeff06ff69d65913865d96078c2ddbbe3b2f6f6/68747470733a2f2f73332e616d617a6f6e6177732e636f6d2f776174747061642d6d656469612d736572766963652f53746f7279496d6167652f6158557859636c656d59624f73413d3d2d3337333835393532392e313461343434363232383366663432393530383333353638363634372e6a7067?s=fit&w=720&h=720" alt="Meme sobre un alumno que tuvo solo unos momentos para corregir su trabajo"><figcaption>Meme sobre un alumno que tuvo solo unos momentos para corregir su trabajo</figcaption></figure>