# Cola (Queue)

[< Regresar](/)

Una **cola** es una estructura de datos que sigue el principio **FIFO** (*First In, First Out*), es decir, el primer elemento en entrar es el primero en salir.

> Piensa en una fila para hacer el mandado: las personas se atienden en el orden en que llegaron.

## Operaciones principales

- `enqueue` (agregar al final): `O(1)` en listas enlazadas, `O(n)` en arreglos
- `dequeue` (eliminar del frente): `O(1)`
- `peek` (ver el frente sin eliminarlo): `O(1)`
- `size` (tamaño de la cola): `O(1)`

Las operaciones en una cola son eficientes porque siempre ocurren en extremos opuestos: al frente o al final.

## Ejemplo visual (con arreglos)

Supongamos que se tiene la siguiente cola vacía:

```
[]
```

### Agregar (`enqueue`)

Se agregan (`enqueue`) elementos:

```
[10]
[10, 20]
front -> [10, 20, 30] <- end
```

Nota que el `10` fue el primero en entrar, por lo tanto, será el primero en salir.

### Eliminar (`dequeue`)

Se elimina (`dequeue`) el primer elemento:

```
[20, 30]
```

Solo se elimina el elemento al frente (`10`), recorriendo los demás elementos si se usa un arreglo (`O(n)`).

### Ver (`peek`)

Se obtiene (`peek`) el elemento al frente sin quitarlo:

```
Frente = 20
```

### Tamaño (`size`)

Se obtiene (`size`) el número de elementos sin modificarlos:

```
Tamaño = 2
```

## ¿Cuándo usar una cola?

Las colas son útiles en situaciones donde se necesita:

- Procesar tareas en orden (como en una impresora).

