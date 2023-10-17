---
{"dg-publish":true,"permalink":"/inputs/course/responsive-web-disign/enlaces-en-html/","tags":["programation","HTML","DVC/RWD/1"]}
---

[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 1

- **`<a>` - Crear un enlace o link**. La etiqueta anchor define un enlace a otra página indicando la ruta con el [[Inputs/Course/Responsive Web Disign/Imágenes en HTML#^7d2cf2\|atributo href]][^1].
   ```HTML 
   <a href="enlace.com"></a>
   ``` { #1cbe87}


-  **Enlaces en textos**. Se coloca entre la etiqueta `<a>` envolviendo al texto[^1].
   ```HTML 
   <a href="enlace.com">Texto del enlace</a>
   ```

- **Enlaces dentro de párrafos**. Se añade la etiqueta `<a>` a la parte que quieras convertir en enlace[^1].
   ```HTML 
   <p>Este es un texto con un <a href="enlace.com">link</a> dentro del texto</p>
   ```

- **`target` - Definir donde abrir enlace**. Para definir si quieres que se abra el enlace en una nueva pestaña puedes usar el atributo `target` con el valor `_blank`[^1].
   ```HTML 
   <a href="enlace.com" target="_blank">Texto del enlace</a>
   ```

> [!example]-
> <a href="https://static.vecteezy.com/system/resources/previews/015/738/191/original/choco-chips-cookies-illustration-png.png" target="_blank">Has click aquí para una galleta</a>