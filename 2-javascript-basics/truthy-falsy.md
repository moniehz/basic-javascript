## Valores: Truthy y Falsy
<br>

Valores que por default son falso (falsy) o verdadero (truthy).
<br>

 ### Ejemplos en los que Boolean devuelve falso:
 
```jsx
Boolean(0); //false
Boolean(null); //false
Boolean(NaN); //false
Boolean(undefined); //false
Boolean(false); //false
Boolean(""); //false
```

### Ejemplos en los que Boolean devuelve verdadero:
 
```jsx
Boolean(1); //true para 1 o cualquier número diferente de cero (0)
Boolean("a"); //true para cualquier caracter o espacio en blanco en el string
Boolean([]); //true aunque el array esté vacío
Boolean({}); //true aunque el objeto esté vacío
Boolean(function(){}); //cualquier función es verdadera también
Boolean(-1); //true
Boolean(true); //true
```