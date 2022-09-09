## Métodos de recorrido de arrays
<br>

### `filter()`

Ayuda a filtrar cosas específicas de nuestro array, generando un nuevo array.

```jsx
var articulos = [
	{nombre: "Bici", costo: 3000},
	{nombre: "TV", costo: 5000},
	{nombre: "Libro", costo: 200},
]

var articulosFiltrados = articulos.filter(function(articulo){
	return articulo.costo <= 500;
})
```

### `map()`

Permite mapear todo el contenido del array y nos trae lo que queremos en otro array.

```jsx
var nombreArticulos = articulos.map(function(articulo){
	return articulo.nombre;
})
```

### `find()`

Ayuda a encontrar un objeto del array creando un nuevo array por medio de la validación.

```jsx
💡 A diferencia de `filter()`, `find()` devuelve el primer elemento que encuentra. `filter()` devuelve todos.
```

### `foreach()`

Permite filtrar en nuestro array sin la necesidad de crear otro.

```jsx
articulos.forEach(function(articulo){
	console.log(articulo.nombre)
})
```

### `some()`

Valida si un objeto o propiedades existen en el array, devuelve `true` o `false`.

```jsx
var articulosBaratos = articulos.some(function(articulo){
	reutrn articulo.costo <= 700;
})
```

### `every()`

Este método checa que todos los elementos en el array cumplan con la validación que ponemos, y al final nos regresa un true o un false .

```jsx
var articulosBaratos = articulos.every(function(articulo){
    return articulo.costo <= 700;
});

console.log(articulosBaratos); 
```

### `reduce()`

Este método corre una función en cada elemento del array, para comenzar a sumar los costos de cada elemento.

```jsx
var costoTotal = articulos.reduce(function(totalActual, articulo){
    return articulo.costo + totalActual;
}, 0); // El 0 será la cantidad inicial con la que comenzará el totalActual

console.log(costoTotal); 
```

### `includes()`

Esto nos permite verificar si un elemento está presente en una matriz (incluido NaN, a diferencia de indexOf).

```jsx
var numeros = [1, 2, 3, 4, 5, 6];

var incluyeNumero = numeros.includes(2); 

console.log(incluyeNumero);
```

<br>

 ## Ejemplos
 
```jsx
var articulos = [
    { nombre: "Bici", costo: 3000 },
    { nombre: "TV", costo: 2500 },
    { nombre: "Libro", costo: 320 },
    { nombre: "Celular", costo: 10000 },
    { nombre: "Laptop", costo: 20000 },
    { nombre: "Teclado", costo: 500 },
    { nombre: "Audifonos", costo: 1700 },
];

//filter Genera un nuevo array
var articulosFiltrados = articulos.filter(function(articulo){
    return articulo.costo <= 500; //articulos con precio menor a 500 pesos
});

//map Ayuda a mapear ciertos elementos de los articulos, es necesario generar nuevo array
var nombreArticulos = articulos.map(function(articulo){
    return articulo.nombre;
});

//find Ayuda a encontrar algo dentro del array articulos
var encuentraArticulo = articulos.find(function(articulo){
    return articulo.nombre === "Laptop";
});

//forEach No es necesario generar nuevo array, se utiliza para realizar un recorrido de un array principal
articulos.forEach(function(articulo){
    console.log(articulo.nombre);
});

//some Se genera nuevo array, regresa un condición en Boolean
var articulosBaratos = articulos.some(function(articulo){
    return articulo.costo <= 700;
});```
```