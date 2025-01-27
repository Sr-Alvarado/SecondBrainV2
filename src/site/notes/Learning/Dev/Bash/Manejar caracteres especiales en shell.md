---
{"dg-publish":true,"dg-path":"Dev/Bash/Manejar caracteres especiales en shell.md","permalink":"/dev/bash/manejar-caracteres-especiales-en-shell/","created":"2025-01-21T11:54","updated":"2025-01-21T13:00"}
---

## Resumen
Bash ofrece dos métodos para manejar caracteres especiales:
- [[Learning/Dev/Bash/Manejar caracteres especiales en shell#Secuencias de Escape\|Secuencias de Escape]]. La barra invertida `\`, evita la interpretación de caracteres especiales en comandos.
- [[Learning/Dev/Bash/Manejar caracteres especiales en shell#Comillas Dobles\|Comillas Dobles]]. Las comillas `"` o `'`, tratan múltiples palabras como un solo argumento.

Ademas, debemos tener claro:
- [[Learning/Dev/Bash/Manejar caracteres especiales en shell#¿Comillas simples o comillas dobles\|¿Comillas simples o comillas dobles?]]. Las que eviten la ambigüedad. Si el argumento incluye comillas dobles, usa comillas simples; si el argumento incluye comillas simples, usa comillas dobles.
## Tipos
### Secuencias de Escape
Impide que la shell interprete el siguiente carácter como especial, tratándolo como texto plano. Ejemplo:

```bash
cat text\ \(1\).txt
```
* `cat`. Comando de [[GNU\|GNU]], imprime en consola el contenido completo de un archivo. 
* `\`. Símbolo de escape, declara al espacio y los paréntesis como texto plano.
* `text (1).txt`. Nombre del archivo.

### Comillas
Indican que todo el texto dentro de las comillas debe tratarse como un solo argumento, incluyendo caracteres especiales. Puede usarse comillas simples `'` o comillas dobles `"`. Ejemplo:

```bash
cat "text (1).txt"
```
* `cat`. Comando de [[GNU\|GNU]], imprime en consola el contenido completo de un archivo. 
* `"`: Delimita el inicio y fin del nombre del archivo.
* `text (1).txt`: Nombre del archivo.

## QA
### ¿Comillas simples o comillas dobles?
La elección en principio es personal, sin embargo, hay un truco, siempre debemos evitar la ambigüedad.

Si tu argumento tiene comillas dobles y lo envuelves en comillas dobles el sistema no sabra, donde comienza y termina, causando errores. Ejemplo:
```bash
echo "este es un "texto" con comillas dobles"
```
- El sistema podría dar un error al no entender claramente cual es el argumento.

Por ello, se considera buena practica usar las comillas opuestas para envolver el texto de las usadas dentro del argumento. Ejemplo:
```bash
echo 'este es un "texto" con comillas dobles'
```
- Al usar comillas simples `'` para envolver un argumento que contiene comillas dobles `"` eliminamos la ambigüedad.