---
{"dg-publish":true,"dg-path":"Dev/Python/int() - Convertir a números enteros en Python.md","permalink":"/dev/python/int-convertir-a-numeros-enteros-en-python/","created":"2024-05-29T18:14","updated":"2024-07-20T17:00"}
---

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