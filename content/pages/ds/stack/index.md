# Pila (Stack)

[< Regresar](/)

Una **pila** es una estructura de datos que sigue el principio **LIFO** (*Last In, First Out*), es decir, el último elemento en entrar es el primero en salir.

> Piensa en una pila de platos: solo se pueden remover los platos de la parte superior.

## Operaciones principales

- `push` (agregar al tope): `O(1)`
- `pop` (eliminar del tope): `O(1)`
- `peek` (ver el tope sin eliminarlo): `O(1)`
- `size` (tamaño de la pila): `O(1)`

Las operaciones en una pila son muy eficientes porque siempre ocurren en el mismo extremo: el tope.

## Ejemplo visual

Supongamos que se tiene la siguiente pila vacía:

```
[]
```

### Agregar (`push`)

Se agregan (`push`) elementos:

```
[10]
[10, 20]
bottom -> [10, 20, 30] <- top
```

Nota que el `30` es el último en entrar, por lo tanto, deberá ser el primero en salir.

### Eliminar (`pop`)

Se quita (`pop`) el último elemento:

```
[10, 20]
```

Nota que solo se elimina el elemento en el tope (`30`), sin necesidad de desplazar los demás (`O(1)`).

### Ver (`peek`)

Se obtiene (`peek`) el elemento en el tope sin quitarlo:

```
Tope = 20
```

### Tamaño (`size`)

Se obtiene (`size`) el número de elementos sin modificarlos:

```
Tamaño = 2
```

## ¿Cuándo usar una pila?

Las pilas son útiles en casos donde se necesita:

- Deshacer acciones (como Ctrl+Z). Un ejemplo claro de esto es el historial de navegación (las flechitas que se ven arriba en un navegador). Más información sobre esto [aquí](https://developer.mozilla.org/en-US/docs/Web/API/History/pushState).
- Evaluar expresiones (como en compiladores o calculadoras).

