Modificamos el CSS con  un media query, reseteando los anchos fijos

```
@media screen and (max-width:480px) {

	.caja,.principal,.mapa-ubicacion,.contenido-diferenciales,.video{
		width: auto;
	}
	
	h1{
		text-align: center;
	}
	
	nav{
	position: static;
	}
	
	.contenido-principal{
		background-image: linear-gradient(rgba(255, 255, 255, 0.6), rgba(255, 255, 255, 0.5)), url(img/utensilios.jpg);
		padding: 20px 10px;
	}
	
	.utensilios{
		width: 0%;
		visibility: hidden;
	}
	
	  
	
	.lista-diferenciales,.imagenDiferenciales{
		width: 100%;
	}
}
```
