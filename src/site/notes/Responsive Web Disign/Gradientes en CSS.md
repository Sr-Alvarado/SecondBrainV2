---
{"dg-publish":true,"dg-path":"Gradientes en CSS.md","permalink":"/gradientes-en-css/","hide":true,"tags":["programation","CSS","publish","DVC/RWD/3"],"created":"2024-01-25T19:06","updated":"2023-12-02T12:49"}
---


[^1]: [[Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 3
[^2]: 
[^3]: [linear-gradient() - CSS | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/gradient/linear-gradient)

- **`linear-gradient` - Añadir un gradiente de colores**. Valor que añade un gradiente lineal entre varios colores a un elemento. Se usa dentro de la propiedad `background`. 
   ```CSS 
   h1{
     background: linear-gradient(blue, red); /* Degradado de azul a rojo */
   }
   ```

- **Indicar la dirección del gradiente**. Se agrega la propiedad `gradientDirection` con el valor: `deg` grados, `in oklab` interpretación rectangular, `in hsl` interpolación polar[^3]. Si no se agrega por defecto usará 180 grados o de arriba a abajo.
   ```CSS 
   h1{
     background: linear-gradient(to left top, blue, red); /* Degradado de azul a rojo la esquina inferior derecha hacia la esquina superior izquierda */
   ```

- **Especificar el espacio que ocupara cada color.** Puedes añadir un `color-stop` o porcentaje de espacio que ocupará un color puro en el degradado con un `%` al lado del color.
   ```CSS 
   h1{
     background: linear-gradient(to left top, blue 10%, red); /* Degradado de azul ocupando el 10% del espacio a rojo ocupando el resto desde la esquina inferior derecha hacia la esquina superior izquierda */
   ```