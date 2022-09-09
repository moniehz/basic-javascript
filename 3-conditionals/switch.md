## Switch
<br>

Básicamente, un `switch` es como un IF, pero diferente en su sintaxis y su uso, pero fuera de algunas ocasiones son muy parecidos.

- La sintaxis de switch es:

```jsx
switch('valor a validar') {
    case 'opción 1':
    'acción a realizar';
    break;
}
```
El uso de `break` es importante, si no se le agrega accionará todas las opciones dentro del switch.

<br>

 ## Ejemplos

 ```jsx
 let dia = "Martes";

switch(dia) 
{
	case "Lunes":
		console.log("Hoy es Lunes");
		break;
	case "Martes":
		console.log("Hoy es Martes");
		break;
	case "Miercoles":
		console.log("Hoy es Miercoles");
		break;
	case "Jueves":
		console.log("Hoy es Jueves");
		break;
	case "Viernes":
		console.log("Hoy es Viernes");
		break;
	case "Sabado":
		console.log("Hoy es Sabado");
		break;
	case "Domingo":
		console.log("Hoy es Domingo");
		break;
	default:
		console.log("Es el fin de los dias");
}
 ```

En el caso de que ninguna de las opciones dentro del switch sea la correcta, tenemos 2 opciones por hacer que son:

- Dejar el código seguir sin hacer nada.
- Utilizar default que es como si utilizáramos un else pero para switch.