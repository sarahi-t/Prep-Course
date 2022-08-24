# JavaScript IV <br />

1. **Objetos** <br />
Los objetos son un tipo de dato en JavaScript que contienen datos y funcionalidades relacionadas. Están organizados como pares *key: value*, donde key representa un nombre y value lo que se guarda en  él. Un objeto puede ser asignado a una variable, y sus elementos son separados con una coma (`,`) entre llaves (`{}`): <br />
`let dog = {}; // un objeto variable dog` <br />
`const dog = {}; //un objeto constante dog`  <br />
Cuando un objeto es `const`, no puede ser reasignado en su totalidad, pero se le pueden hacer modificaciones a sus propiedades.
<br />

2. **Propiedades** <br />
Las propiedades de los objetos pueden ser accedidas y también modificarse. Se utilizan dos diferentes notaciones para acceder a una propiedad: con punto (`.`) y corchetes (`[]`). La sintaxis es `objeto.key;` u `objeto[key];` <br />
La asignación se realiza con el signo de igual a (`=`). Si no existe el par dentro del objeto, se crea; y de existir, se reasigna. La sintaxis es la siguiente: `objeto.key = value;` o en su defecto `objeto[key] = value;`.
<br />

3. **Métodos** <br />
Una propiedad es lo que tiene un objeto, y un método es lo que *hace*. A una función dentro de un objeto se le conoce como método. <br />
Se pueden incluir métodos en un objeto como cualquier par key: value, separados por comas. Y como cualquier función, se pueden mandar a llamar. La key de cada método será el nombre de la función y el valor es una function expression anónima. <br />
```
const dog = {
	ladrar: function () {
	console.log('Woof!');
	}
};
```
<br />

Esto se puede simplificar gracias a la sintaxis ES6. Se puede omitir la keyword de `function`. El nombre de la función es la key dentro del objeto:
```
const dog = {
	ladrar () {
	console.log('Woof!');
	}
};
```
<br />

4. **Bucle** `for...in` <br />
Existe una manera sencilla para iterar en los objetos. La sintaxis `for...in` ejecuta un bloque de código por cada propiedad en un objeto.
<br />

5. **Notación de puntos VS notación de corchetes** <br />
Para no caer en un error, se debe utilizar la notación de corchetes cuando se intenta acceder a keys que tienen números, espacios o caracteres especiales. <br />
<br />
