# Selection Sort

[< Regresar](/)

![](https://static.packt-cdn.com/products/9781785888731/graphics/image_13_007-1.jpg)

_Selection Sort_ es un algoritmo similar a _Bubble Sort_ en el sentido de que realiza de manera iterativa intercambios entre elementos para acomodarlos en su posición ordenada.

La diferencia con _Bubble Sort_ está en que _Selection Sort_ utiliza un valor `min` para mantener el registro del índice del valor más pequeño encontrado durante cada iteración.

Los pasos del algoritmo son:

1. Empezando desde el primer elemento de la lista, se intenta encontrar el valor más pequeño en el resto de la lista (de la posición actual hasta el final).
2. Intercambia el valor más pequeño encontrado con el valor de la posición actual.
3. Mover al siguiente elemento y repetir hasta que se haya recorrido toda la lista.
4. La lista estará ordenada cuando se haya pasado por todos los elementos.

```
def selection_sort(nums):
    for i in range(len(nums)):
        min_idx = i
        for j in range(i + 1, len(nums)):
            if nums[j] < nums[min_idx]:
                min_idx = j
        nums[i], nums[min_idx] = nums[min_idx], nums[i]
    return nums
```


## Recursos

1. Imagen de: [Learning Functional Data Structures and Algorithms](https://subscription.packtpub.com/book/programming/9781785888731)
