## Objects
<br>

Un objeto es una estructura de datos (al igual que los array), con la diferencia que en los objetos no existe el índice numérico, lo que hay son propiedades, con ellas accedemos a cada uno de los valores.

Los valores del objeto pueden ser de todo tipo, es decir que podemos tener un number, un string, una función, un array, incluso otro objeto que contenga otros valores.

Un objeto sería:
```jsx
var MiAuto = {
	marca: "Toyota",
	modelo: "Corola",
	year: 2020
}
while (condition);
```

Es posible agregar propiedades que sean funciones:
```jsx
var MiAuto = {
	detalles: function(){
		console.log(`Auto ${this.modelo} ${this.year}`)
	}
}
```

<br>

 ## Ejemplos
 
```jsx
var miLaptop = {
    Modelo: "15-dw0004la",
    Procesador: "Intel Core i7",
    MemoriaRAM: "8GB",
    DiscoDuro: "256GB",
    Peso: "1.74 kg",
    caracteristicas: function(){
        console.log(`Mi laptop tiene las siguientes caracteristicas ${this.Modelo} ${this.Procesador} ${this.MemoriaRAM} ${this.DiscoDuro} ${this.Peso}`)
    }
}

miLaptop.caracteristicas()
```