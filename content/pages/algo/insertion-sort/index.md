# Insertion sort

[< Regresar](/)

El algoritmo de ordenamiento _Insertion Sort_ construye la lista ordenada de manera incremental: toma un elemento a la vez y lo inserta en la posición correcta respecto a los elementos previamente ordenados.

Los pasos del algoritmo se pueden definir de la siguiente manera:

1. Comenzar desde el segundo elemento de la lista (suponiendo que el primer elemento ya está "ordenado").
2. Comparar el elemento actual con los anteriores y desplazar hacia la derecha aquellos que sean mayores (o menores, según el criterio).
3. Insertar el elemento actual en su posición adecuada.
4. Repetir hasta que todos los elementos hayan sido insertados en su lugar.

Este algoritmo tiene una complejidad de `O(n^2)` en el peor de los casos (cuando la lista está en orden inverso), pero en el mejor de los casos (lista ya ordenada) su complejidad es `O(n)`, ya que solo realiza una comparación por elemento.

> Aunque no es eficiente para listas grandes, _Insertion Sort_ es muy útil para listas pequeñas o casi ordenadas debido a su simplicidad y bajo costo de desplazamiento de elementos.

```
def insertion_sort(nums):
    for i in range(len(nums)):
        j = i
        while j > 0 and nums[j - 1] > nums[j]:
            nums[j], nums[j - 1] = nums[j - 1], nums[j]
            j -= 1
    return nums
```

Este ejemplo implementa _Insertion Sort_ de menor a mayor en una lista de números.

