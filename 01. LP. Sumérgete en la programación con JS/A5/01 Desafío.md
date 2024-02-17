Hacer que se pueda variar el número máximo a adivinar.

```
let numeroMaximo = parseInt(prompt("¿Cuál es el número máximo a buscar?"))

let numeroSecreto = Math.floor(Math.random() * numeroMaximo) + 1;

console.log(typeof(numeroSecreto));

console.log(numeroSecreto);

console.log(numeroMaximo);

let numeroUsuario = numeroSecreto + 1;

let intentos = 1;

//Cambio esto por el operador ternario

//let palabra = "intento"

let maximointentos = 3;

  
  
  

while(numeroSecreto != numeroUsuario){

numeroUsuario = parseInt(prompt(`Me indicas un entre 1 y ${numeroMaximo} por favor:`));

  

//alert('Hola Mundo!!');

  

//console.log(numeroUsuario);

  

if(numeroSecreto == numeroUsuario) {

alert(`Acertaste el numero secreto es: ${numeroUsuario}. Necesitaste ${intentos} ${intentos == 1 ? 'intento' : 'intentos'} para lograrlo`);

break;

} else {

if(numeroSecreto > numeroUsuario){

alert(`El numero secreto es mayor`);

} else {

alert(`El numero secreto es menor`);

}

}

intentos++;

//palabra = "intentos"

if( intentos > 3){

alert(`Llegaste al numero máximo de intentos que es: ${maximointentos}`);

break;

}

}
```
