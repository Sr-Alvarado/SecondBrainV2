---
{"dg-publish":true,"dg-path":"Textos en HTML.md","permalink":"/textos-en-html/","hide":true,"tags":["programation","HTML","DVC/RWD/1","publish"]}
---

[^1]: [[Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 1

- **`<h>` - Añadir títulos**. Los headers indican importancia (1-6), a menor el número mayor importancia. Solo debe haber un `<h1>` por página[^1].
   ```HTML 
   <h1>Titulo 1</h1>
   ⁝
   <h6>Titulo 6</h6>
   ```

- **`<p>` - Añadir párrafos**. La etiqueta `<p>` se usa para definir un párrafo[^1].
   ```HTML 
   <p>Párrafo 1</p>
   ```

- **`<!--` - Añadir comentarios**. La etiqueta `<!--` define un comentario, dentro puede haber tantas lineas de texto como quieras[^1].
   ```HTML 
   <!-- Comentarios -->
   ```

- **`<strong>` - Letra negrita**. Para indicar importancia o urgencia una parte de un texto podemos usar la etiqueta `<strong>`[^1].
   ```HTML
   <p>Los gatos <strong>aman</strong> la leche</p>
   ```
  
- **`<em>` - Letra cursiva**. Para enfatizar una parte de un texto podemos usar la etiqueta `<em>`[^1].
   ```HTML
   <p>Los gatos <em>aman</em> la leche</p>
   ```

- **`<footer>` - Añadir un pie de página**. Se usa la etiqueta `<footer>` para definir un pie de página[^1].
   ```HTML 
   <footer></footer>
   ```

> [!example]-
> <h1>Quisque ut dolor gravida, placerat libero vel, euismod.</h1>
> <p>Plura mihi bona sunt, inclinet, amari petere vellent. Ab illo tempore, ab est sed immemorabili. Ullamco <strong>texto con más importancia</strong> ex ea commodi consequat. Quae vero auctorem tractata ab fiducia dicuntur. At nos hinc posthac, sitientis piros Afros.</p><p>Petierunt uti sibi concilium totius <em>texto enfatizado</em> certam indicere. Morbi fringilla convallis sapien, id pulvinar odio volutpat. A communi observantia non est recedendum.</p><footer>Pie de página: Inmensae subtilitatis, obscuris et malesuada fames.</footer>
> 
> > [!info]- Code
> >```HTML
> >   <h1>
> >     Quisque ut dolor gravida, placerat libero vel, euismod.
> >   </h1>
> >   <p>
> >     Plura mihi bona sunt, inclinet, amari petere vellent. Ab illo tempore, ab est sed immemorabili. Ullamco 
> >     <strong>
> >       texto con más importancia
> >     </strong> 
> >     ex ea commodi consequat. Quae vero auctorem tractata ab fiducia dicuntur. At nos hinc posthac, sitientis piros Afros.
> >   </p>
> >   <p>
> >     Petierunt uti sibi concilium totius 
> >     <em>
> >       texto enfatizado
> >     </em> 
> >     certam indicere. Morbi fringilla convallis sapien, id pulvinar odio volutpat. A communi observantia non est recedendum.
> >   </p>
> >   <footer>
> >     Pie de página: Inmensae subtilitatis, obscuris et malesuada fames.
> >   </footer>
> >```