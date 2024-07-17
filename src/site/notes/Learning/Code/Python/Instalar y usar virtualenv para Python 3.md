---
{"dg-publish":true,"dg-path":"Code/Python/Instalar y usar virtualenv para Python 3.md","permalink":"/code/python/instalar-y-usar-virtualenv-para-python-3/","tags":["python/3","virtualenv","shell","terminal"],"created":"2024-03-04T11:36","updated":"2024-03-27T12:56"}
---

Si estás en este artículo, se asume que: sabes que es [[virtualenv\|virtualenv]], [[Python 3\|Python 3]] y [[pip\|pip]], y tienes instalado los 2 últimos. Así que vamos de frente a lo bueno.

## Como instalar virtualenv
- **Fuente original**: [Instalar y usar virtualenv con Python 3 – Centro de Ayuda de DreamHost](https://help.dreamhost.com/hc/es/articles/115000695551-Instalar-y-usar-virtualenv-con-Python-3)

Para este ejemplo usaremos [[pip3\|pip3]]. Si no lo tienes instalado, ejecuta este comando:
```shell
python3 -m pip install --upgrade pip
```
Para instalar virtualenv para python3 con pip3 usa este comando:
```shell
pip3 install virtualenv
```
Para ver la dirección exacta donde se instaló puedes usar:
```shell
which virtualenv
```
Y listo! Ya instalaste virtualenv para crear entornos virtuales con Python.

## Crear y activar un entorno virtual con virtualenv
- **Fuente original**: [Instalar y usar virtualenv con Python 3 – Centro de Ayuda de DreamHost](https://help.dreamhost.com/hc/es/articles/115000695551-Instalar-y-usar-virtualenv-con-Python-3)

Ubícate en la dirección del fichero donde ejecutarás el virtualenv.
```shell
cd ~/RUTA_ABSOLUTA_DEL_PROYECTO
```
Crea el ambiente virtual usando:
```shell
virtualenv -p ~/RUTA_ABSOLUTA_DE_TU_VERSION_DE_PYTHON venv
```
- `virtualenv` indica que se usará este programa.
- `-p` es un flag de virtualenv que especifica la ruta de tu versión de Python.
   - Si no conoces esta ruta, puedes saberla usando este comando: `which python3`.
- `venv` es el nombre que le das al virtualenv creado.

Ahora toca activar el ambiente virtual:
```shell
source venv/bin/activate
```
Y listo! El nombre de tu ambiente virtual aparecerá a la izquierda de los flags de la terminal. Cualquier paquete `pip` que instales ahora se ubicará en tu carpeta actual y solo funcionará allí.

## Desactiva un entorno virtual con virtualenv
- **Fuente original**: [Instalar y usar virtualenv con Python 3 – Centro de Ayuda de DreamHost](https://help.dreamhost.com/hc/es/articles/115000695551-Instalar-y-usar-virtualenv-con-Python-3)

Para desactivar tu entorno virtual solo debes ejecutar este comando:
```shell
deactivate
```

Y listo!

## Elimina un entorno virtual con virtualenv
- **Fuente original**: [Instalar y usar virtualenv con Python 3 – Centro de Ayuda de DreamHost](https://help.dreamhost.com/hc/es/articles/115000695551-Instalar-y-usar-virtualenv-con-Python-3)

Para eliminar el virtualenv solo debes eliminar la carpeta del virtualenv:
```shell
rm -rf venv
```

Y listo! Ahora ya sabes como instalar, crear, activar, desactivar y eliminar un ambiente virtual usando virtualenv. Espero que esta información te sea útil. 