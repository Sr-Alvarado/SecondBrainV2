---
{"dg-publish":true,"dg-path":"Opacidad en CSS.md","permalink":"/opacidad-en-css/","hide":true,"tags":["programation","CSS","publish","DVC/RWD/3"],"created":"2024-01-25T19:06","updated":"2023-12-02T13:06"}
---


[^1]: [[Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 3

- **`opacity` - Definir la opacidad de un elemento**. Propiedad que define la opacidad o transparencia de un elemento, 0 es completamente transparente y 1 es completamente opaco, es decir el color se muestra tal como es.
   ```CSS 
   .sleeve {
     background-color: white;
     opacity: 0.5;
   }
   ```

- **`alpha channel` - Otra forma de añadir opacidad**. Alternativamente puede usar la propiedad alpha channel, esta forma se usa con las [[Responsive Web Disign/Representar colores  en CSS\|funciones de color]] (RGB, HSL, HEX). Agrega una `a` al final de cada función de color y un nuevo valor (0 - 1.0) al final de los atributos.
   ```CSS
   .sleeve {
     width: 110px;
     height: 25px;
     background-color: rgba(255, 255, 255, 0.5); /* Agrega un color RGB blanco con opacidad al 50% */
   }
   ```

