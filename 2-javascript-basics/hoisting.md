## Hoisting
<br>

En JavaScript, las declaraciones (por ejemplo, de variables o funciones) se mueven al principio de su scope o ámbito. Este comportamiento se conoce como hoisting y es muy importante tenerlo en cuenta a la hora de programar para prevenir posibles errores.
- Las funciones siempre se mueven arriba del scope. Por lo tanto, podemos elegir donde declararlas y usarlas.
- La declaración de las variables se mueven arriba del scope, pero no la asignación. Antes de usar una variable, habrá que crearla y asignarla.
El Hoisting funciona de ECMAScript 5 para abajo, de ECMAScript 6 en adelante no sucede porque el Hoisting sucede con var y function. En las versiones de ECMAScript 6 en adelante aparece const y let.

<br>

 ## Ejemplos
 
```jsx
//Ej. 1 Lo que nosotros ponemos:
console.log(miNombre);

var miNombre = "Juan";

//Lo que enrealidad sucede por el Hoisting:
var miNombre;

console.log(miNombre); //Devuelve un undefined

miNombre = "Juan"; //Recien aqui se inicializa la variable


//Ej. 2 Lo que nosotros ponemos:
sumar();
var x = 2;
function sumar(){
    var suma = x + y;
    return suma;
}
var y = 1;

//Lo que en realidad sucede por el Hoisting:
function sumar(){
    var suma = x + y;
    return suma;
}  
var x = 2;
var y = undefined;
sumar();
var y = 1;
//Primero se cargan las funciones, segundo la declaración de variables y el resto en el orden normal del código.
```