---
{"dg-publish":true,"permalink":"/learning/dev/python/declarar-varias-variables-en-una-sola-linea-en-python/","created":"2024-05-29T17:59","updated":"2024-05-29T18:29"}
---

Solo alinea el nombre y el valor:
```py
first_name, last_name, country, age, is_married = 'Asabeneh', 'Yetayeh', 'Helsink', 250, True
```
- El primer elemento `first_name` se asigna al primer valor `Asabeneh`
- El segundo elemento `last_name` se asigna al segundo valor `Yetayeh`
- Y así con todos los elementos.
- Debe haber el mismo número de variables y de valores, de lo contrario, no se hará la asignación.