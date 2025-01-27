---
{"dg-publish":true,"permalink":"/learning/dev/python/modificadores-de-parametro-en-python/","created":"2025-01-01T19:45","updated":"2025-01-01T20:37"}
---

## Resumen
En Python los modificadores de parámetros (`/`, `*`, `*args`, `**kwargs`) controlan cómo se pasan los argumentos a una función, definiendo si son posicionales, nombrados o variables.
- [[#`/` - Argumento solo posicional|`/` - Argumento solo posicional]]. Exige que los parámetros antes del `/` solo se pasen por posición.
- [[#`*` - Argumento solo nombrado|`*` - Argumento solo nombrado]]. Exige que los parámetros después del `*` solo se pasen por nombre.
- [[#`*args` - Argumentos posicionales variables|`*args` - Argumentos posicionales variables]]. Captura múltiples argumentos posicionales en una tupla.
- [[#`**kwargs` - Argumentos nombrados variables|`**kwargs` - Argumentos nombrados variables]]. Captura múltiples argumentos nombrados en un diccionario.

## Tipos de modificadores
### `/` - Argumento solo posicional
El marcador `/` indica que los parámetros anteriores solo pueden pasarse por posición, no por nombre. Esto es útil cuando queremos que los argumentos sigan un orden específico sin que el usuario pueda pasarlos por nombre. Ejemplo:

```py
def dividir(a, b, /):
    return a / b

dividir(10, 2)  # Correcto: los argumentos se pasan por posición.
dividir(a=10, b=2)  # Error: los argumentos no pueden pasarse por nombre.
```
- `/`. Exige que los parámetros antes del símbolo `/`, como `a` y `b`, solo puedan pasarse por posición.

### `*` - Argumento solo nombrado
El marcador `*` indica que todos los parámetros posteriores deben ser pasados por nombre, no por posición. Esto asegura que los argumentos sean explícitos. Ejemplo:

```py
def saludar(nombre, *, mensaje="Hola"):
    return f"{mensaje}, {nombre}"

saludar("Juan", mensaje="Buenos días")  # Correcto: `mensaje` se pasa por nombre.
saludar("Juan", "Buenos días")  # Error: `mensaje` debe pasarse por nombre.
```
- `*`. Indica que los parámetros después del símbolo `*`, como `mensaje`, deben ser pasados solo por nombre.

### `*args` - Argumentos posicionales variables
El modificador `*args` permite aceptar un número variable de argumentos posicionales, que se almacenan como una tupla. Esto es útil para funciones que pueden recibir múltiples argumentos sin especificar su número exacto. Ejemplo:

```py
def sumar(*args):
    return sum(args)

sumar(1, 2, 3)  # Correcto: acepta múltiples valores posicionales.
sumar()  # Correcto: no es obligatorio pasar valores.
```
- `*args`. Captura cualquier cantidad de argumentos posicionales y los almacena en una tupla, permitiendo mayor flexibilidad.

### `**kwargs` - Argumentos nombrados variables
El modificador `**kwargs` permite aceptar un número variable de argumentos nombrados, que se almacenan en un diccionario. Es útil cuando no se sabe qué claves y valores se recibirán. Ejemplo:

```py
def describir(**kwargs):
    for clave, valor in kwargs.items():
        print(f"{clave}: {valor}")

describir(nombre="Juan", edad=30, profesion="Ingeniero")  # Correcto: acepta argumentos nombrados.
describir()  # Correcto: no es obligatorio pasar valores.
```
- `**kwargs`. Captura cualquier cantidad de argumentos nombrados, almacenándolos en un diccionario para fácil acceso.