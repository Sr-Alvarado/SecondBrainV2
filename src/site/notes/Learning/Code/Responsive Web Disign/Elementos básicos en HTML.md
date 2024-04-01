---
{"dg-publish":true,"dg-path":"Code/Responsive Web Disign/Elementos básicos en HTML.md","permalink":"/code/responsive-web-disign/elementos-basicos-en-html/","tags":["programation","HTML"],"created":"2024-01-25T19:06","updated":"2024-03-31T23:29"}
---


> [!info]-
>> [!cite]+ Fuentes y enlaces relacionados
>> - [[Learning/Code/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 1
>> - [[Learning/Code/Responsive Web Disign/Imágenes en HTML\|Imágenes en HTML]]
>> - [`<head>`: The Document Metadata (Header) element - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/head)
>> - [`<figure>`: The Figure with Optional Caption element - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figure)
>> - [[Learning/Code/Responsive Web Disign/Formularios en HTML\|Formularios en HTML]]
>> - [HTML Block and Inline Elements | W3schools](https://www.w3schools.com/html/html_blocks.asp#:~:text=A%20block%2Dlevel%20element%20always%20takes%20up%20the%20full%20width,paragraph%20in%20an%20HTML%20document.)
>> - [Aprende HTML y CSS - Curso Desde Cero | Youtube](https://www.youtube.com/watch?v=XqFR2lqBYPs)
>> - [[Learning/Code/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 2
>> - [`<div>`: The Content Division element - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/div)


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/elementos-y-etiquetas-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Los elementos son los componentes básicos en [[Learning/Wiki/HTML\|HTML]]. Las etiquetas definen el tipo de elemento[^7], su estructura es de apertura `<etiqueta>` y de cierre `</etiqueta>`[^1].
```html
<etiqueta>Contenido del elemento</etiqueta> --> El conjunto reprecenta un elemento
```
 

</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/self-closing-tag-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Son etiquetas que no necesitan otra etiqueta de cierre[^1]. Estas etiquetas representan el segundo tipo de elementos en [[Learning/Wiki/HTML\|HTML]], elementos reemplazables por otro contenido al ser remplazados no necesitan contenido interno por tanto no usan etiquetas internas.
```HTML
<selftag src="">  
```
 

</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/atributos-o-propiedades-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Son palabras especiales dentro de la etiqueta de apertura de un elemento para controlar su comportamiento definiendo funciones o valores[^1].
   ```HTML 
   <etiqueta atributo="funcion/valor">
   ```
 

</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/index-nombre-del-archivo-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Es un estándar que el archivo principal de tu página web se llame `index`[^7].

</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/doctype-html-version-de-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Lo primero es informar al navegador la versión de [[Learning/Wiki/HTML\|HTML]] en que se escribió el documento[^7].
```HTML 
<!DOCTYPE html>
```


</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/html-elemento-raiz-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




La etiqueta `<html>` declara el elemento raíz del archivo, todos los demás elementos van dentro[^7].
```html
<html>
</html>
```

</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/lang-definir-el-idioma-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Para definir el idioma de una página web se usa el atributo `lang` en el elemento `<html>` y como valor el código internacional de ese idioma[^7].
```HTML 
<!DOCTYPE html>
<html lang="es">
</html>
```


</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/indentacion-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Los elementos contenidos dentro de otro (embebidos) se anidan usando 2 espacios antes de comenzar (sangría), mejora la lectura del código[^1]. Los elementos embebidos adquieren las propiedades del elemento de nivel superior.
```HTML
<body>
  <main>
  </main>
</body>
```


</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/head-metadatos-de-la-pagina-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Para indicar datos de la pág (scripts, ccs, title) que no va a ver el usuario se usa la etiqueta `head`[^3]. Si se omite, el navegador lo añadirá por defecto[^7]. ```html
<head>
</head>
```

</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/meta-anadir-meta-informacion-de-la-pagina-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Este elemento es un [[Learning/Code/Responsive Web Disign/Elementos básicos en HTML#^4af022\|self-closing tag]] que permite añadir información de la página web que no están contenidos en otros elementos del HTML. Pueden haber varios, cada uno añade información diferente.
```html
<meta />
```

</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/meta-name-value-content-value-declarar-el-alto-y-el-ancho-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Este atributos declaran el alto y el ancho de página en la pantalla renderizada. `name` define que se hablará del viewport y `content` define el ancho y el alto. En conjunto permiten que la página se vea similar en web y en móvil. 
```HTML 
<meta 
  name="viewport" 
  content="width=device-width, initial-scale=1.0" 
/> 
```


</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/meta-charset-utf-8-declarar-caracteres-especiales-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Por defecto el navegador usa los caracteres en inglés, para declarar caracteres de otros idiomas de usa la etiqueta `meta` con el atributo `charset`.
```HTML
<head>
  <meta charset="UTF-8">
</head> 
```


</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/title-anadir-un-titulo-a-una-pestana-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Se usa la etiqueta `<title>` dentro del elemento `<head>`[^1]. Este elemento es usado por los buscadores para indexar tu página web[^8].
```HTML 
<head>
  <meta charset="UTF-8">
  <title>Titulo que el navegador mostrará en la pestaña</title>
</head>
```


</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/body-cuerpo-de-la-pagina-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Todos los elementos que deben ser renderizados o mostrados en la página deben estar dentro de la etiqueta `<body>`[^1].
```HTML 
<body>
   <main>
   </main>
</body>
```
 

</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/main-cuerpo-central-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




La etiqueta `<main>` define el contenido principal del cuerpo de una página, se usa para mejorar el [[Search Engine Optimization\|posicionamiento]] en [[Buscadores web\|buscadores]][^1].
```HTML 
<main>
  <h1>Tema central</h1>
</main>
```


</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/section-sub-secciones-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




La etiqueta `<section>` define sub-secciones que se enfocan en temas específicos dentro de la sección principal `<main>`[^1].
```HTML 
<main>
  <h1>Todo sobre los gatos</h1>
  
  <section>
    <h2>Orígen de los gatos</h2>
  </section>
</main>
```


</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/figure-definir-un-bloque-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Declara que un contenido es autónomo. Todos los elementos dentro de esta etiqueta representan una sola unidad[^4]. Permite asociar imágenes con su titulo y su descripción[^2].
```HTML 
<figure>
  <img src="rutaImagen.svg" alt="texto por si no carga">
  <figcaption>Descripción de la imagen</figcaption>
</figure>
```
 

</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/inline-elements-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Son elementos que se muestran juntos en la página a pesar de que en el código aparezcan uno debajo del otro[^5].
 

</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/id-identificar-elementos-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Atributo que identifica elementos específicos, cada `id` debe tener un valor único, diferente a cualquiera de la misma página[^5].
 

</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/el-orden-de-los-atributos-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Cuando un elemento tiene multiples atributos, el orden de cada uno no es importante[^1].

</div></div>
 

<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




Agrupa los elementos embebidos en una nueva linea[^1]. Usa todo el ancho disponible, se extiende a la derecha e izquierda tanto como puede[^6].


</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/div-crea-un-contenedor-generico-en-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Elemento que crea un contenedor sin propiedades[^9]. Se usa principalmente para agregar diseños en CSS[^8].
```HTML 
<div>
</div>
```


</div></div>
 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/html-tags/class-anadir-clases-a-un-elemento-html/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Atributo que agrega clases, estilos CSS, a un elemento HTML.
```HTML 
<p
  class="spacious clase_2" <! Este elemento tiene 2 clases >
>holi!</p>
``` 


</div></div>
 