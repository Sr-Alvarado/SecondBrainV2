---
{"dg-publish":true,"permalink":"/inputs/course/responsive-web-disign/botones-en-html/","tags":["programation","HTML"]}
---

[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]]
[^2]: [[Inputs/Course/Responsive Web Disign/Forms en HTML\|Forms en HTML]]
[^3]: [[Inputs/Course/Responsive Web Disign/HTML Basics\|HTML Basics]]
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
- **Definir valores - Value attribute**. Si seleccionas el radio button y envías el formulario, los datos del radio button se basarán en sus atributos `name` y `value`, cuando los radio button no tienen el atributo `value`, los datos del formulario tomarán la forma del `name` `name del grupo=on`, para enviar un dato exacto se usa el atributo `value`, por conveniencia se le coloca el mismo nombre que el `id`[^1][^3].
  ```HTML 
  <label> Opción 1
    <input type="radio" name="grupo1" id="Opcion 1" value="Opcion 1">
  </label>
  <label> Opción 2
    <input type="radio" name="grupo1" id="Opcion 2" value="Opcion 2">
  </label>
   ```
