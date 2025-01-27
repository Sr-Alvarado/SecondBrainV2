---
{"dg-publish":true,"permalink":"/learning/dev/python/requirements-txt-instalar-dependencias-desde-un-archivo-en-python/","created":"2024-10-02T12:58","updated":"2024-10-02T13:07"}
---

Una buena práctica en proyectos pequeños es usar un archivo para listar las dependencias del proyecto [[python\|python]]. Como buena práctica el archivo se nombra como:`requirements.txt`. 

## requirements.txt
Dentro de `requirements.txt` coloca el nombre de cada dependencia de tu proyecto, puedes añadir y filtrar las versiones que se deberían usar. Ejemplo:

```txt
# Versión específica
numpy==1.21.0

# Versión mayor o igual a
pandas>=1.3.0

# Versión menor a
scikit-learn<0.24

# Versión mayor a
flask>1.1

# Versión dentro de un rango
requests>=2.25,<=2.27

# Última versión compatible (según semantic versioning)
pytest~=6.0

# Versión específica con extras opcionales
matplotlib[toolkits]==3.4.2
```


## Instalar desde un archivo usando `pip`
Para instalar las dependencias desde un archivo, usando [[pip\|pip]], solo debes ejecutar el comando:
```bash
pip install -r requirements.txt
```
- `-r`. Es una opción de `pip` que declara que se debe leer el archivo a continuación e instalar las dependencias que especificadas.