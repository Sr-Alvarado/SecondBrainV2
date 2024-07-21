---
{"dg-publish":true,"dg-path":"Code/30 Days of Python/Day 1 - Introducción.md","permalink":"/code/30-days-of-python/day-1-introduccion/","created":"2024-03-08T15:10","updated":"2024-07-21T11:58"}
---


   **| [[Learning/Code/30 Days of Python/30 Days of Python\|🏠 Home]] | [[Learning/Code/30 Days of Python/Day 2 - Funciones\|➡️ Next day]] | [⌨️ Ejercicios](https://github.com/Sr-Alvarado/30-Days-Of-Python-thon-solved-exercises/blob/main/01_day_introduccion.py) |** 

## Download and Install python
- Descarga la última versión de python desde python.org
- Instala siguiendo la guía de la misma página
## Check my install version of python
```shell
python --version
```
![Pasted image 20240308152213.png|100%](/img/user/Engine/Attachments/Pasted%20image%2020240308152213.png)

## Use python in Python Shell

```shell
YOUR_PYTHON_VERSION
```

![Pasted image 20240308152229.png|100%](/img/user/Engine/Attachments/Pasted%20image%2020240308152229.png)

## Basics errors
- SyntaxError
- IndexError
- NameError
- ModuleNotFoundError
- KeyError
- ImportError
- AttributeError
- TypeError
- ValueError
- ZeroDivisionError
## Mathematical operations

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/operadores-matematicos/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




## Operaciones
- **Sum**: 3`+`2
- **Subtraction**: 3`-`2
- **Multiply**: 3`*`2
- **Division**: 3`/`2 
- **Exponente**: 3`**`2 ==Se lee: 3 al exponente 2==
- **[[Learning/Code/Módulo - Resto de una división\|Módulo]]**: 3`%`2 ==Devuelve el residuo de una división==
- **Resto**: 3`//`2 ==Devuelve solo la parte entera de una división==

## Operadores
- **Igual**: ` '==` 
- **Diferente**: ` !=` 
- **Mayor que**: ` >`
- **Menor que**: ` <`
- **Mayor o igual**: ` >=`
- **Menor o igual**: ` <=` 

</div></div>


## Comments
- **Una sola linea**: `# one line quote`
- **Multi-linea**: `"""multi line quote"""` 

## Create blocks / Indentation
Python usa la indentación para crear bloques, puedes usar una sangría de 2 espacios para crear la indentación, python reconocerá todo lo que lleve esa sangria como parte bloque anterior sin sangría.

```py
Bloque 1
   Sub Bloque 1.1
   Sub Bloque 1.2
      Sub Bloque 1.2.1
Bloque 2
```

## Data types
### Numbers
Python acepta 3 tipos de números:
- **Integer**. Números reales
- **Float**. Números decimales
- **Complex**. Números complejos
### Strings
Los strings son las cadenas de texto, para declarar una cadena de texto puedes usar:
- **Una sola linea**: `'cadena de texto simple'`
- **Una sola linea**: `"cadena de texto simple"`
- **Multi-linea**: `'''cadena de texto de varias lineas de texto'''`
- **Caso especial**: `"""text"""`, si un texto con comillas triples no es asignada a una variable, python lo reconocerá como un comentario.
### Boleans

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/boleanos/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




En programación, es un tipo de dato que representa uno de dos valores: Verdadero o falso.
- `True` or `1`
- `False` or `0`

</div></div>
 
### Lists
Una lista es una colección ordenada de elementos, puede contener diferentes tipos de datos. Se define con [], ejemplo:
- ['Banana', 10, False, 9.81]

### Dictionary
Un diccionario es una colección desordenada de elementos, usa el formato clave-valor:
```py
{
'clave':'valor',
'first_name':'Asabeneh', 
'age':250, 
'is_married':True,
'skills':['JS', 'React', 'Node', 'Python']
}
```

### Tuple
Es como una lista, la diferencia es que, una vez creada no se pueden cambiar los datos de una Tupla, es [[Inmutabilidad\|inmutable]]. Se define usando ().
```py
('Asabeneh', 'Pawel', 'Brook', 'Abraham', 'Lidiya') # Names
```

### Set
Es una lista parecida a una tupla o a una lista, la particularidad de un Set es que esta lista no es ordenada, solo acepta valores únicos, si tienes dos valores iguales, solo guardará uno.
```py
{3.14, 9.81, 2.7} # order is not important in set
```

## Exercises
[Ejercicios Primer día · 30 days of python](https://github.com/Sr-Alvarado/30-Days-Of-Python-thon-solved-exercises/blob/main/01_day_introduccion.py)
