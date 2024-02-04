---
{"dg-publish":true,"dg-path":"Representar colores en CSS.md","permalink":"/representar-colores-en-css/","hide":true,"tags":["programation","CSS","publish","DVC/RWD/3"],"created":"2024-01-25T19:06","updated":"2023-12-02T12:47"}
---


[^1]: [[Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 3

- **Añadir un color RGB**. Se usa la función `rgb(0, 0, 0)`[^2]. Se usan valores desde `0` a `255` para definir colores en [[RGB\|RGB]], también se pueden usar `%`.
   ```CSS 
   .one {
     background-color: rgb(0, 255, 0);
   }
   ```

- **`#` - Añadir colores en RGB**. Otra forma de representar los colores RGB es a través de su notación hexadecimal (1-9, A-F), un `#` seguido de 6 dígitos `#00FF00`, cada 2 dígitos representar a un color primario y van en orden ascendente, el `#000000` es black y el `#FFFFFF` es white.
   ```CSS 
   .one {
     background-color: #00FF00; /* Color rojo puro */
   }
   ```

- **`hsl(360,%,%)` - Modelo HSL**. Modelo de matiz, saturación y luminosidad.
   - El **matiz** es representado por un circulo donde el rojo es `0` grados el verde es `120` grados y el azul es `240` grados. Los otros colores están entre estos puntos.
   - La **saturación** representa la transparencia del elemento y se mide en `%`, en `0%` el elemento es transparente, y en `100%` el color es puro.
   - La **luminosidad** representa la luz y se mide en `%`, en `0%` el elemento es completamente negro, en `50%` el color es puro y en `100%` el color es blanco.
   ```CSS 
   .blue {
     background-color: hsl(240,100%,50%); /* Representa un color azul puro */
   }
   ```

- 