Una forma de alinear un grupo de elementos o manipular sus propiedades de manera rápida es haciendo uso de las etiquetas div dentro del HTML. 

```
<div class="caja">
	<h1><img src="img/logo.png"></h1>
	<nav>
		<ul>
			<li><a href="index.html">Home</a></li>
			<li><a href="productos.html">Productos</a></li>
			<li><a href="contacto.html">Contacto</a></li>
		</ul>
	</nav>
</div>
```
Además es recomendable asignar una clase o Identificador, según sea tu conveniencia. Esto para poder aplicar estilos de manera más controlada.

Ahora con ayuda de CSS acomodaremos los elementos img y nav uno al lado del otro

```
.caja{
	margin: 0 auto;
	position: relative;
	width: 85%;
}

  

nav{
	position: absolute;
	top: 40%;
	right: 0px;
}
```

el margin de la clase caja da un margen superior e inferior igual a 0 y a la izquierda y derecha a colocar `auto` dejamos que el margen total se distribuya a ambos lados, es importante señalar que para que esto tenga efecto debemos darle al div un ancho `width` menor al 100% de la pantalla, es esta caso preferí usar porcentaje a pixeles... me queda pendiente utilizar un los em como unidad de medida.