---
{"dg-publish":true,"permalink":"/learning/dev/python/len-contar-la-longitud-de-una-lista/","created":"2024-07-20T13:44","updated":"2024-07-20T15:54"}
---

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