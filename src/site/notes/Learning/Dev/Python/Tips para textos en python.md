---
{"dg-publish":true,"dg-path":"Dev/Python/Tips para textos en python.md","permalink":"/dev/python/tips-para-textos-en-python/","created":"2024-09-20T20:01","updated":"2024-09-20T20:29"}
---

## Unir varias lineas en una sola usando  `\`
Si tienes un texto muy largo que, para poder verlo completo, cortas en varias lineas pero sabes que es una sola línea puedes usar `\`, este símbolo le indicará a python que las líneas son en realidad una sola línea. Ejemplo:

```py
texto = """\
Este es un texto realmente largo\
por lo que para poder verlo a simple\
vista debo cortarlo en varias lineas\
"""

print(texto)
```

Imprime:
```bash
Este es un texto realmente largo por lo que para poder verlo a simple vista debo cortarlo en varias lineas
```

Si fuiste listo, notaste que al principio y al final del string también coloqué una `\`, lo que hace la barra invertida es unir la linea actual con la siguiente línea. Coloqué la `\` al principio y al final para que al imprimir no me diera una linea vacía antes y después del texto.

# Eliminar las sangrías extra
En python el espaciado es muy importante, es una solución elegante para identificar a simple vista la jerarquía. Sin embargo al usar textos puede generar que obtengamos textos con sangrías innecesarias. Es por ello que haciendo uso del módulo interno de python `textwrap` podemos eliminar las sangrías extra. Ejemplo:

```py
from textwrap import dedent

texto = dedent("""\
           Este es un texto realmente largo
           por lo que para poder verlo a simple
           vista debo cortarlo en varias lineas\
        """)

print(texto)
```

Imprime:
```bash
Este es un texto realmente largo
por lo que para poder verlo a simple
vista debo cortarlo en varias lineas
```

