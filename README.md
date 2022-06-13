# Curso manipulación de Arrays

# Mutable vs inmutable

- Mutable: es algo que se puede cambiar o agregar.
- Inmutable: es algo que no puede cambiar ni agregar.

![Primitive and reference values](/assets/images/primitive-reference-values.png)

![Pass By ](/assets/images/pass-by-example.gif)

# Metodos chidoris

## map

.map() es INMUTABLE por lo tanto no modifica el array original, sino que crea uno nuevo con la “transformación” aplicada.

Además, mantienes el mismo length que el array original, te devuelve en el nuevo array la misma cantidad que el array que le aplicaste el método.

## join

El método join() une todos los elementos de una matriz (o un objeto similar a una matriz) en una cadena y devuelve esta cadena.

![Join](/assets/images/join.png)

## filter

filter() lo que hace es filtrar el array original en base a una condición, los que la cumplan estaran en el nuevo array creado.
.
Por lo tanto filter() es inmutable y el nuevo array creado solamente puede contener:

- cero coincidencias
- todas coincidencias
- algunas coincidencias

Pero nunca más coincidencias que el tamaño del array original.

## reduce

Este método REDUCE, efectivamente hace eso. Solo reduce a un solo valor y no devuelve otro array, simplemente un valor.

Se utiliza muchísimo para hacer cálculos a partir de la información de un array.

En su composición, a primeras, tiene como argumentos de la función del primer parámetro, al acumulador y como segundo parámetro al elemento por el que va iterando el loop. Y como segundo argumento del reduce(), se pasa el valor inicial del acumulador.

![Reduce](/assets/images/reduce.gif)

## find

El método find() devuelve el primer elemento del array que cumpla con la condición dada o no devuelve undefined si es que no encuentra ningún elemento que cumpla los requisitos pedidos.

Retorna una referencia asi que el valor es mutable.

## findIndex

En cambio el método findIndex() es una variante que te devuelve el index o posición donde esta ese primer elemento que encuentra con las características de la condición dada. De no encontrar ninguno devuelve -1 como respuesta del return del método.

## includes

El método includes() determina si una array incluye un determinado elemento, devuelve true o false según corresponda.

![includes](/assets/images/includes.png)

También posee un segundo parámetro que es el fromIndex, que es la posición donde comenzar a buscar el valor en el array.

![includes from index](/assets/images/includes-from-index.png)

Este fromIndex sí es igual o mayor que el tamaño del array, devuelve false automaticamente sin buscar en el vector. Sí el fromIndex es negativo busca en todo el array. Y para los casos 0, -0, +0 lo toma como cero y también lee todo el array.

## concat

Fusiona arrays. Es inmutable (no modifica el array original).

![concat](/assets/images/concat.png)

## flatMap

flatMap() es un método que primero mapea cada elemento, y después aplana el resultado en un nuevo array.

Es idéntico a hacer un map() seguido de un flat() de profundidad 1.

![Flat map](/assets/images/flatMap.png)

Si necesitas hacer un flat de mayor profundidad, es mejor usar los métodos por separado, en lugar de usar flatMap().

# Desafios chidoris

## Calcular impuesto y redondear

![Calcular impuesto y redondear](/assets/images/calcular-impuesto-redondear.png)

## ¿Existe algún numero par?

![Existe algun numero par](/assets/images/existe-numero-par.png)

## ¿En que posición existe un string?

![En que posicion esta un string](/assets/images/posicion-existe-string.png)

## ¿Todos los numeros son par?

![Todos numeros par](/assets/images/todos-numeros-par.png)

## Total sumando numeros (reduce)

![Total sumando numeros](/assets/images/total-array-numeros.png)

## Convertir string a url

![String a url](/assets/images/string-a-url.png)

# Notas

## Evitar sobreescribir referencia con map al agregar una propiedad

![Map add new property](/assets/images/map-add-new-property.png)

## Generar histogramas

![Histograma](/assets/images/histograma.png)

## Se sobreponen fechas

![Sobreposicion de fechas](/assets/images/algoritmo-sobreponen-fechas.png)

## Filter vs find

![Filter vs find](/assets/images/filter-vs-find.webp)

## Aplanar arrays de arrays

![Aplanar arrays de arrays](/assets/images/aplanar-arrays-de-arrays.png)

## Obtener una propiedad de un array de objetos

![flatmap avanzado](/assets/images/flat-map-avanzado.png)
