---
{"dg-publish":true,"dg-path":"Formularios en HTML.md","permalink":"/formularios-en-html/","hide":true,"tags":["programation","HTML","DVC/RWD/1","publish"]}
---

[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 1
[^2]: [Mi primer formulario HTML | MDN](https://developer.mozilla.org/es/docs/Learn/Forms/Your_first_form) 
[^3]: [Atributos de formularios en HTML | Universidad de Murcia](https://www.um.es/docencia/barzana/DAWEB/Formularios-HTML5.html)
[^4]: [[Inputs/Course/Responsive Web Disign/Elementos básicos en HTML\|Elementos básicos en HTML]]
[^5]: [`<input>` - HTML | MDN](https://developer.mozilla.org/es/docs/Web/HTML/Element/input)

- **`<form>` - Añadir un formulario**. Se usa la etiqueta `<form>` para declarar un formulario[^1].
  ```HTML 
  <form></form>
   ```

{ #d6e3f2}


- **`action` - Ruta destino de los datos**. Para indicar la ubicación URL[^2] a donde se enviará los datos del formulario se usa el [[Inputs/Course/Responsive Web Disign/Elementos básicos en HTML#^4679bb\|atributo]] `action`[^1]. Si no se especifica, la página donde está el formulario se recargará con los datos del formulario[^3].
  ```HTML 
  <form action="URL.com"></form>
   ``` { #568b7f}



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/elementos-basicos-en-html/#4679bb" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **Atributos**. Son palabras especiales dentro de la etiqueta de apertura de un elemento para controlar su comportamiento[^1].
   ```HTML 
   <etiqueta atributo="funcion/valor">
   ```
 

</div></div>



- **`<input>` - Recolectar los datos**. [[Inputs/Course/Responsive Web Disign/Elementos básicos en HTML#^4af022\|Self-Closing tag]] que permite recolectar datos de un formulario[^1], a través de la creación de controles interactivos para recibir los datos[^5].
  ```HTML 
  <form action="URL.com">
    <input>
  </form>
   ```



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/elementos-basicos-en-html/#4af022" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **Self-closing tag**. Son etiquetas que no necesitan otra etiqueta de cierre[^1]. Estas etiquetas representan el segundo tipo de elementos en HTML, elementos reemplazables por otro contenido al ser remplazados no necesitan contenido interno por tanto no usan etiquetas internas.
   ```HTML
   <selftag src="">  
   ```
 

</div></div>



- **`type` - Definir el input**. El atributo  `type` define el tipo de dato que se debe llenar[^1]. Si no se especifica su valor predeterminado es `"text"`[^5].
  ```HTML 
  <form action="URL.com">
    <input type="text">
  </form>
   ```

- **`name` - Poner nombre al input**. El atributo `name`[^1] define el título con el que se envían con los datos del formulario[^5].
  ```HTML 
  <form action="URL.com">
    <input type="text" name="Titulo">
  </form>
   ```

- **`placeholder` - Dar una pista del campo**.  El atributo `placeholder` indica al usuario que elementos pide el formulario[^1]. No debe contener saltos de linea, veces no es visible[^5].
  ```HTML 
  <form action="URL.com">
    <input type="text" name="Titulo" placeholder="Email address">
  </form>
   ```

- **`required` - Hacer obligatorio un campo**. El atributo `required` especifica al usuario campos obligatorios del formulario[^5]. No necesita ningún valor[^1].
  ```HTML 
  <form action="URL.com">
    <input type="text" name="Titulo" placeholder="Email address"     required>
  </form>
   ```

- **`value` - Asignar un valor un campo seleccionable**. El atributo `value` declara que valor se enviará. En un [[Inputs/Course/Responsive Web Disign/Botones en HTML#^08712f\|radio button]] los datos dependen del `name` y del `value`, si no se define el `value` el formulario enviará `nombre=on`. Por conveniencia se usa el mismo nombre del `id`[^1].
  ```HTML 
  <form action="URL.com">
    <input type="radio" name="grupo1" id="opcion 1" value="opcion 1" required>
  </form>
   ``` { #34f042}



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/botones-en-html/#08712f" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **`type="radio"` - Añadir un botón de radio**. La función `"radio"` define un circulo pequeño y clickable, generalmente se usa en [[Inputs/Course/Responsive Web Disign/Formularios en HTML#^0e7928\| grupos fieldsed]] para seleccionar un solo botón a mismo tiempo[^4]. Se define en el atributo `type` dentro de la etiqueta `<input>`[^1].
  ```HTML 
  <input type="radio">
   ```
 

</div></div>




<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/elementos-basicos-en-html/#37ea09" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **`id` - Identificar elementos**. Atributo que identifica elementos específicos, cada `id` debe tener un valor único, diferente a cualquiera de la misma página[^5].
 

</div></div>



- **`<fieldset>` - Agrupar elementos**. La etiqueta `<fieldsed>` agrupar elementos `<input>`[^1] en una [[Inputs/Course/Responsive Web Disign/Elementos básicos en HTML#^28750b\|block-level element]].
  ```HTML 
  <fieldset>
    <label> 
      <input type="radio" name="grupo1" id="Opcion 1" value="Opcion 1">
      Opción 1
    </label>
    <label>
      <input type="radio" name="grupo1" id="Opcion 2" value="Opcion 2">
      Opción 2
    </label>
  </fieldset>
   ``` { #0e7928}



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/elementos-basicos-en-html/#28750b" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **Block-level elements**. Agrupa los elementos embebidos en una nueva linea[^1]. Usa todo el ancho disponible, se extiende a la derecha e izquierda tanto como puede[^6]. 

</div></div>



- **`<legend>` - Añade una descripción**. La etiqueta `<legend>` declara una descripción del grupo `<fieldset>`. Da contexto a los usuarios sobre que datos ingresar[^1].
  ```HTML 
  <fieldset>
    <legend>¿Qué opción prefieres?</legend>
    <label>
      <input type="radio" name="grupo1" id="Opcion 1" value="Opcion 1">
      Opción 1
    </label>
    <label>
      <input type="radio" name="grupo1" id="Opcion 2" value="Opcion 2">
      Opción 2
    </label>
  </fieldset>
   ```


> [!example]- 
> 
> <fieldset>
>    <legend>¿Quieres salir conmigo?</legend>
>    <label>
>       <input type="radio" name="cita" id="si" value="Si">
>       Si
>    </label>
>    <label>
>       <input type="radio" name="cita" id="obvio" value="Obvio">
>       Obvio
>    </label>
>    <label>
>       <input type="radio" name="cita" id="porsupuesto" value="Por supuesto">
>       Por supuesto
>    </label>
> </fieldset>
> 
> > [!info]- Código
> > ```
> > <fieldset>
> >    <legend>¿Quieres salir conmigo?</legend>
> >    <label>
> >       <input type="radio" name="cita" id="si" value="Si">
> >       Si
> >    </label>
> >    <label>
> >       <input type="radio" name="cita" id="obvio" value="Obvio">
> >       Obvio
> >    </label>
> >    <label>
> >       <input type="radio" name="cita" id="porsupuesto" value="Por supuesto">
> >       Por supuesto
> >    </label>
> > </fieldset>
> > ```
