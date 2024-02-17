Para poder agregar un evento de clic sobre un elemento modificamos la propiedad de nuestro css de la siguiente manera

El evento es `active` y se vería deflejado de la siguiente manera

```
.productos li:hover{
	border-color: #C78C19;
}

.productos li:active{
	border-color: green;
}
```


Además estos eventos pueden afectar a elementos específicos dentro de un objeto, por ejemplo si quieremos modificar el tamaño de la fuente del título h2 de mi objeto producto al pasar el puntero sobre el tendríamos que realizar:

```
.productos h2 {
	font-size: 30px;
	font-weight: bold;
}

.productos li:hover h2{
	font-size: 33px;
}
```

nota como el evento hover es aplicado sobre el li y el elemento afectado es el h2 de ese li. Además por buena practica esto se  deja abajo de las propiedades estáticas del h2.