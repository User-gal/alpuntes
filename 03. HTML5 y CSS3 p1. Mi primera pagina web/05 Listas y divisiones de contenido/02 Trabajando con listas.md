Crear listas en HTML

Las listas  dentro de html se pueden crear con ayuda de las etiquetas

```
<ul>
	<li>Elemento 1</li>
	<li>Elemento 2</li>
	...
	<li>Elemento n</li>
</ul>
```

ul(unordered list) nos crea listas no ordenadas, y cada elemento dentro de la lista debe ir entre las etiquetas li(list item)si nosotros deseamos crear una lista ordenada(Numerada) usamos ol(ordened list);

```
<ol>
	<li>Elemento 1</li>
	<li>Elemento 2</li>
	...
	<li>Elemento n</li>
</pl>
```

## Clases

Una forma de referenciar elementos desde nuestro css, como una buena practica es asignarle a los elemento una classe, para esto dentro del tag del elemento agregamos la prodiedad class.

```
<ul>
	<li class="item">Elemento 1</li>
	<li class="item">Elemento 2</li>
	...
	<li class="item">Elemento n</li>
</ul>
```
desde nuestro style.css lo personalizaríamos con:

```
.item{
	font-color: blue;
	font-size: 15px;
	font-style: Italic;
}
```

