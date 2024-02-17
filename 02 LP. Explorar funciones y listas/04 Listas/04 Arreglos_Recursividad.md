La recursividad nos permitirá llamar una función desde ella misma, esto permitirá que no tengamos que repetir una función una y otra vez con nombres distintos:

```
let listaNumerosSorteados = [];

//genera un número entre 1 y 10
function generarNumeroSecreto() {
	let numeroGenerado = Math.floor(Math.random()*10) + 1;
	//Si el numero generado ya esta en la lista volvemos a generar
	if(listaNumerosSorteados.includes(numeroGenerado)){
	//Esto es recursividad, podemos volver a llamar la función hasta cumplir con la condición
		return generarNumeroSecreto();
	} else {
		listaNumerosSorteados.push(numeroGenerado);
		return numeroGenerado;
	}
}

generarNumeroSecreto();
```

1. En la primera ejecución se generar un número entre 1 y 10, despues de generar el numero pasaremos por el If, la condición es ``` listaNumerosSorteados.includes(valorBuscado);``` buscará en la lista el argumento  dado, por lo tanto devolvera 'True' si lo encuentra y 'False' si no lo encuentra.
2. Si el numero generado se encuentra en la lista entonces entra al ```return generarNumeroSecreto();``` esto provocará que de manera recursva se genere un nuevo valor,  y solo saldrá de esta recursividad hasta encontrar un nuevo valor. 
3. Si no encuentra el valor, pasa al else, donde primero se utiliza el código ``` listaNumeroSorteados.push(valorAAgregar) ``` para agregar a la lista el valor generado y después se devuelve el valor generado.

En este caso solo podemos jugar 10 veces, ya que una vez generados los valores del 1 al 10 no habrá manera de salir de la recursividad, es por eso que debemos tener en cuenta las limitaciones de nuestros procesos.
