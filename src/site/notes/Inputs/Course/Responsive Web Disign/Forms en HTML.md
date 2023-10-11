---
{"dg-publish":true,"permalink":"/inputs/course/responsive-web-disign/forms-en-html/","tags":["programation","HTML"]}
---

[^1]: [[Inputs/Course/Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]]
[^2]: [Mi primer formulario HTML - MDN](https://developer.mozilla.org/es/docs/Learn/Forms/Your_first_form) 
[^3]: [Atributos de formularios en HTML - Universidad de Murcia](https://www.um.es/docencia/barzana/DAWEB/Formularios-HTML5.html)
[^4]: [[Inputs/Course/Responsive Web Disign/HTML Basics\|HTML Basics]]
[^5]: [input - HTML: Lenguaje de etiquetas de hipertexto | MDN](https://developer.mozilla.org/es/docs/Web/HTML/Element/input)

- **Añadir un formulario**. Se usa la etiqueta `<form>` para declarar un formulario[^1].
  ```HTML 
  <form></form>
   ```
- **Atributo action**. Indica la ubicación URL[^2] donde deben enviarse los datos del formulario[^1], si permanece vacío la página que contiene al formulario se recargará con los datos de este[^3].
  ```HTML 
  <form action="URL.com"></form>
   ```
- **Elemento Input**. Es una Self-Closing tag[^4] que permite recolectar datos de un form[^1], a través de la creación de controles interactivos para recibir los datos[^5].
  ```HTML 
  <form action="URL.com">
    <input>
  </form>
   ```
- **Definir el input**. Para definir el tipo de input que se desea usar se usa el tributo  `type`[^1], su valor predeterminado es `"text"` si no se especifica[^5].
  ```HTML 
  <form action="URL.com">
    <input type="text">
  </form>
   ```
- **Colocar un nombre al input**. Define un nombre al input[^1], este será enviado con los datos del formulario[^5].
  ```HTML 
  <form action="URL.com">
    <input type="text" name="Titulo">
  </form>
   ```
- **Atributo Placeholder**. Da una pista de que elementos deben ir en el form[^1], no debe contener saltos de linea, hay veces en que no es visible[^5].
  ```HTML 
  <form action="URL.com">
    <input type="text" name="Titulo" placeholder="Email address">
  </form>
   ```
- **Hacer obligatorio un campo**. Se usa el atributo `required` para especificar que el usuario debe llenar el campo si desea enviar el form[^5]. Este atributo no necesita ningún valor[^1].
  ```HTML 
  <form action="URL.com">
    <input type="text" name="Titulo" placeholder="Email address"     required>
  </form>
   ```
- **Agrupar elementos input - `<fieldset>` element**. Para agrupar elementos input relacionados se usa la etiqueta `<fieldset>`[^1], que es una block-level element[^3].
  ```HTML 
  <fieldset>
    <label> Opción 1
      <input type="radio" name="grupo1" id="Opcion 1" value="Opcion 1">
    </label>
    <label> Opción 2
      <input type="radio" name="grupo1" id="Opcion 2" value="Opcion 2">
    </label>
  </fieldset>
   ```
- **Legend element**. Declara una descripción del elemento `<fieldset>`. Da contexto a los usuarios sobre que datos ingresar en el form[^1].
  ```HTML 
  <fieldset>
    <legend>¿Qué opción prefieres?</legend>
    <label> Opción 1
      <input type="radio" name="grupo1" id="Opcion 1" value="Opcion 1">
    </label>
    <label> Opción 2
      <input type="radio" name="grupo1" id="Opcion 2" value="Opcion 2">
    </label>
  </fieldset>
   ```
- 