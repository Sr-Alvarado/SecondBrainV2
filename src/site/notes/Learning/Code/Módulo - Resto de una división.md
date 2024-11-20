---
{"dg-publish":true,"dg-path":"Code/Módulo - Resto de una división.md","permalink":"/code/modulo-resto-de-una-division/","created":"2024-06-03T17:25","updated":"2024-06-03T18:11"}
---

El módulo de dos números se entiende como el resto de la división. La cantidad que queda después de dividir esos números considerando que solo se hacen divisiones enteras, es decir solo números naturales. En programación se suele usar `%` para declarar esta operación.
- `10 % 5 = 10 - (5 * 2) = 0`
- `12 % 5 = 12 - (5 * 2) = 2`
- `12 % 12 = 12 - (12 * 1) = 0`

### Casos especiales
**¿Cuál es resultado de 5 % 10?** --> `5 % 10 = 5 - (10 * 0) = 5`
- El truco para entender porque sucede esto es recordar que estamos operando en números naturales. Si el primer número (divisor) es menor al segundo (dividendo) la división dará 0, por lo tanto el residuo de esa operación será igual al divisor.

**¿Puedo sacar el módulo de números reales?**
- Si, el módulo se calcula sin tomar en cuenta los decimales, sin embargo se puede usar números con decimales en divisor y/o dividendo, estos números se comportan como una unidad por lo que la operación es completamente valida.
   - `2.4 % 1.2 = 2.4 - (1.2 * 2) = 0`
   - `2.8 % 1.2 = 2.8 - (1.2 * 2) = 0.4`