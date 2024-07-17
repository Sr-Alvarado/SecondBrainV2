---
{"dg-publish":true,"dg-path":"Code/30 Days of Python/range() - Genera una secuencia de números.md","permalink":"/code/30-days-of-python/range-genera-una-secuencia-de-numeros/","created":"2024-07-16T18:25","updated":"2024-07-16T18:51"}
---

La función `range` permite generar una cierta cantidad de números, por defecto, desde el 0. El funcionamiento básico es:
```py
range(8) # Genera 8 números,desde 0 hasta el 8-1.
# 0,1,2,3,4,5,6,7

range(3,8) # Genera 5 números,es decir (8-3), desde el 3 hasta 8-1.
# 3,4,5,6,7

range(3,8,2) # Genera números desde el 3 hasta el 8-1, de 2 en 2.
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