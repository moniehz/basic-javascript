## Condicionales: If, Else, else if
<br>

Son un conjunto de reglas para validar si algo es verdadero o falso y podamos generar ciertas acciones de acuerdo al resultado de la condición.

### `IF`

La estructura sería:

```jsx
if() { 
    
}
```

- Dentro de los paréntesis () se evaluaría si algo es verdadero o falso.
- Dentro de las llaves {} se encuentra la tarea a generar si la condición es verdadera.
- Si lo que se está evaluando resulta falso, lo que está dentro de las llaves no se ejecuta, queda ignorado.

### `IF...ELSE`

La estructura sería:

```jsx
if() { 
    
} else {

}

```

- Dentro de los paréntesis () se evaluaría si algo es verdadero o falso.
- Dentro de las primeras llaves {} se encuentra la tarea a generar si la condición es verdadera.
- Si lo que se está evaluando resulta falso, lo que está dentro de las primeras llaves no se ejecuta, queda ignorado, pero se ejecuta lo que está dentro de las llaves de else, sería el default del if.

### `ELSE IF`
La estructura sería:

```jsx
if() { 
    
} else if (){

} else {

}
```

- Dentro de los primeros paréntesis () se evaluaría si algo es verdadero o falso.
- Dentro de las primeras llaves {} se encuentra la tarea a generar si la primera condición es verdadera.
- Si lo que se está evaluando resulta falso en la primera condición if, lo que está dentro de las primeras llaves no se ejecuta, queda ignorado, pero se evalúa la segunda condición else if.
- Si dentro de los paréntesis del else if resulta verdadero, se ejecuta lo que está dentro de las llaves {}, de ser falso sería el default y se ejecutaría la tarea del último else.

### `Operador ternario`

La estructura sería:

```jsx
condition ? true : false; 
```

- Inicialmente se encuentra condition, ahí se coloca la condición a evaluar.
- Después del signo de cierre de interrogación ? se encuentra la tarea a ejecutar si resulta verdadera la condición evaluada.
- Después del signo de dos puntos : se encuentra la tarea a ejecutar de resultar falsa la condición evaluada.

<br>

 ## Ejemplos
 
 ```jsx
 //Condicional IF
 var esUsuario = true;

if(esUsuario) {  //con el if validamos que la condición sea true
    console.log('Tiene acceso al contenido');  //dado que esUsario es verdadero se puede imprimir el mensaje
}

var esUsuario = false; 

 //Condicional IF...ELSE
if(esUsuario) {
    console.log('Tiene acceso al contenido');  //la condición resultó verdadera
} else {
    console.log('Tienes que crear una cuenta para poder acceder al contenido'); //la condición resultó falsa
}

//Condicional ELSE IF
var edad = 18; 
var accion;  

if(edad === 18) {
    accion = 'Puede votar, será su 1ra votación'   //en la primera condición fue verdadera
} else if(edad > 18) { 
    accion = 'Puede votar'   //la segunda condición fue verdadera, no la primera
} else { // call back 
    accion = 'Aun no puede votar'   //ni la primera ni la segunda condición resultaron verdaderas, por lo que se ejecutó el "default"
}

console.log(accion);

//Operador ternario
var numero = 1; 
var resultado = numero === 1 ? 'Sí soy un 1' : 'No soy un 1';

console.log(resultado);  //dado que numero es igual a 1, console.log imprime el primer mensaje: "Si soy un 1"
```