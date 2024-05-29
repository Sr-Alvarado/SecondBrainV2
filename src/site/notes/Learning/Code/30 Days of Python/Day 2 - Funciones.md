---
{"dg-publish":true,"dg-path":"Code/30 Days of Python/Day 2 - Funciones.md","permalink":"/code/30-days-of-python/day-2-funciones/","created":"2024-05-29T16:47","updated":"2024-05-29T18:14"}
---


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/30-days-of-python/all-verificar-si-todos-los-elementos-son-verdaderos-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Evalúa iterables, si todos los elementos son verdaderos devuelve TRUE, si uno es falso devuelve FALSE. Los elementos que se consideran FALSE son:


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/30-days-of-python/elementos-que-devuelven-false-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




- 0 --> El cero en cualquier tipo (entero, flotante y complejo)
- "" --> Cadenas vacías (strings, diccionarios, listas, tuplas, conjuntos y conjuntos inmutables)
- `None` --> El objeto None
- `bytearray(b'')` --> arreglos de bytes vacíos
- `bytes(b'')` --> secuencias de bytes vacías

</div></div>


Todo lo demás se considera TRUE.

</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/30-days-of-python/any-verificar-si-todos-los-elementos-son-falsos-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Es similar a [[Learning/Code/30 Days of Python/all() - Verificar si todos los elementos son verdaderos en Python\|all()]], cuando alguno es verdadero devuelve TRUE cuando todos son falsos devuelve FALSE.

- [[Learning/Code/30 Days of Python/Elementos que devuelven FALSE en python\|Elementos que devuelven FALSE en python]]

</div></div>
 


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/30-days-of-python/int-convertir-a-numeros-enteros/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Antes de hacer operaciones aritméticas con números debemos asegurarnos que el tipo de dato es numérico de contrario dará ERROR. Para convertir un string con un número en un tipo entero usamos:
```py
z = "2hola"
a = "10"
b = 9.8
c = 1 + 1j

print(int(z))   #ERROR
print(int(a))   #10
print(int(b))   #9
print(int(c))   #ERROR
```
- Puede convertir strings si solo contienen números.
- En caso de números reales solo devuelve la parte entera.
- No puede convertir números complejos.

</div></div>
 


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/30-days-of-python/list-tranforma-elementos-a-una-lista/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




```py
first_name = "Asab"

print(list(first_name))    #["A","s","a","b"]
```
- Si le das un string devolverá la cadena de texto separada en elementos de letras.

</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/30-days-of-python/sistemas-numericos-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Para identificar que un número está en un sistema numérico o en otro Python usa prefijos, los más comunes son:
- `0b11` --> 3 en **Binario** (0b)
- `0o10` --> 8 en **Octal** (0o)
- `0xA2` --> 162 en **Hexadecimal** (0x)
- `10` --> 10 en **Decimal**, los decimales no tienen prefijo

</div></div>
 


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/30-days-of-python/help-obtener-informacion-sobre-alguna-funcion-integrada-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Esta función permite obtener información, al estilo del `--help` en Linux, sobre las funciones core de python.

</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/30-days-of-python/nombres-de-variables-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




```py
capitales_latam = ["Lima","Bogotá","Santiago de Chile","Buenos Aires","Caracas"]
```


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/30-days-of-python/nombrar-variables/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




```bh
a = 2
```
- Una única cadena de texto, si quieres separar palabras usa `_` guiones bajos.
- El nombre debe ser muy descriptivo, mientras más detallado mejor, pero no te pases.
- El primer carácter debe ser una letra.
- Las mayúsculas importan: `variable` y `Variable` se reconocen como diferentes.

</div></div>

- El nombre también puede comenzar con `_`.
- Puede tener caracteres alfanuméricos (`A-z`, `0-9` y `_`)
- Usa `_` para separar palabras
- Se recomienda dejar todas las variables en minúsculas

</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/30-days-of-python/declarar-varias-variables-en-una-sola-linea-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Solo alinea el nombre y el valor:
```py
first_name, last_name, country, age, is_married = 'Asabeneh', 'Yetayeh', 'Helsink', 250, True
```
- El primer elemento `first_name` se asigna al primer valor `Asabeneh`
- El segundo elemento `last_name` se asigna al segundo valor `Yetayeh`
- Y así con todos los elementos.
- Debe haber el mismo número de variables y de valores, de lo contrario, no se hará la asignación.

</div></div>

