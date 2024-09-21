---
{"dg-publish":true,"dg-path":"Code/Python/Order de importaciones en python.md","permalink":"/code/python/order-de-importaciones-en-python/","created":"2024-09-21T13:03","updated":"2024-09-21T13:04"}
---

Cuando trabajas con python y requieres importar paquetes debes saber que existe una forma correcta de ordenarlas:
- **Las estándar**. Módulos internos de python
- **De terceros**. Módulos creados por terceros
- **Locales**. Módulos creados por ti

Cada grupo debe estar separado por un espacio de los otros grupos. Ejemplo:
```py
# Estándar
from dotenv import load_dotenv
from textwrap import dedent
import os

# De terceros
from crewai import Agent
from langchain_openai import ChatOpenAI

# Locales
from tools.ExaSearchTool import ExaSearchTool

load_dotenv()
```
Adicionalmente, a mi me gusta ordenarlas por orden alfabético, permite que verificar una dependencia sea un trabajo más rápido.