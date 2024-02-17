Dentro del CSS los elementos

h1, p, etc... se llaman selectores, es decir nos permiten definir que es lo que vamos a formatear.


La propiedad background nos modifica el color del fondo de un elemento.

Lo podemos asignar a los selectores de manera individual

```
	h1{
		background: #CCCCCC;
	}
	p{
		background: #CCCCC;
	}
	

```

o bien utilizar una etiqueta más global.

```
	body{
		background: #CCCCCC;
	}
```

nosotros también podemos seleccionar alguna etiqueta en particular como por ejemplo

```
strong{
	color: red;
}
```

![[Pasted image 20240128170025.png]]
esto le daría el colo rojo a todas las étiquetas strong, sin embargo si quiero que sea un elemento en particular podría decirle a css lo siguiente

```
em strong{
	color: red;
}
```

Esto solo aplicará el color rojo **al strong que se encuentre dentro de un em.**
![[Pasted image 20240128170113.png]]
