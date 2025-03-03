# ¿Qué es un algoritmo?

[< Regresar](/)

![](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse2.mm.bing.net%2Fth%3Fid%3DOIP.plnlzEgxN2lvPS6zsvgDXgHaEK%26pid%3DApi&f=1&ipt=8a105e031a520c670090eedc89e7b5d32c1a7f0470451f656807054e816e7f2f&ipo=images)

> Un algoritmo es un conjunto de pasos a seguir. Eso es todo.

Sin embargo, muchas veces en las introducciones al tema se suelen presentar descripciones más _técnicas_:

> Un algoritmo es una secuencia finita y detallada de instrucciones que pueden ser implementadas en una computadora.

- **Definido**: Sigue una secuencia específica de pasos.
- **No ambiguo**: Tiene una _única_ interpretación y siempre produce el mismo resultado.
- **Implementable**: Puede ejecutarse en un número finito de pasos.

## Media y mediana

Un ejemplo básico de un algoritmo son la media y la mediana, dos formas comunes de resumir un conjunto de datos.

### Media

El algoritmo de la media (también conocida como promedio) es sencillo:

> La media de un conjunto de datos es la suma de todos los valores dividida entre la cantidad total de elementos.

Si se tiene el conjunto `{2, 4, 6, 8, 10}`, el algoritmo nos pide:

1. Sumar los números: `2 + 4 + 6 + 8 + 10` = `30`
2. Dividir entre la cantidad total de elementos: `30 / 5` = `6`

### Mediana

> La mediana es el valor central en un conjunto de datos ordenado, separando la mitad inferior de la superior.

Si se tiene el conjunto `{3, 7, 1, 5, 9}`, el algoritmo nos pide:

1. Ordenar los datos: `{1, 3, 5, 7, 9}`
2. Identificar el valor central: `5`

Si el número total de elementos es par, la mediana se obtiene calculando la media de los dos valores centrales.

Por ejemplo, en `{2, 4, 6, 8}`:

1. Ordenar los datos (nota que si los datos ya estan ordenados nada cambia): `{2, 4, 6, 8}`
2. Tomar los valores centrales (`4` y `6`) y calcular su media: `(4 + 6) / 2 = 5`
