## Loops: For y For...of
<br>

Los bucles pueden ejecutar un bloque de código varias veces. JavaScript admite diferentes tipos de bucles:

- `for` Recurre un bloque de código varias veces.
- `for/in` Recorre las propiedades de un objeto.
- `for/of` Recorre los valores de un objeto iterable.
- `while` Recorre un bloque de código mientras se cumple una función específica.
- `do/while` Recorre un bloque de código mientras se cumple una función específica.

<br>

### BUCLE FOR

Se utiliza para repetir una o más instrucciones un determinado número de veces. El FOR se suele utilizar cuando sabemos seguro el número de veces que queremos que se ejecute.

Para iniciar un `for` , debe tomarse en cuenta 4 cosas:

- El `init`, que se ejecutará una vez cuando comience el ciclo. Aquí es donde normalmente inicializamos una variable y la usamos como contador de bucle, Aunque se puede ingresar cualquier fragmento de código.
- En segundo lugar, el `condition`. Esto lo que hará es comprobar si se cumple dicha condición en cada ejecución y seguirá repitiendo hasta que se vuelva falso.
- El `increment` se ejecutará después de cada ejecución del ciclo. Usualmente usamos esto para incrementar el contador de bucles, pero esto también puede ser cualquier fragmento de código o estar totalmente vacío.
- Finalmente, debe especificar el `statements(código)` para que se ejecute en bucles.

Sintaxis:
```jsx
for (INIT; CONDITION; INCREMENT) {
  STATEMENTS
}

/*
for (let i=0; i<10; i++) {
  console.log(i);
}>
*/
```

<br>

### BUCLE FOR OF

Ejecuta un bloque de código para cada elemento de un objeto iterable, como lo son: String, Array, objetos similares a array.

Sintaxis:
```jsx
for (const valor of objetoIterable) {
  console.log(valor);
}
```

<br>

 ## Ejemplos
 
```jsx
var estudiantes = ["Juan", "Monse", "Daniel", "Bere"];

//tarea que va a se nuestro loop, que saludará a los estudiantes
function saludarEstudiantes(estudiante){
   console.log(`Hola, ${estudiante}`);
}

//For se divide en 3 pasos:
//1. genero variable igual a cero
//2. Variable mientras sea menor que el array estudiante
//3. i se va a aumentar por un numero
for(var i = 0; i < estudiantes.length; i++ ){
    saludarEstudiantes(estudiantes[i]); //imprime el array estudiante
}


//Otra forma de trabajar el for, recorrerlo por elemento
for (var estudiante of estudiantes){
    saludarEstudiantes(estudiante);
}
//Salida: Hola, Juan
//		  Hola, Monse
//		  Hola, Daniel
//		  Hola, Bere
```