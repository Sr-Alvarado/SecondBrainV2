---
{"dg-publish":true,"dg-path":"Code/Python/Añadir un .gitignore listo en Python.md","permalink":"/code/python/anadir-un-gitignore-listo-en-python/","created":"2024-09-23T18:54","updated":"2024-10-02T12:51"}
---

No se si lo sepas pero, la gente de [[Learning/Code/GitHub/GitHub\|GitHub]] tiene un repo con un montón de [[Learning/Code/Git/gitignore - Indicar a Git que ignore un archivo\|gitignore]] listos para usar. Usando su repo podemos descargar un `.gitignore` perfecto para [[python\|python]]. Solo abre la terminal en tu proyecto y copia:
```bash
wget -O .gitignore https://raw.githubusercontent.com/github/gitignore/main/Python.gitignore
```
- `wget`. Programa [[CLI\|CLI]] especializado en descargar archivos de la web.
- `-O`. Flag de `wget` que declara el nombre que se le dará al archivo descargado^[ No es obligatorio, si no lo colocas el nombre usará el nombre original. Ejemplo: `wget www.enalce-de-descarga.com`.].
- `link`. Enlace de donde de descargará el archivo, `wget` descargará todo lo que se pueda, si es una página web, descargará el [[Learning/Wiki/HTML\|HTML]].