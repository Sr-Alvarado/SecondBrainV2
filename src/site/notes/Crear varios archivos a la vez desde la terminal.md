---
{"dg-publish":true,"permalink":"/crear-varios-archivos-a-la-vez-desde-la-terminal/","created":"2024-02-04T20:42","updated":"2024-02-04T20:42"}
---

## Vamos directo a lo bueno...
### Crear archivos con diferentes nombres
```bash
touch {one,two,three}.txt
```
- Este comando creará 3 archivos `.txt` con los nombres `one.txt`, `two.txt` y `three.txt`.
### Crear archivos con una parte del nombre igual
```bash
touch texto{1,2,3}.txt
```
- Este comando creará 3 archivos `.txt` con los nombres `texto1.txt`, `texto2.txt` y `texto3.txt`.
### Tips
Puedes modificar esto a voluntad, solo asegúrate de:
- Usar llaves para indicar la parte que quieres se sea única.
- Separar por comas.
- No dejar espacios intermedios.