## Loops: While
<br>

### WHILE

El bucle while recorre un bloque de código siempre que una condición especificada sea verdadera.

- En un bucle `while` la variable es declarada antes del loop y es accedida al estar en el scope global.
- Empieza el bucle con la palabra `while` seguida de la condición de parada o condición a evaluar. Esta será evaluada antes en cada ronda del bucle. Mientras la condición evalué `true`, el bloque seguirá corriendo. Una vez que evalué `false` el bucle se detendrá.
- Finalmente tenemos el bloque de código del bucle.

Sintaxis:
```jsx
while (condition) {
  // code block to be executed
}
```

<br>

### BUCLE DO WHILE

El bucle  do while es una variante del bucle while. Este ciclo ejecutará el bloque de código una vez, antes de verificar si la condición es verdadera, luego repetirá el ciclo mientras la condición sea verdadera.

Sintaxis:
```jsx
do {
// code block to be executed
}
while (condition);
```

<br>

 ## Ejemplos
 
```jsx
var estudiantes = ["Juan", "Monse", "Daniel", "Bere"];

function saludarEstudiante(estudiante) {
    console.log(`Hola ${estudiante}`);
}

var i = 0;

//do-while
do {
    saludarEstudiante(estudiantes[i]);
    i++;
} while (i < estudiantes.length)

do {
    var estudiante = estudiantes.shift();
    saludarEstudiante(estudiante);
} while (est

//while
while (estudiantes.length > 0) {
    var estudiante = estudiantes.shift();
    saludarEstudiante(estudiante);
}
```