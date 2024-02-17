Es una secuencia de instrucciones de código que se ejecuta repetidas veces, hasta que la condición asignada a dicho bucle deja de cumplirse.

Comúnmente hacen uso de un flag(variable) que permitirá salir de este bucle, si no hay una condición que permita salir, el código podría caer en un ciclo infinito.

La sentencia while permite ejecutar una instrución o grupo de instrucciones hasta que se cumpla una condición dada. Su estructura es:

```
while(Condición){
	Instrucciones
}
```

El bloque de instrucciones se ejecutará hasta que la condición se cumpla.  En el ejemplo del curso repetimos la petición de números hasta encontrar el correcto.
```
while(numeroSecreto != numeroUsuario){
	numeroUsuario = prompt("Me indicas un entre 1 y 10 por favor:");
	
	if(numeroSecreto == numeroUsuario) {
		alert(`Acertaste el numero secreto es: ${numeroUsuario}`);
	} else {
		if(numeroSecreto > numeroUsuario){
			alert(`El numero secreto es mayor`);
		} else {
			alert(`El numero secreto es menor`);
		}
	}
}
```


> [!NOTE] Indenta tu código
> La indentación es anidar el código que pertenezca a otra instrucción, en JS se puede identificar por que es el código que queda dentro de las { }.
> Se hace presionando la tecla tabulador.
> Esto permitirá que la lectura del código sea mucho más secillo.
