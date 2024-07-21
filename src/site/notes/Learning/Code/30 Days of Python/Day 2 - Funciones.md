---
{"dg-publish":true,"dg-path":"Code/30 Days of Python/Day 2 - Funciones.md","permalink":"/code/30-days-of-python/day-2-funciones/","created":"2024-05-29T16:47","updated":"2024-07-21T12:00"}
---


**| [[Learning/Code/30 Days of Python/Day 1 - Introducción\|:luc_arrow_left_circle: After day]] | [[Learning/Code/30 Days of Python/30 Days of Python\|:luc_home: Home]] | [[Learning/Code/30 Days of Python/Day 3 - Operadores en Python\|:luc_arrow_right_circle: Next day]] | [:obs_code_glyph: Ejercicios](https://github.com/Sr-Alvarado/30-Days-Of-Python-thon-solved-exercises/blob/main/02_day_variables.py) |** 

## Funciones
Python nos permite crear funciones para modificar elementos, dentro de estas existe una subclasificación, los métodos. Todos los métodos en python son funciones pero no todas las funciones son métodos, las funciones toman métodos como entrada y los métodos actúan sobre los objetos. Las funciones transforman un objeto y métodos solo brindan datos sobre ese objeto, su longitud, su tipo, el orden. Más información en [[Funciones vs métodos en Python\|Funciones vs métodos en Python]]. 

### all()

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/python/all-verificar-si-todos-los-elementos-son-verdaderos-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Evalúa iterables, si todos los elementos son verdaderos devuelve TRUE, si uno es falso devuelve FALSE. Los elementos que se consideran FALSE son:


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/python/elementos-que-devuelven-false-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




- 0 --> El cero en cualquier tipo (entero, flotante y complejo)
- "" --> Cadenas vacías (strings, diccionarios, listas, tuplas, conjuntos y conjuntos inmutables)
- `None` --> El objeto None
- `bytearray(b'')` --> arreglos de bytes vacíos
- `bytes(b'')` --> secuencias de bytes vacías

</div></div>


Todo lo demás se considera TRUE.

</div></div>


### any()

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/python/any-verificar-si-todos-los-elementos-son-falsos-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Es similar a [[Learning/Code/Python/all() - Verificar si todos los elementos son verdaderos en Python\|all()]], cuando alguno es verdadero devuelve TRUE cuando todos son falsos devuelve FALSE.

- [[Learning/Code/Python/Elementos que devuelven FALSE en python\|Elementos que devuelven FALSE en python]]

</div></div>
 
### int()

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/python/int-convertir-a-numeros-enteros-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Antes de hacer operaciones aritméticas con números debemos asegurarnos que el tipo de dato es numérico de contrario dará ERROR. Para convertir un string con un número en un tipo entero usamos:
```py
z = "2hola"
a = "10"
b = 9.8
c = "9.8"
d = 1 + 1j

print(int(z))   # ERROR
print(int(a))   # 10
print(int(b))   # 9
print(int(c))   # ERROR
print(int(c))   # ERROR
```
- Puede convertir strings si solo contienen números.
- No puede convertir strings con números flotantes, primero debes convertirlo a flotante y luego a entero.
- En caso de números reales solo devuelve la parte entera.
- No puede convertir números complejos.

</div></div>
 

### list()

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/python/list-transforma-elementos-a-una-lista-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




```py
first_name = "Asab"

print(list(first_name))    #["A","s","a","b"]
```
- Si le das un string devolverá la cadena de texto separada en elementos de letras.

</div></div>


### help()

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/python/help-obtener-informacion-sobre-alguna-funcion-integrada-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Esta función permite obtener información, al estilo del `--help` en Linux, sobre las funciones core de python.

</div></div>


### zip()

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/python/zip-crea-tuplas-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




La función `zip()` combina 2 o más iterables (listas, tuplas, cadenas, etc.) para crear una tupla. 
```py
lista1 = [1,2,3]
lista2 = ["a","b","c"]

tupla = zip(lista1, lista2) # Salida: [(1,"a"),(2,"b"),(3,"c")]
```

En caso de que los iterables tengan diferentes longitudes, zip solo se ejecuta hasta el iterable más corto.
```py
lista1 = [1,2]
lista2 = ["a","b","c"]

tupla = zip(lista1, lista2) # Salida: [(1,"a"),(2,"b")]
```


</div></div>


### range()

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/python/range-genera-una-secuencia-de-numeros-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




La función `range` permite generar una cierta cantidad de números, por defecto, desde el 0. El funcionamiento básico es:
```py
range(8) # Genera 8 números,desde 0 hasta el 8-1, sumando 1.
# 0,1,2,3,4,5,6,7

range(3,8) # Genera 8-3 números, desde el 3 hasta 8-1, sumando 1.
# 3,4,5,6,7

range(3,8,2) # Genera 8-3 números, desde el 3 hasta el 8-1, sumando 2.
# 3,5,7
```

En términos más técnicos la función range funciona así:
```py
version1 = range(total)
version2 = range(inicio,final)
version3 = range(inicio,final,saltos)
```
- `inicio`. Es el número con que comenzará la secuencia.
- `total`. El la cantidad de valores que se generará. En el caso de la versión 2 y 3 este número se calcula restando: `inicio`-`final`. Pero por temas prácticos también se puede hallar simplemente restado 1 al valor `final`.
- `saltos`. Es el número de números que se saltará la secuencia. Ejemplo: `range(2,8,2)` devuelve `2,4,6` porque le estamos indicando que en ves de generar números sumando 1 los genere sumando 2. 

## La función `range` y `print`

Pasa algo interesante cuando imprimimos un rango directamente:
```py
rango=range(2,9,2)
print=(rango)
   # Imprime: range(2,9,2)
```

Esto sucede porque python usa la [[Generación bajo demanda\|Generación bajo demanda]], que en términos simples significa que si no lo va a usar pues no lo calcula. El objeto si existe pero en ves de contener los valores generados, solo almacena en memoria la información para generar estos objetos. Cuando se requiera generar alguno, varios o todos hará el calculo y recién almacenará en momoria los números que requiera según la información de generación.

</div></div>


### len()

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/python/len-contar-la-longitud-de-una-lista/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Esta función te permite calcula la longitud, el número de items, dentro de un objeto:
```py
empty_object = ""
list_object = [1,2,3,5,3,7,8]
string_object = "Hello world"
dictionary_object = {"James": 10, "Mary": 12, "Robert": 11}

leg(empty_object)
# 0

len(list_object)
# 7

len(string_object)
# 11

len(dictionary_object)
# 3
```


La función `len()` no funciona con datos enteros, flotantes, complejos o boleanos porque estos objetos por definición no tienen longitud.
```py
len(5)
# TypeError: object of type 'int' has no len()

len(5.5)
# TypeError: object of type 'float' has no len()

len(True)
# TypeError: object of type 'bool' has no len()

len(5 + 2j)
# TypeError: object of type 'complex' has no len()
```

## Detalles técnicos
**Mejora la performance al usar `len()`**. Cuando se usa `len()` con secuencias ordenadas (listas, tuplas y strings) la función no necesita interactuar con el contenido del objeto. El contenedor de ese objeto almacena su longitud; cada ves que se agrega un item a ese objeto el valor del atributo de longitud suma uno y cada vez que se elimina un item, resta uno. Esto garantiza que `len()` use los recursos del sistema lo más eficientemente posible.

</div></div>


## Sistemas numéricos

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/python/sistemas-numericos-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Para identificar que un número está en un sistema numérico o en otro Python usa prefijos, los más comunes son:
- `0b11` --> 3 en **Binario** (0b)
- `0o10` --> 8 en **Octal** (0o)
- `0xA2` --> 162 en **Hexadecimal** (0x)
- `10` --> 10 en **Decimal**, los decimales no tienen prefijo

</div></div>
 

## Nombrar variables

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/python/nombres-de-variables-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




```py
capitales_latam = ["Lima","Bogotá","Santiago de Chile","Buenos Aires","Caracas"]
```


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/nombrar-variables/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




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


### Varias en una sola línea

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/python/declarar-varias-variables-en-una-sola-linea-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Solo alinea el nombre y el valor:
```py
first_name, last_name, country, age, is_married = 'Asabeneh', 'Yetayeh', 'Helsink', 250, True
```
- El primer elemento `first_name` se asigna al primer valor `Asabeneh`
- El segundo elemento `last_name` se asigna al segundo valor `Yetayeh`
- Y así con todos los elementos.
- Debe haber el mismo número de variables y de valores, de lo contrario, no se hará la asignación.

</div></div>

