## Coerción
<br>

Es la forma en la que podemos cambiar un tipo de valor a otro.

Existen dos tipos:
- Implícita: Es cuando el lenguaje nos ayuda y cambia de un tipo de valor a otro tipo de valor.
- Explícita : Es cuando nosotros obligamos a un valor de un tipo a cambiar a otro tipo.

<br>

 ## Ejemplos
 
```jsx
var a = 4 + "7"; //Convierte a 4 en un string y lo concatena con el "7", por esto regresa un string de valor "47"

4 * "7"; //Convierte al "7" en un número y realiza la operación, por esto devuelve 28

var a = 20;
var b = a + ""; //Aquí concatenamos para convertir la variable a string (coerción implícita)
console.log(b); 

var c = String(a); //Aquí obligamos a la variable a convertirse en string (coerción explícita)
console.log(c);

var d = Number(c); //Aquí obligamos a la variable a convertirse en número (coerción explícita)
console.log(d);
```