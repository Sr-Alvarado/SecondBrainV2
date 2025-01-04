---
{"dg-publish":true,"dg-path":"Dev/Python/Añadir un .gitignore listo en Python.md","permalink":"/dev/python/anadir-un-gitignore-listo-en-python/","created":"2024-09-23T18:54","updated":"2025-01-03T22:29"}
---

No se si lo sepas pero, la gente de [[Learning/Dev/GitHub/GitHub\|GitHub]] tiene un repo con un montón de [[Learning/Dev/Git/gitignore - Indicar a Git que ignore un archivo\|gitignore]] listos para usar. Usando su repo podemos descargar un `.gitignore` perfecto para [[python\|python]]. Solo abre la terminal en tu proyecto y copia:
```bash
wget -O .gitignore https://raw.githubusercontent.com/github/gitignore/main/Python.gitignore
```
- `wget`. Programa [[CLI\|CLI]] especializado en descargar archivos web.
- `-O`. Flag de `wget`, declara el nombre que se le dará al archivo descargado^[ No es obligatorio, si no lo llamas, usará el nombre original. Ejemplo: `wget www.enalce-de-descarga.com`.].
- `link`. Dirección web de descarga, `wget` descargará lo que haya en el enlace, si es una página web, descargará el [[Learning/Wiki/HTML\|HTML]]. 