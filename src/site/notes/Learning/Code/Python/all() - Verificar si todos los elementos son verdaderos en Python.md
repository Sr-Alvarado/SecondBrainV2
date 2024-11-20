---
{"dg-publish":true,"dg-path":"Code/Python/all() - Verificar si todos los elementos son verdaderos en Python.md","permalink":"/code/python/all-verificar-si-todos-los-elementos-son-verdaderos-en-python/","created":"2024-05-29T17:01","updated":"2024-05-29T18:28"}
---

Evalúa iterables, si todos los elementos son verdaderos devuelve TRUE, si uno es falso devuelve FALSE. Los elementos que se consideran FALSE son:


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/code/python/elementos-que-devuelven-false-en-python/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




- 0 --> El cero en cualquier tipo (entero, flotante y complejo)
- "" --> Cadenas vacías (strings, diccionarios, listas, tuplas, conjuntos y conjuntos inmutables)
- `None` --> El objeto None
- `bytearray(b'')` --> arreglos de bytes vacíos
- `bytes(b'')` --> secuencias de bytes vacías

</div></div>


Todo lo demás se considera TRUE.