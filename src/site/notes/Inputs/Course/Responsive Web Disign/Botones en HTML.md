---
{"dg-publish":true,"permalink":"/inputs/course/responsive-web-disign/botones-en-html/","tags":["programation","HTML","DVC/RWD/1"]}
---

[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]]
[^2]: [[Inputs/Course/Responsive Web Disign/Formularios en HTML#^d6e3f2\|Añadir un formulario]]
[^3]: [[Inputs/Course/Responsive Web Disign/Elementos básicos en HTML\|Elementos básicos en HTML]]
[^4]: [Input type ="radio" - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/radio)
[^5]: [<label>: The Label element - HTML: HyperText Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/label)
[^6]:[Formularios HTML](https://www.aprenderaprogramar.com/index.php?option=com_content&view=article&id=520:formularios-html-form-label-name-value-id-ejemplos-checkbox-option-button-combobox-cu00720b&catid=69&Itemid=192)

- **Añadir un botón simple**. Para añadir un botón se usa la etiqueta `button`, si no se definen atributos para el botón predeterminadamente este envía la información al atributo `action` del formulario[^1][^2]. Los elementos `button` y `input` son elementos *inline*[^3].
  ```HTML 
  <button>Nombre</button>
   ```
- **Función enviar información del form**. A pesar de que por defecto el botón cumpla esta función, lo correcto es especificar la acción que cumplirá en botón con el atributo `type` en el valor `submit`[^1].
  ```HTML 
  <button type="submit">Nombre</button>
   ```

- **Botón de radio**. Se representa como un circulo pequeño que puede rellenar, generalmente se usan en grupos de radios `<fieldset>` donde solo se puede seleccionar un botón a mismo tiempo[^4]. Se usan dentro de una etiqueta `<input>`[^1].
  ```HTML 
  <input type="radio">
   ```

{ #08712f}

- **Botón de checkbox**. Se representa como una caja que puedes marcar, por lo general se usan para marcar más de una opción[^1]. Se usan dentro de una etiqueta `<input>`[^1].
  ```HTML 
  <input type="checkbox">
   ```
- **Elemento label**. Asocia un texto con un `<input>`, al clickar en el texto se seleccionará el elemento `<input>`. Para una asociación implícita[^5] se anida el `<input>` dentro de la etiqueta `<label>`[^1].
  ```HTML 
  <label>
    Opción
    <input type="radio">
  </label>
   ```
- **Selección única en radio button - Name attribute** #Mejorar_Idea. Para que cuando se seleccione un botón radio se deseleccione los otros,  todos deben tener el mismo atributo `name`, que identifica un grupo de control[^6].
  ```HTML 
  <label>
    Opción
    <input type="radio" name="grupo1">
  </label>
   ```


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/inputs/course/responsive-web-disign/formularios-en-html/#34f042" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



- **`value` - Asignar un valor un campo seleccionable**. Este atributo declara que valor debe enviarse. En un [[Inputs/Course/Responsive Web Disign/Botones en HTML#^08712f\|radio button]] los datos se que se envían dependen del `name` y del `value`, si no se define un `value` el formulario enviará `nombre=on`. Por conveniencia se usa el mismo nombre del `id`[^1].
  ```HTML 
  <form action="URL.com">
    <input type="radio" name="grupo1" id="opcion 1" value="opcion 1" required>
  </form>
   ``` 


</div></div>
