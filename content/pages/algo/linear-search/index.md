# Búsqueda Lineal (Linear Search)

[< Regresar](/)

Este algoritmo de búsqueda se basa, como su nombre lo indica, en un método *lineal*, comúnmente a través de iteraciones sobre un arreglo. Debido a la naturaleza lineal de la búsqueda, el algoritmo tiene una complejidad de tiempo `O(n)`.

```
def linear_search(target, arr):
    for value in arr:
        if value == target:
            return True
    return False
```

La única razón para considerar el uso de este algoritmo es cuando el número de datos es pequeño. Para conjuntos de datos con más de 10,000 elementos, probablemente sea mejor utilizar otro algoritmo de búsqueda, como [búsqueda binaria](/pages/algo/binary-search).

> **Nota**: No es recomendado implementar este tipo de busqueda con listas enlazadas

## Recursos

1. [Definición en Wikipedia](https://en.wikipedia.org/wiki/Linear_search)

