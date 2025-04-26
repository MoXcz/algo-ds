# Búsqueda Binaria (Binary Search)

[< Regresar](/)

Este algoritmo se basa en búsquedas por *mitades*, tomando en cuenta que la colección de elementos *debe estar ordenada*. Gracias a su característico método de búsqueda, su complejidad de tiempo es `O(log n)`.

```
def binary_search(target, arr):
    low = 0
    high = len(arr) - 1
    while low <= high:
        median = (low + high) // 2
        if arr[median] == target:
            return True
        elif arr[median] < target:
            low = median + 1
        else:
            high = median - 1
    return False
```

El proceso de dividir en mitades surge al comparar si el elemento buscado se encuentra a la izquierda (menor) o a la derecha (mayor) del elemento actual. De esta manera, se eliminan rápidamente grandes cantidades de elementos:

`1,000,000` → `500,000` → `250,000` → `125,000` → ...

> **Nota**: Se recomienda utilizar algoritmos de ordenamiento cuya complejidad sea cercana a `O(n log n)`.

## Recursos

1. [Definición en Wikipedia](https://en.wikipedia.org/wiki/Binary_search)

