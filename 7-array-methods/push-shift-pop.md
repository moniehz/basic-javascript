## Eliminando elementos de un Array
<br>

### `push()`

Permite agregar uno o más elementos al final de un array.

```jsx
let numArray = [1, 2, 3, 4]

function newNum(){
	numArray.push(6, 7)
}
```

```jsx
💡 `push()` con strings: `txtArray.push("Hola")`
```

### `shift()`

Elimina un elemento del array, `shift()` elimina el elemento que este en el índice 0.

```jsx
let shiftArray = array.shift()
```

### `pop()`

Elimina el último elemento del array.

<br>

 ## Ejemplos
 
```jsx
//push

/*Array de números*/
let numArray = [1,2,3,4,5]

functionnewNum(){
  numArray.push(6,7)
}

newNum()

// resultado [1,2,3,4,5,6,7]

/*Array de String*/
let txtArray = ["Juan", "Monse", "Daniel", "Bere"]

addCharacters();

functionaddCharacters(){
    txtArray.push("Alex", "Liliana")
    console.log(txtArray)
};

// resultado ["Juan", "Monse", "Daniel", "Bere","Alex", "Liliana")]
```

```jsx
//shift

let array = ["Juan", "Monse", "Daniel", "Bere"]

let shiftArray = array.shift();
console.log(array);

// resultado [Monse", "Daniel", "Bere"]
```

```jsx
//pop
let array = ["Juan", "Monse", "Daniel", "Bere"]

let shiftArray = array.pop();

console.log(array);
// resultado ["Juan", "Monse", "Daniel"]
```