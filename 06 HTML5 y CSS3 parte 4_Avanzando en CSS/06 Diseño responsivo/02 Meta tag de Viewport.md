Una página responsiva es aquella que se consigue adaptar a la pantalla del dispositivo en el cual se cargue, sea este una computadora, tableta, pantalla o teléfono. 

Debemos preocuparnos siempre de esto, en particular con teléfonos, ya que hoy día la gran mayoría de las personas se conectan a través del mismo.

Desde la vista de desarrollador podemos simular pantallas de móviles.

Para considerar esta variante, agregamos a nuestro HTML en el header

```
<meta name="viewport" content="width=device-width">
```

Y en el CSS creamos un media query  que nos creará excepciones de estilo cuando se cumplan ciertas condiciones

```
/* Querys responsivos*/

@media screen and (max-width:480px) {
	body{
		background: red;
	}
}
```
