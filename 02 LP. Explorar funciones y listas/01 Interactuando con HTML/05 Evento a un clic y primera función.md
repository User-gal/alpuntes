Cada acción dentro de tu página se llama evento

Presionar un botón
Pasar el mouse sobre algún elemento

Todos los eventos en html empiezan como 'on'

por ejemplo si en nuestro html tenemos una etiqueta de botón

```
<button onclick="alert("Presinaste el botón");" class="container_boton">Intentar</button>
```

Nosotros tenemos un botón que al ser presionado nos mostrará un mensaje, sin embargo, esta forma de trabajo hará que nuestro código sea cada vez más difícil de leer, es por eso que como alternativa a esto, usamos una llamada a una función la cual sera programada para ejecutar los pasos a seguir después ejecutar la acción.

el HTML quedaría

```
<button onclick="intentoUsuario();" class="container_boton">Intentar</button>
```

entonces el JavaScript quedaría

```
function intentoUsuario(){
	alert("Presionaste el botón");
}
```

La estructura para declarar una funcion es:

```
function nombreDeLaFuncion(argumentos){
	Instrucciones
	...
}
```
