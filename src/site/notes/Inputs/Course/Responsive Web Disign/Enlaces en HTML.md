---
{"dg-publish":true,"permalink":"/inputs/course/responsive-web-disign/enlaces-en-html/","tags":["programation","HTML","DVC/RWD/1"]}
---

[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]]

- **`<a>` - Enlazar con otra página**. Para crear un enlace a otra página se usa la etiqueta `<a>` (anchor) con el [[Inputs/Course/Responsive Web Disign/Imágenes en HTML#^7d2cf2\|atributo href]] para especificar la dirección[^1].
   ```HTML 
   <a href="enlace.com"></a>
   ``` { #1cbe87}

-  **Enlaces en textos**. Se coloca entre la etiqueta anchor[^1].
   ```HTML 
   <a href="enlace.com">Texto del enlace</a>
   ```

- **Enlaces dentro de párrafos**. Puedes convertir cualquier texto en un enlace añadiendo la etiqueta `<a>` a la parte que quieras convertir en enlace[^1].
   ```HTML 
   <p>Este es un texto con un <a href="enlace.com">link</a> dentro del texto</p>
   ```

- **Definir donde abrir enlace**. Para definir si quieres que se abra el enlace en una nueva pestaña puedes usar el atributo `target` con el valor `_blank`[^1].
   ```HTML 
   <a href="enlace.com" target="_blank">Texto del enlace</a>
   ```
