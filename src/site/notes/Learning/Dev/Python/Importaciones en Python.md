---
{"dg-publish":true,"dg-path":"Dev/Python/Importaciones en Python.md","permalink":"/dev/python/importaciones-en-python/","created":"2024-11-04T17:10","updated":"2024-12-14T11:16"}
---

## Resumen


## Contenido
Las importaciones permiten traer código de otro lado y ejecutarlo en el archivo actual, al hablar de --- existen importaciones absolutas y relativas.
### Conocimiento previo
Hay ciertas cosas que debemos conocer antes de hablar de importaciones:
- [[Módulos en Python\|Módulos]]. Un módulo es cualquier archivo que tenga la extension `.py`
- [[Paquetes en Python\|Paquetes]]. Es cualquier carpeta que contenga un modulo, en [[Python2\|Python2]] debe contener ademas un archivo llamado [[__init__.py\|__init__.py]].
- [[Objetos en Python\|Objetos]]. Es cualquier clase, función o variable dentro de un archivo `.py`.

### Sintaxis
Cuando hablamos de importaciones en [[Python\|Python]], en realidad queremos llamar a ciertos módulos y/o paquetes. Ejemplo:
```py
import module1 from package1 as otro_nombre
```
- `import`. Sintaxis básica para importar paquetes o módulos en python.
- `from`. Se usa para declarar que se desea importar un sub-elemento (modulo, sub-paquete u objeto).
- `as`. Se usa para renombrar en el archivo local lo que se importa.

### Donde busca python las importaciones
Python busca primero los que fueron importados antes, `sys.modules`; en modulo internos del lenguaje, `buil-in`; y en los directorios del proyecto, `sys.path`:
- El primer lugar donde Python busca las importaciones es en [sys.modules](https://docs.python.org/3/library/sys.html#sys.modules): Es la memoria cache de todos los módulos importados anteriormente.
- Luego, busca en los módulos [[buil-in en Python\|buil-in]]: Estos son los módulos pre-instalados que vienen cuando instalas alguna version de Python.
- Al final, Python busca en el [[sys.path\|sys.path]]: Es una lista de los directorios de tu equipo.

### Guías de estilo
Hay ciertas reglas que es mejor seguir para mantener el código coherente y fácil de entender cuando se trata de importaciones:
- Siempre deben ir al principio del archivo.
- Se dividen en 3 grupos: Standard, de terceros y locales.
- Cada grupo debe estar separado por un espacio.
- Se recomienda ordenarlas alfabéticamente.

**Ejemplo de estilo**:
```py
# Standard library imports
import datetime
import os

# Third party imports
from flask import Flask
from flask_restful import Api
from flask_sqlalchemy import SQLAlchemy

# Local application imports
from local_module import local_class
from local_package import local_function
```
- Las `buil-in` o standard al principio, ordenadas alfabéticamente.
- Las de terceros en segundo lugar, ordenadas alfabéticamente.
- Las creadas por nosotros al final, ordenadas alfabéticamente.

### Importaciones absolutas
Estas son importaciones que usan la ruta absoluta de origen del proyecto para identificar que importar. Es la forma recomendada de hacer importaciones.
```py
from package1.subpackage2.subpackage3.subpackage4.module5 import function6
```
- En este caso debemos de carpeta a sub-carpeta para llamar a una importación.

#### Ejemplo de importaciones absolutas
**Ruta de carpetas del proyecto**:
Para el ejemplo asumiremos que el proyecto tiene la siguiente estructura de carpetas.
```bash
└── project
	├── main.py
    ├── package1
    │   ├── module1.py
    │   └── module2.py
    └── package2
    │   ├── __init__.py
    │   ├── module3.py
    │   ├── module4.py
    │   └── subpackage1
    │       └── module5.py
```

**Objetos de los módulos**.
Para el ejemplo asumiremos que los módulos (archivos) contienen ciertos objetos:
- `package1/module2.py` contiene la función, `function1`.
- `package2/__init__.py` contiene la clase, `class1`
- `package2/subpackage1/module5.py` contiene la función, `function2`.

**main.py**
Queremos importar módulos y paquetes desde `main.py`.
```py
from package1 import module1
from package1.module2 import function1
from package2 import class1
from package2.subpackage1.module5 import function2
```
- Nota que, para llamar a los paquetes hemos comenzado siempre desde la raíz del proyecto, esto siempre es así, sin importar en donde nos encontremos.

### Importaciones relativas
Permite hacer importaciones mas cortas, no llama a la importación desde la raíz si no desde la ubicación actual, por lo que depende de que la estructura del proyecto no cambie.
```py
from .some_module import some_class
from ..some_package import some_function
from . import some_class
```
- `.` se refiere a la carpeta actual.
- `..` se refiere a la carpeta padre de esta carpeta. Añadiendo otro punto te lleva a la carpeta padre de la carpeta padre...

### Archivo `__init__.py`
Este archivo declara que una carpeta se comportara como modulo, por lo general se puede quedar vacío, pero puede declarar las rutas y nombres de los paquetes y objetos dentro del modulo.

