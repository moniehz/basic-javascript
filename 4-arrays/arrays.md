## Arrays

### ¿Qué es?

Tipo de estructura de datos que guarda varios datos del mismo tipo dentro.

### Elementos de arrays
- `.length()` Devuelve la longitud del array.
- `.push()` Agrega elementos al final del array.
- `.pop()` Elimina un elemento del array (el del final).
- `.unshift()` Agrega elementos al inicio del array.
- `.shift()` Elimina el elemento al inicio del array.
- `.indexOf()` Devuelve la posición de un elemento.
<br>

### Mas elementos de arrays

```jsx
var colores = ["rojo", "azul", "verde", "amarillo"];
```

<br>

`Reverse`: Invierte los elementos del array.

```jsx
colores.reverse();
//["amarillo", "verde", "azul", "rojo", "anaranjado"]
```

<br>

`Sort`: Ordena alfabeticamente los datos, sin importar su tipo de dato.

```jsx
colores.sort();
//["amarillo", "anaranjado", "azul", "rojo", "verde"]
```

<br>

`Slice`: Método que puede contener uno o dos argumentos que indiquen el inicio y parada de posiciones, pues devuelve los elementos contenidos en el array de acuerdo a los argumentos indicados, por ejemplo si a colores le agregamos `colores.slice(1,3);` obtendremos los que se encuentran en la posición 1, 2.

```jsx
colores =  ["amarillo", "anaranjado", "azul", "rojo", "verde"]
colores.slice(1,3);
//["anaranjado", "azul"]
```

Si solo se indica un argumento se tomará como inicio ese argumento y como final la última posición, entonces si usamos:

```jsx
colores.slice(2);
//["azul", "rojo", "verde"]
```

<br>

 ## Ejemplos
 
```jsx
var frutas = ["Manzana", "Plátano", "Cereza", "Fresas"];

console.log(frutas);

console.log(frutas.length); //Longitud o número de elementos
console.log(frutas[n]); //Acceder al elemento por medio de index

//Mutar o alterar Array
var masFrutas = frutas.push("Uvas") //Añadir elementos al final del array
var ultimo = frutas.pop() //Eliminar el último elemento del Array
var nuevaLongitud = frutas.unshift("Uvas"); //Añadir elemento al inicio del array
var borrarFruta = frutas.shift("Uvas"); //Borra el primer elemento
var posicion = frutas.indexOf("Cereza"); //Devuelve el index o posicion del elemento
```