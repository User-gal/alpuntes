El último elemento general de una página web es el pié de página. HTML tienen un tag reservado para esta área, el cual es `footer` 

```
<footer>
	<img src="img/logo-blanco.png">
	<p>Copyright Barbería Alura - 2024</p>
</footer>
```

además de esto podemos asignarle propiedades de estilo desde css.

En este caso se hace uso de una imágen como fondo del footer, para lograr esto se asigna una url apuntando a la imagen a la propiedad `background: url(img/bg.jpg)`

```
footer{
	background: url(img/bg.jpg);
	padding: 45px;
	text-align: center;
}
```
