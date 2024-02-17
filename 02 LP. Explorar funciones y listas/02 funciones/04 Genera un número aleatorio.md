Se vuelve a agregar el código para generar el número aleatorio mediante una function.

Con el concepto de función se pueden agregar nuevas caracteristicas a esta función original.

recordando el código para generar el número aleatorio entre 1 y 10.
```
let numeroAleatorio = Math.floor(Math.random()*10) + 1;
```

La utilizaremos dentro de una función

de una manera larga sería

```
function generarNumeroSecreto(){
	let numeroAleatorio = Math.floor(Math.random() * 10) + 1 ;
	return numeroAleatorio;
}

let adivinaNumero = generarNumeroSecreto();
```

el return devuelve la variable asignada al lugar donde es llamada la fución(una variable)

sin embargo una manera más correcta de hacer este proceso es 

```
function generarNumeroSecreto(){
	return Math.floor(Math.random() * 10) + 1 ;
}

let numeroSecreto = generarNumeroSecreto();
```

