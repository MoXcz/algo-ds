# Bubble Sort

[< Regresar](/)

![](https://favtutor.com/resources/images/uploads/mceu_61632030011682402256084.png)

El algoritmo de ordenamiento _Bubble Sort_ compara de manera iterativa los elementos adyacentes para decidir si deben intercambiarse de posición, de tal manera que, al finalizar, todos los elementos de la lista estarán en su posición adecuada según el criterio de ordenamiento utilizado.

Los pasos del algoritmo se pueden definir de una manera similar a la siguiente:

1. Recorrer la lista comparando cada par de elementos adyacentes.
2. Si un elemento es mayor que el siguiente (o menor, según el criterio), intercambiarlos.
3. Repetir hasta que no haya más intercambios en una pasada completa.
4. La lista estará ordenada cuando no se realicen más intercambios.

Este algoritmo tiene una complejidad de `O(n^2)`, ya que en el peor de los casos requiere realizar `n` pasadas sobre la lista, con dos iteraciones anidadas, para ordenar y verificar que no queden elementos desordenados.

En el caso de que la lista ya esté ordenada, el algoritmo solo realiza una única _pasada_ para confirmar que los elementos están en su posición correcta.

```
def bubble(nums):
    cambio = True
    n = len(nums)
    while cambio:
        cambio = False
        for i in range(1, n):
            if nums[i - 1] > nums[i]:
                nums[i - 1], nums[i] = nums[i], nums[i - 1]
                cambio = True
        n -= 1
    return nums
```

Este ejemplo implementa _Bubble Sort_ de menor a mayor en una lista de números.

## Recursos

1. Imagen de [aqui](https://favtutor.com/blogs/bubble-sort-python)
