---
{"dg-publish":true,"dg-path":"Code/30 Days of Python/int() - Convertir a números enteros.md","permalink":"/code/30-days-of-python/int-convertir-a-numeros-enteros/","created":"2024-05-29T18:14","updated":"2024-05-29T18:14"}
---

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