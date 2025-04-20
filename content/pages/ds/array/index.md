# Arreglo

[< Regresar](/)

Un **arreglo** (o **lista**) es una colección simple y ordenada de datos. Algunas de las operaciones más comunes sobre un arreglo y su complejidad computacional son:

- **Agregar al final**: `O(1)`
- **Obtener por índice**: `O(1)`
- **Eliminar**: `O(n)` (los elementos se desplazan)
- **Buscar**: `O(n)` (se recorre la lista)

Teniendo en cuenta estas restricciones de la notación Big O, se puede concluir que los arreglos son especialmente eficientes cuando se trabaja con listas *cuyo orden original se mantiene constante*.

Esto se debe a que, al eliminar o insertar un elemento en una posición que **no** sea al final, el resto de la estructura debe desplazarse para hacer espacio o cerrar el hueco dejado por el elemento.

## Ejemplo visual

Supongamos que se tiene el siguiente arreglo:

```
[10, 20, 30, 40]
```

### Agregar al final (append)

Se agrega `50` al final:

```
[10, 20, 30, 40, 50]
```

Nota que solo se añade un elemento al final, sin afectar a los anteriores (`O(1)`).

### Insertar en el medio

Se inserta `25` en la posición 2 (entre `20` y `30`):

```
[10, 20, 25, 30, 40, 50]
```

Nota que todos los elementos desde la posición 2 (`20`) en adelante deben **desplazarse a la derecha** (`O(n)`).

### Eliminar en el medio

Se elimina el elemento en la posición 3 (el `30`):

```
[10, 20, 25, 40, 50]
```

Nota que los elementos posteriores deben **desplazarse a la izquierda** para llenar el espacio (`O(n)`).

