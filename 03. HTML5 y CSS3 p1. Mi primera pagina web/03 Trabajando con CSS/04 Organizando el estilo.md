No es una buena practica utilizar la metodología inline, que es asignar el tag style a todos los elementos de un html.

## Método 2
Se recomienda definir un bloque específico de estilos, de la siguiente manera dentro del head.

```
<style>
	p{
		text-align: center;
	}
</style>
```


## Método 3
Sin embargo la metodologia más utilizada es crear un archivo de estilo aparte del html

por ejemplo 

style.css

y su contenido sería el de la etiqueta style

```
p{
	text-align: center;
}
```

sin embargo para que este funciones necesitas agregar al head del html

```
	<link rel="stylesheet" href="style.css">
```