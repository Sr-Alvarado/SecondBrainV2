---
{"dg-publish":true,"permalink":"/inputs/course/responsive-web-disign/imagenes-en-html/","tags":["programation","HTML","FreeCodeCamp"]}
---

[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]]
[^2]: [[Inputs/Course/Responsive Web Disign/Enlaces en HTML\|Enlaces en HTML]]
[^3]: [[Inputs/Course/Responsive Web Disign/HTML Basics\|HTML Basics]]

- **Añadir una imagen**. Se usa la etiqueta `<img>`, esta es una *self-closing tag*[^1].
   ```HTML 
   <img>
   ```
- **Llamar una imagen externa**. Para llamar a un elemento externo se usa el atributo `src` (sourse) y se debe igualar (=) a la URL donde se localiza entre comillas (")[^1].
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
>   <figure><img src="rutaImagen.png" alt="texto por si no carga"><figcaption>Descripción de la imagen</figcaption></figure>