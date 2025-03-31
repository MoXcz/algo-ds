# Big O

[< Regresar](/)

![Big O chart](/images/big_o_chart.jpeg)

Big O representa el crecimiento de las computaciones necesarias conforme `n` aumenta.

`n` es una variable que representa la cantidad de datos de entrada (*input*).

```
for i in range(n + 1):
    sum += i
return sum
```

En este caso, el *input* es `n`, y el Big O de la operación es `O(n)`, porque por cada valor de 0 a `n` se realiza una operación (sumar `i` a `sum`).

Por otro lado, el siguiente ejemplo representa un Big O de `O(1)`, ya que la operación se ejecuta *en tiempo constante*, sin importar el valor `n`.

```
return n * (n + 1) / 2
```

## ¿En conclusión?

Big O es una unidad de medida utilizada en algoritmos para predecir la cantidad de cómputo necesario para ejecutar una operación. Esto es clave, ya que un algoritmo con una complejidad alta puede volverse ineficiente o inoperable a medida que los datos crecen.

## Recursos

1. Imagen de: [Big-O Cheat Sheet](https://www.bigocheatsheet.com/)
