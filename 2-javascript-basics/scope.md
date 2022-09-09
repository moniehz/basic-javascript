## Scope
<br>

Es elcance que tienen las variables en el código.

### Variables globales

Pueden ser accedidas desde un scope local o global. Las variables globales son definidas fuera de las funciones (Scope global).

### Scope local

Son aquellas variables definidas dentro del cuerpo de la función, estas son solo accedidas desde dentro de la misma función.

### Scope global
Variables que pueden ser accedidas y procesadas por cualquier función dentro del código.

 <br>
 
 ## Ejemplos
 
```jsx
//Scope global:
var miNombre = "Juan";

//Scope local:
function nombre(){
    var miApellido = "M";
    console.log(miNombre + " " + miApellido);
}

nombre(); //Devuelve "Juan M"
```