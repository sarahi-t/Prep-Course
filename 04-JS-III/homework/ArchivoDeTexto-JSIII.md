# JavaScript III
**Arrays**<br />
Los arrays son una manera de organizar datos en JavaScript. Esta "lista" recibe valores del mismo o diferentes tipos de datos, separados por una coma dentro de corchetes (`[]`). A estos valores se les denomina "elementos". <br />

Los arrays están indexados, o sea que cada valor dentro de los corchetes es representado por un número, empezando por el cero. Esto es conveniente, ya que se puede acceder a diferentes elementos a través de su índice.<br />

Los arrays tienen propiedades, como su longitud (número de elementos). Se puede conocer la longitud usando `.length`. También, existen métodos que pueden modificar el arreglo: <br />
- El método `.push` agrega un elemento al final de la lista.
- El método `.pop` no solo elimina, pero devuelve el último elemento.
- `.shift` elimina el primer elemento.
- Y `.unshift` agrega un elemento al inicio del array.<br />

Para facilitar la visualización, o manipulación de elementos en un arreglo, se pueden utilizar los ciclos `for`. Conociendo la *longitud* de nuestro arreglo, podemos iterar por cada uno de sus elementos con una condición de stop del número de elementos que contiene.