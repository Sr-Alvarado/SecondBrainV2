---
{"dg-publish":true,"dg-path":"Code/Python/zip() - Crea tuplas en Python.md","permalink":"/code/python/zip-crea-tuplas-en-python/","created":"2024-07-16T17:36","updated":"2024-07-16T17:49"}
---

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
