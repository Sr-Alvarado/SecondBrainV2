---
{"dg-publish":true,"dg-path":"Dev/Versionado de proyectos en programación.md","permalink":"/dev/versionado-de-proyectos-en-programacion/","created":"2024-09-21T12:11"}
---

## Resumen
Generalmente al crear un proyecto en programación lo nombras como `v1`, luego `v1.1`, `v2`, etc. Sin embargo, no es necesario inventarse la rueda; ya existen guías de buenas prácticas que definen claramente cómo versionar un proyecto.
- [[Learning/Dev/Versionado de proyectos en programación#SemVer\|#SemVer]]. Versionado semántico. **(Recomendado)**
- [[Learning/Dev/Versionado de proyectos en programación#Versionado por calendario\|#Versionado por calendario]]. Basado en años.
- [[Learning/Dev/Versionado de proyectos en programación#Versionado por código de revisión\|#Versionado por código de revisión]]. Basado en el commit.
- [[Learning/Dev/Versionado de proyectos en programación#Versionado por fecha\|#Versionado por fecha]]. Basado en la fecha exacta de actualización.
- [[Learning/Dev/Versionado de proyectos en programación#Versionado por nivel de madurez\|#Versionado por nivel de madurez]]. Basado en el estado del desarrollo.

## Guías de versionado
### SemVer
El formato SemVer o versionado semántico define tres niveles de actualización:
- `1` → Versión mayor, para cambios incompatibles.
- `0` → Versión menor, para nuevas funcionalidades.
- `0` → Parche, para corrección de errores.

**Ejemplo completo**:
- `1.0.0` → Primera versión estable.
- `1.1.0` → Nueva funcionalidad compatible.
- `1.1.1` → Corrección de errores.

### Versionado por calendario
Se basa en el año y, opcionalmente, el mes para identificar las actualizaciones dentro de ese año.
- `YY`/`YYYY` → Año del lanzamiento.
- `MM`/`M` → Mes del lanzamiento.

**Ejemplo real**: Ubuntu
- `20.04`. Versión de abril del 2020.
- `22.10`. Versión de octubre del 2022.

### Versionado por código de revisión
Asocia la versión al número de commit, hash de Git, o compilación.
- `r1234` → Revisión 1234 en el sistema de control de versiones.
- `build-458` → Compilación número 458.

**Ejemplo completo**:
- `git-abc123`. Versión asociada al commit específico `abc123`.

### Versionado por fecha
Basado en fechas exactas, útil para publicaciones frecuentes.
- `20240101` → Versión publicada el 1 de enero de 2024.
- `2024.01.03` → Versión publicada el 3 de enero de 2024.

**Ejemplo completo**:
- `2023-12-31` (última versión del año 2023).

### Versionado por nivel de madurez
Indica el estado del desarrollo de la versión.
- `alpha` → En fase inicial, inestable.
- `beta` → Funcional, pero en pruebas.
- `rc1` → Versión candidata, próxima a ser estable.

**Ejemplo completo**:
- `1.0-alpha` → Primer desarrollo experimental.
- `1.0-beta` → Versión en pruebas.
- `1.0-rc1` → Primera candidata a estable.

## Preguntas y Respuestas
### ¿Cuál es la diferencia entre el versionado por calendario y el versionado por fecha?
El **[[Learning/Dev/Versionado de proyectos en programación#Versionado por calendario\|#Versionado por calendario]]** es más general, se enfoca en actualizaciones por segmentos del año (como años o semestres), es decir, si tu proyecto está acostumbrado a lanzar una actualización en cierto mes del año. El **[[Learning/Dev/Versionado de proyectos en programación#Versionado por fecha\|#Versionado por fecha]]** es más especifico, detalla el momento exacto del lanzamiento, se usa para proyectos que se actualizan constantemente.