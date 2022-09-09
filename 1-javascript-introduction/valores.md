## Valores
<br>

Existen 2 componentes importante en JS:
- Valores o datos: Almacenan informacion 
- Funciones: Realizan acciones con la informacion.

### Valores primitivos

Tipo de dato más básico en JS, son inmutables y contienen un único valor.

- **Number**: Valores numéricos.
- **String**: Cadena de caracteres, se coloca entre comillas dobles.
- **Boolean**: Valor lógico, puede ser True o False.
- **Empty values**: Se les conoce como valores "placeholder" pero son para variables sin valor.

### Valores no primitivos o tipo de objetos

- **Array**: Se genera con corchetes `[]` los cuales dentro ocupan valores primitivos `[1, 2, 3]`
- **Objeto**: Se generan con llaves `{}` y dentro llevan data que se convierte en objeto `{nombre: "Sofía"}`


Para comprobar los tipos de valores usamos la función "typeof". 
<br>
`typeof true; //boleaan`

<br>

## Ejemplos
 
```jsx
//Primitivos

const name = 'Juan M'; //String
const age = 45; //Number
const hasKids = true; //Boolean
const car = null; //Null
let test; // Undefined
const sym = Symbol(); //Symbol

//Objetos

const hobbies = ['movies', 'music']; //Array
const address = {
    city: 'Boston',
    state: 'MA'
}

const today = new Date();
console.log(today);
console.log(typeof today);
```