---
{"dg-publish":true,"permalink":"/inputs/course/responsive-web-disign/botones-en-html/","tags":["programation","HTML","DVC/RWD/1"]}
---

[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 1
[^2]: [[Inputs/Course/Responsive Web Disign/Formularios en HTML#^d6e3f2\|Añadir un formulario]]
[^3]: [[Inputs/Course/Responsive Web Disign/Elementos básicos en HTML\|Elementos básicos en HTML]]
[^4]: [Input type ="radio" - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/radio)
[^5]: [<label>: The Label element - HTML: HyperText Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/label)
[^6]:[Formularios HTML](https://www.aprenderaprogramar.com/index.php?option=com_content&view=article&id=520:formularios-html-form-label-name-value-id-ejemplos-checkbox-option-button-combobox-cu00720b&catid=69&Itemid=192)

- **`<button>` - Añadir un botón simple**. La etiqueta `button` añade una casilla clickable. Si no se define atributos por defecto este envía la información al atributo `action` del formulario[^1][^2]. Los elementos `button` e `input` son elementos [[Inputs/Course/Responsive Web Disign/Elementos básicos en HTML#^31cf25\|inline]][^3].
  ```HTML 
  <button>Nombre</button>
   ```



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/formularios-en-html/#568b7f" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **`action` - Ruta destino de los datos**. Para indicar la ubicación URL[^2] a donde se enviará los datos del formulario se usa el [[Inputs/Course/Responsive Web Disign/Elementos básicos en HTML#^4679bb\|atributo]] `action`[^1]. Si no se especifica, la página donde está el formulario se recargará con los datos del formulario[^3].
  ```HTML 
  <form action="URL.com"></form>
   ``` 


</div></div>




<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/elementos-basicos-en-html/#31cf25" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **Inline elements**. Son elementos que se muestran juntos en la página a pesar de que en el código aparezcan uno debajo del otro[^5].
 

</div></div>



- **`type="sumit"` - Enviar información del form**. La función `"sumit"` especifica la acción que cumplirá el botón. Se define en el atributo `type` dentro de la etiqueta `<button>`[^1].
  ```HTML 
  <button type="submit">Nombre</button>
   ```

- **`type="chekbox"` - Añadir un botón checkbox**. La función `checkbox` se representa como una caja marcable, generalmente se usa para seleccionar más de una opción[^1]. Se define en el atributo `type` dentro la etiqueta `<input>`[^1].
  ```HTML 
  <input type="checkbox">
   ```

- **`<label>` - Añadir una etiqueta**. La etiqueta `<label>` asocia un texto con un `<input>`, al clickar el texto se seleccionará el elemento `<input>`. Para una asociación implícita[^5] se anida el `<input>` dentro de la etiqueta `<label>`[^1].
  ```HTML 
  <label>
    Opción
    <input type="radio">
  </label>
   ```

- **`name` - Agrupar inputs**. El atributo `name` se usa para identificar un grupo de control[^6]. En un `radio button` permite seleccionar solo uno, todos los `<input>` a agrupar deben tener el mismo `name`.
  ```HTML 
  <label>
    Opción
    <input type="radio" name="grupo1">
  </label>
   ```

- **`type="radio"` - Añadir un botón de radio**. La función `"radio"` define un circulo pequeño y clickable, generalmente se usa en [[Inputs/Course/Responsive Web Disign/Formularios en HTML#^0e7928\| grupos fieldsed]] para seleccionar un solo botón a mismo tiempo[^4]. Se define en el atributo `type` dentro de la etiqueta `<input>`[^1].
  ```HTML 
  <input type="radio">
   ```

{ #08712f}



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/formularios-en-html/#0e7928" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



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
   ``` 


</div></div>




<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/formularios-en-html/#34f042" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **`value` - Asignar un valor un campo seleccionable**. El atributo `value` declara que valor se enviará. En un [[Inputs/Course/Responsive Web Disign/Botones en HTML#^08712f\|radio button]] los datos dependen del `name` y del `value`, si no se define el `value` el formulario enviará `nombre=on`. Por conveniencia se usa el mismo nombre del `id`[^1].
  ```HTML 
  <form action="URL.com">
    <input type="radio" name="grupo1" id="opcion 1" value="opcion 1" required>
  </form>
   ``` 


</div></div>



> [!Example]-
> sdsd