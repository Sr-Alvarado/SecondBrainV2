---
{"dg-publish":true,"dg-path":"Dev/Python/Slicing en Python.md","permalink":"/dev/python/slicing-en-python/","created":"2024-09-13T16:12","updated":"2024-09-13T16:28"}
---

Es un método en Python que permite cortar partes de una cadena. Es válido para secuencias ordenadas como [[cadena\|cadena]]s, [[Lista\|Lista]]s, [[tupla\|tupla]]s, y [[array\|array]]s. La sintaxis es: `[inicio:fin:paso]`. Donde:
- `inicio`. Posición inicial, desde donde comenzará el corte. Si está vacío comienza desde el primer elemento.
- `fin`. Posición final, hasta donde se cortará. Si está vacío termina en el último elemento.
- `paso`. Cantidad de caracteres a saltar. Si es positivo salta a la derecha, si es negativo salta a la izquierda. (Cuando no se especifica es 1, corta saltando del 1 al 2 al 3...)

Ejemplo:
```py
text = "Hola Mundo!"

sort_firt_4_elements = text[4:]                # Devuelve: " Mundo!"
sort_last_4_elements = text[:4]                # Devuelve: "Hola Mu"
sort_middle_elements = text[2:6]               # Devuelve: "la Mun"
sort_jump_2_elements = text[::2]               # Devuelve: "Hl ud!"
sort_jump__negative_2_elements = text[::-1]    # Devuelve: "!odnuM aloH"
```