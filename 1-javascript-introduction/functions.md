## Funciones en JavaScript
<br>

Una función es un procedimiento en JavaScript, un conjunto de sentencias que realizan una tarea o calculan un valor. Para usar una función, debe definirla en algún lugar del ámbito desde el cual desea llamarla.

La declaración de una función consiste de la palabra reservada `function`, seguida por:
- El nombre de la función (opcional).
- Una lista de argumentos para la función, encerrados entre paréntesis y separados por comas.
- Las sentencias JavaScript que definen la función, encerradas por llaves.
- Las funciones que no tienen especificado el retorno con la palabra reservada `return`, regresarán `undefined`.

<br>

Existen 2 tipos de funciones
### 1) Declarativas (function declaration / function statement): 
- Se declaran directamente. 
- Utilizamos la palabra reservada function al inicio para poder declarar la función.
<br>

```jsx
function miFuncion1()
{
    return;
}
```

### 2) De expresión (function expression / funciones anónimas): 
- Se guardan en una función.
- La declaración se inicia con la palabra reservada var, donde se generará una variable que guardará una función anónima.
<br>

```jsx
var miFuncion2 = function()
{
    return;
}
```

### Diferencias:

A las funciones declarativas se les aplica hoisting, y a la expresión de función, no. Ya que el hoisting solo se aplica en las palabras reservadas var y function.
Lo que quiere decir que con las funciones declarativas, podemos mandar llamar la función antes de que ésta sea declarada, y con la expresión de función, no, tendríamos que declararla primero, y después mandarla llamar.

El hoisting se refiere a que las declaraciones de variables y funciones es movido al principio del código, pero lo que ocurre en realidad es dichas declaraciones son almacenadas en memoria.
- Funciones declarativas: Son asignadas a la memoria por lo que la podemos llamar antes sin problemas.
- Funciones de expresión: NO son asignadas en memoria por lo que no pueden ser llamadas antes.

<br>

Existe un tipo de declaración en los parámetros de una función en el cual no se necesitan especificar el número de parámetros que se van a recibir, eso se hace de la siguiente manera:
```jsx
const imprimeArgumentos = function(...args) 
{
    return args;
};
```

<br>

## Ejemplos
 
```jsx
//De expresión con parámetros
var miFuncion3 = function(a,b)
{
    return a + b;
}

//Llamando una función.
miFuncion1();
miFuncion2();
miFuncion3(1,2);

//Uso de parámetros de una función.
var estudiante = "Juan"
saludarEstudiante1(estudiante);
saludarEstudiante2(estudiante);

function saludarEstudiante1(estudiante)
{
    //template strings `texto ${variable}`
    console.log(`Hola ${estudiante}`);
}

function saludarEstudiante2(estudiante)
{
    console.log("Hola " + estudiante);
}

//Uso de parámetro de una función con return
var num1 = 10;
var num2 = 25;

console.log("Resultado: " + sumar(num1,num2));

function sumar(x,y){
    var resultado = x + y;
    return resultado;
}

// Trabajar con los argumentos en una función de flecha
const imprimeArgumentos = function(...args) 
{
    return args;
};

imprimeArgumentos(10, true, false, "Juan", "Hola");
```