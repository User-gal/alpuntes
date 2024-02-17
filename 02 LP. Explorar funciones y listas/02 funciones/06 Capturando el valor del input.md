Utilizaremos input para capturar el intento del usuario

Una mejor manera de traer un objeto desde html a JS es utilizar ID's, ya que puede que tengas más de un elemento del mismo tipo dentro de tu código HTML

El HTML quedaría 
```
<input type="number" id="valorUsuario" min="1" max="10" class="container__input">
<div class="chute container__botones">
	<button onclick="verificarIntento();" class="container__boton">Intentar</button>
	<button class="container__boton" id="reiniciar" disabled>Nuevo juego</button>
</div>
```

nota como el input, tiene un identificador el cual es 'valorUsuario', de esta manera lo podremos mandar a traer con el código de JS.

Entonces el código de JS  es:

```
function verificarIntento(){
	let numeroUsuario = parseInt(document.getElementById('valorUsuario').value);
	if(numeroUsuario == numeroSecreto){
		Intrucciones
	}
}
```
Aquí se declara una variable para depositar dentro de esta el valor del input, nota que se convierte esta valor a entero, ya que el input a pesar de estar declarado como un numero en el HTML sigue siendo un valor string dentro de JS. Además de utiliza el método '.getElementByID('ID)' para llamar a el Input desde JS, y con '.value' obtenemos el valor de ese objeto.