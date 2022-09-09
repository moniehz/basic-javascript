## Operadores: Asignación, comparación y aritméticos
<br>

### De asignación

- `=` : Operador de asignación

### De comparación

- `==` : Igual que (Compara valores)
- `===` : Estrictamente igual que (compara valores y tipo de dato)
- `>` : Mayor
- `≥ or >=` : Mayor igual que
- `<` : Menor
- `≤` : Menor igual que
- `≠` : Diferente que

### Lógicos

- `!` : NOT niega un valor
- `&&` : AND
- `||` : OR


### Aritméticos

- `+` : Operador suma este se utiliza para concatener dos cadenas de texto
- `-` : Operador resta
- `*` : Operador de multicación
- `/` : Operador de devisión
- `%` : Operador de modulo
- `**` : Operador de potenciación

  Tambien se les conoce como operadores binarios. por que toman dos valores y generan un resultado.
  
 <br>
 
 ## Ejemplos
 
```jsx
//Operadores binarios:
3 + 2; //Suma
50 - 10; //Resta
10 * 20; //Multiplicación
20 / 2; //División

"Juan " + "M"; //concatenación de strings

//Operadores unitarios:
!false; //negación de la negación devolverá true
!true; //devolverá false

//Operadores de asignación:
var a = 1; //Asignamos un valor a la variable

//Operadores para comparar:
3 == "3"; //Compara los valores y devuelve "true" en este caso
3 === "3"; //Compara y valida los tipos y valores. Devuelve "falso" en este caso
5 > 3; //5 es mayor que 3 devuelve true
5 < 3; // 5 es menor que 3 devuelve false
5 >= 6; // 5 es mayor o igual 6 devuelve false
5 <= 6; // 5 es menor o igual que 6 devuelve true
5 <> 6; //5 no es igual que 6

a && b; //Valida si ambas variables son verdaderas para que se cumpla la condición
a || b; //Aquí se cumple la condición si alguna de las dos variables es verdadera

var edad = 40;
edad++; //Incrementa el valor en 1
edad += 2; //Incrementa el valor por 2
```