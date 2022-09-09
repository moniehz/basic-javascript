## Objects: Función constructora
<br>

Función donde podremos crear nuevos objetos por medio de los parámetros de la función

```jsx
function Auto(marca, modelo, year){
	this.marca = marca;
	this.modelo = modelo;
	this.year = year;
}
```

### Instancia: 
Genera un objeto que deriva de otro.

```jsx
var AutoNuevo = new Auto("Tesla", "Model 3", 2021)
```

<br>

```jsx
💡 let: Declara una variable de alcance local con ámbito de bloque
```

```jsx
💡 prompt(): Input
```

<br>

 ## Ejemplos
 
```jsx
function autos(marca, modelo, annio){
    this.marca = marca;
    this.modelo = modelo;
    this.annio = annio;
}

var marcaArray = ["TESLA", "NISSAN", "TOYOTA", "HONDA"];
var modeloArray = ["2020", "MODEL X", "COVID19"];
var annioArray = [2018, 2019, 2020];

for(var i=0; i<=30; i++){
    var random0 = Math.floor(Math.random() * marcaArray.length);
    var marca = marcaArray[random0];
    var random1 = Math.floor(Math.random() * modeloArray.length);
    var modelo = modeloArray[random1];
    var random2 = Math.floor(Math.random() * annioArray.length);
    var annio = annioArray[random2];
    var autoNuevo = new autos(marca, modelo, annio);
    console.log(autoNuevo);
}
```