---
{"dg-publish":true,"dg-path":"Bordes en CSS.md","permalink":"/bordes-en-css/","hide":true,"tags":["programation","CSS","publish","DVC/RWD/3"],"created":"2024-01-25T19:06","updated":"2023-12-02T13:41"}
---


[^1]: [[Responsive Web Disign/Responsive Web Disign\|Responsive Web Disign]] - Cap 3

- **`border` - Añade un borde**. Propiedad que permite añadir un espacio bordeando el elemento, por defecto a todos lados, puede especificar que lado.
   ```CSS 
   .perro {
     border-left-width: 10px; /* Añade un borde izquiero de 10px */
     border-right-width: 5px; /* Añade un borde derecho de 5px */
    }
   .gato {
     border-width: 10px; /* Añade bordes de 10px a todos los lados */
   }
   ```{ #039830}


- **`border-style` - Añade estilo al borde**. Propiedad que permite añadir un estilo `style` solido `solid`, de líneas discontinuas `dashed` o punteado `dotted` o doble linea continua`double`.
   ```CSS 
   .perro {
     border-style: solid; /* Añade estilo sólido a todos los bordes */
    }
   .gato {
     border-top-style: solid; /* Añade estilo sólido al borde de arriba */
     border-left-style: dashed; /* Añade estilo discontínuo al borde izquierdo */
     border-bottom-style: dotted; /* Añade estilo punteado al borde de abajo */
    }
   ```

- **`border-color` - Añade un color al borde**. Propiedad que agrega un color a un borde.
   ```CSS 
   .perro {
     border-color: white; /* Añade un color blanco a todos los bordes */
    }
   .gato {
     border-bottom-color: black; /* Añade un color negro al borde inferior */
    }
   ```{ #59b6e7}


- **`border-_lado_` - Editar todas las propiedades de un lado**. Propiedad que permite editar todas las propiedades de un borde de un lado `width style color`.
   ```CSS 
   .gato {
     border-left: 10px solid black; /* Agrega un borde sólido negro de 10px al lado izquierdo */
   }
   ```
- 