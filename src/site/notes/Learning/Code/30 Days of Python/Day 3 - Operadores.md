---
{"dg-publish":true,"dg-path":"Code/30 Days of Python/Day 3 - Operadores.md","permalink":"/code/30-days-of-python/day-3-operadores/","created":"2024-06-10T17:35","updated":"2024-07-21T12:17"}
---


**| [[Learning/Code/30 Days of Python/Day 2 - Funciones\|⬅️ After day]] | [[Learning/Code/30 Days of Python/30 Days of Python\|🏠 Home]] | [[Day 4 - Strings\|➡️ Next day]] | [⌨️ Ejercicios](https://github.com/Sr-Alvarado/30-Days-Of-Python-thon-solved-exercises/blob/main/03_day_operators.py) |** 

## Boleanos

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/python/boleanos-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">





<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/boleanos/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">

<div class="markdown-embed-title">

# bolean

</div>



En programación, es un tipo de dato que representa uno de dos valores: Verdadero o falso.
- `True` or `1`
- `False` or `0`

</div></div>

En [[python\|python]] siempre deben comenzar con mayúscula.

</div></div>

## Operadores
En python el símbolo ` =` se usa para asignar un valor.
![Pasted image 20240610174324.png|100%](/img/user/Engine/Attachments/Pasted%20image%2020240610174324.png)

## Operaciones aritméticas

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


## Operadores condicionales

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/python/operadores-condicionales-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




- `is` --> Verifica que 2 variables sean el mismo objeto, si 2 variables apunten al mismo objeto en memoria si es asi devuelve `True`. [[Learning/Code/is vs ==\|is vs ==]] 
- `is not` --> Es el opuesto de `is`, verifica que 2 variables no sean el mismo objeto, si es así devuelve `True`
- `in` --> Comprueba que un elemento pertenezca a una secuencia. Si se cumple devuelve `True`
- `not in` --> Opuesto a `in` verifica que un elemento no pertenezca a una secuencia. Si se cumple devuelve `True`


</div></div>


## Operadores lógicos

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/operadores-logicos/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




```py
3 > 2 and 4 > 3    # True
```
- `and` --> Devuelve `True` si ambos elementos son verdaderos.

```py
3 > 2 or 4 > 5    # True
```
- `or` --> Devuelve `True` si alguno de los elementos es verdadero.

```py
not 3 > 2        # False
```
- `not` --> Revierte el resultado, si es verdadero devuelve `False` y si es falso devuelve `True`.

</div></div>
 
