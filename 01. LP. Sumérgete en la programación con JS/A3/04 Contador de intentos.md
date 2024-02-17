Los contadores, nos permiten almacenar el número de veces que has repetido un loop o bucle.
Esta tiene que ser declarada antes del loop y de preferencia inicializarla.
El valor inicial para esa variable lo determinas a partir de la lógica de programación empleada en tu código.

```
let intentos = 1
let palabra = "intento"

while(numeroSecreto != numeroUsuario){
	numeroUsuario = prompt("Me indicas un entre 1 y 10 por favor:");
	if(numeroSecreto == numeroUsuario) {
		alert(`Acertaste el numero secreto es: ${numeroUsuario}. Necesitaste ${intentos} ${palabra} para lograrlo`);
	} else {
		if(numeroSecreto > numeroUsuario){
			alert(`El numero secreto es mayor`);
		} else {
			alert(`El numero secreto es menor`);
		}
	}
	intentos = intento + 1;
	palabra = "intentos"
}

```

Para poder incrementar el valor de la variable intentos hacemos uso de la instrucción

`intentos = intentos + 1`

Lo que permite sumar al valor de intentos 1 y guardar el resultado en la misma variable.
