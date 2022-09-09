## Variables en JavaScript
<br>

Dentro de JS tenemos tres formas de declarar una variable las cuales son: `var`, `const` y `let`.

### Var

Es una variable que puede cambiar su valor en un futuro y su alcance es local. Sin embargo, puede ser global y local dependiendo de dónde se utilice. Por ejemplo, dentro de una función es una variable local y fuera de esta misma es una variable global. Surgió en ECMAScript5.

- Se puede reinicializar
- Se puede reasignar
- Su alcance es función global

### Const

Es una variable constante que no puede cambiar nunca su valor en un futuro.

- No se pueden reinicializar
- No se pueden reasignar
 - No es inmutable

### Let

Es una variable que puede cambiar su valor pero solo funciona en un bloque donde se declare ( {let} )

- No se puede reinicializar
- Se puede reasignar
- Su contexto es de bloque
 
 <br>
 
 ## Ejemplos
 
```jsx
//Let es una variable local
let valorUno = 10;
if (true) {
    let valorUno = 40; //let es una variable local por lo cual no tomara este valor
    console.log(valorUno)
}
console.log(valorUno);


//Es un valor constante que no puede ser cambiado
const valorConstante = "Monse";
console.log(valorConstante);

//Var es una variable global
var valorDos = 20;
if (true) {
    var valorDos = 40;  //El var es una variable global por lo cual tomara el nuevo valor
    console.log(valorDos);
}
console.log(valorDos);

//Valores vacíos
let valorVacio = null;
let valorIndefinido = undefined;

let nombre = "Monse";
console.log(typeof nombre);

const nombres = {
    nombre : "Monse",
    nombreDos : "Juan",
}
console.log(nombres.nombre);
console.log(nombres.nombreDos);

const numeros = [10,20,30,40,50];
console.log(numeros[2]);
```