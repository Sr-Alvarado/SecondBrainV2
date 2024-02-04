---
{"dg-publish":true,"dg-path":"Listas en HTML.md","permalink":"/listas-en-html/","hide":true,"tags":["programation","HTML","DVC/RWD/1","publish"],"created":"2024-01-25T19:06","updated":"2024-01-10T19:24"}
---

[^1]: [[Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 1

- **`<ul>` - Lista desordenada**. Los elementos se separan por guiones. Se usa la etiqueta `<ul>` (Unordered List) para definir una lista desordenada[^1].
   ```HTML 
   <ul></ul>
   ```

- **`<ol>` - Lista ordenada**. Los elementos se enumeran. Se usa la etiqueta `<ol>` (Order List) para definir una lista desordenada[^1].
   ```HTML 
   <ul></ul>
   ```

- **`<li>` - Añadir items a una lista**. Se anida la etiqueta `<li>` (List Item) dentro de la etiqueta `<ul>`[^1].
   ```HTML 
   <ul>
     <li>Item 1</li>
     ⁝
     <li>Item n</li>
   </ul>
   ```

> [!example]-
> <h3>Lista desordenada</h3>
>   <ul><li>Item 1</li><li>Item 2</li><li>Item 3</li></ul>
> <h3>Lista ordenada</h3>
>   <ol><li>Item 1</li><li>Item 2</li><li>Item 3</li></ol>
> 
> > [!info]- Código
> > ```html
> > <h3>Lista desordenada</h3>
> >    <ul>
> >       <li>Item 1</li>
> >       <li>Item 2</li>
> >       <li>Item 3</li>
> >    </ul>
> > <h3>Lista ordenada</h3>
> >    <ol>
> >       <li>Item 1</li>
> >       <li>Item 2</li>
> >       <li>Item 3</li>
> >    </ol>
> > ```
