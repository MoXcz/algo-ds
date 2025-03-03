# Big O

[< Regresar](/)

![Big O chart](/images/big_o_chart.jpeg)

Big O representa el crecimiento de las computaciones necesarias conforme `n` aumenta.

`n` es una variable que representa la cantidad de datos de entrada (*input*).

```
for i in list {
    print(i)
}
```

En este caso, el *input* es `list`, una lista de elementos, y el Big O de la operación es `O(n)`, porque *por cada valor dentro de la lista* se realiza una operación.

Por otro lado, el siguiente ejemplo representa un Big O de `O(1)`, ya que la operación se ejecuta *una única vez*, sin importar el tamaño del *input*:

```
print(i)
```

Big O es una unidad de medida utilizada en algoritmos para predecir la cantidad de cómputo necesario para ejecutar una operación. Esto es clave, ya que un algoritmo con una complejidad alta puede volverse ineficiente o inoperable a medida que los datos crecen.

## Recursos

1. Imagen de: https://www.bigocheatsheet.com/
