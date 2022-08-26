# JavaScript VI <br />

Una función de orden superior es una función que puede aceptar una función como parámetro, regresar una función, o ambas.

**Funciones Callback** <br />
Se le llaman funciones callback a las funciones que son pasadas como parámetros. Las funciones callback son invocadas durante la ejecución de la función de orden superior. <br/>
Las funciones anónimas también pueden ser argumentos.
<br /><br />
Uno de los usos de funciones de callback es con iteradores. Los iteradores, o métodos de iteración nos ayudan a iterar en arrays, manipular elementos y regresar valores. Algunos ejemplos son:<br />
- `.forEach()`: ejecuta el mismo código para cada elemento de un array.
- `.map()`: toma el argumento de una función callback y regresa un nuevo array.
- `.filter()`: como map también regresa un array pero filtra ciertos elementos del array original. Evalúa una condición para lograrlo. Cada iteración que resulte en true, es añadida al array y el resto de elementos son descartados.
- `.reduce()`: regresa un valor después de iterar los elementos de un array, reduciéndolo. Puede tomar un segundo parámetro (además de la función callback) para darle un valor inicial.
- `.findIndex()`: regresa el índice del primer elemento que se evalúa a true en la función callback.

<br />
Recordemos que un método es también una función, y el papel que juegan las funciones callback en los métodos de iteración es que son tomadas precisamente como el argumento de los iteradores:
<br />

```js
const cosasPorHacer = ['Sacar la basura', 'Pasear al perro', 'Lavar la ropa'];

cosasPorHacer.forEach(function(tareaPorHacer){
	console.log('- ' + tareaPorHacer);
});
```
<br />

En el ejemplo de arriba se puede observar el método `.forEach()` aplicado en el array `cosasPorHacer`. <br />
Después, toma como un argumento una **función callback**.<br />
El método de iteración `.forEach` recorre el array y ejecuta la función callback para cada elemento. Durante cada ejecución, el elemento actual es pasado como un argumento a la función de callback.<br /><br />

Existen otras maneras de hacer callback para `.forEach()`. 
Con funciones flecha

```js
cosasPorHacer.forEach(tareaPorHacer => console.log(tareaPorHacer));
```
y definiendo de antemano una función

```js
function imprimirTareas(elemento){
	console.log(elemento);
}
cosasPorHacer.forEach(imprimirTareas);
```


