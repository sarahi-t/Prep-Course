# JavaScript V <br /> 

JavaScript es un lenguaje orientado a objetos, pero antes de la ES6 no existían las clases. Una de las maneras de "simular" una clase, es  usando la palabra reservada `new` y `function`. <br /> 
Hoy en día se puede utilizar la palabra `class` con su respectivo constructor. 
<br /> 
1. **Prototype**<br /> 
Para hacer un clase se utiliza el patrón constructor/prototype. Primero, se crea una función que será el constructor de nuestra clase. <br /><br />
Todos los objetos en JavaScript tienen un prototype. Como las funciones son un objeto en JavaScript, automáticamente adquiere un prototype.<br /><br />
Se pueden definir métodos internamente (dentro de la función constructora), o agregarlos al prototype como en el siguiente ejemplo:
<br />

```js
function Alumno(name){ 
	this.name = name; 
} 

Alumno.prototype.getName = function () { 
	return this.name; 
}; 

var sarahi = new Alumno('Sarahi'); 
console.log(sarahi.getName()); // imprime 'Sarahi'
``` 
<br />
Al usar este tipo de patrón, todos los objetos del tipo `Alumno` comparten los métodos definidos en el prototype. También, cada objeto tiene sus propiedades: `getName()` es compartida a través de todas las instancias de la clase Alumno. <br /><br />
 
2. **Constructors** <br /> 
El constructor de una clase en JavaScript, usando el patrón de función constructora y prototipo, define las propiedades del objeto; el prototipo define los *métodos* del objeto.
<br /><br />
El constructor de prototype en la clase  del ejemplo es `Alumno`. Se define dentro del constructor la propiedad `name`, utilizando la keyword `this`.  Y, finalmente, con la palabra `new` instanciamos un nuevo objeto: `sarahi` es una instancia de `Alumno`. <br /> 

