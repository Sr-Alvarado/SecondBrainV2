---
{"dg-publish":true,"dg-path":"Enlaces en HTML.md","permalink":"/enlaces-en-html/","hide":true,"tags":["programation","HTML","DVC/RWD/1","publish"]}
---

[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 1

- **`<a>` - Crear un enlace o link**. La etiqueta anchor define un enlace a otra página indicando la ruta con el [[Inputs/Course/Responsive Web Disign/Imágenes en HTML#^811e25\|atributo href]][^1].
   ```HTML 
   <a href="enlace.com"></a>
   ``` 
{ #1cbe87}



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/imagenes-en-html/#811e25" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **`href` - Convertir el elemento en un enlace**. El atributo hyper reference indica el link de destino. Se usa dentro de la etiqueta [[Inputs/Course/Responsive Web Disign/Enlaces en HTML#^1cbe87\|anchor]], todo lo que esté dentro será un enlace [^2].
   ```HTML
   <a href="link.com">
      <img src="rutaImagen.svg">
   </a>
   ```


</div></div>


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
> > [!info]- Code
> >```HTML
> >   <a
> >     href="https://static.vecteezy.com/system/resources/previews/015/738/191/original/choco-chips-cookies-illustration-png.png" 
> >     target="_blank"
> >   > Has click aquí para una galleta
> >   </a>
> >```