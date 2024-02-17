Permiten modificar elemento específicos de nuestro HTML... en este caso letras

```
.titulo-principal{
	font-family: 'Roboto', sans-serif;
	font-size: 2em;
	margin: 0 0 1em;
	text-align: center;
	clear: left;
}

.titulo-principal:first-letter{
	font-weight: bold;
}

.titulo-principal::before{
	content: "[";
}

.titulo-principal::after{
	content: "]";
}

p:first-line{
	font-style: italic;
}
```
