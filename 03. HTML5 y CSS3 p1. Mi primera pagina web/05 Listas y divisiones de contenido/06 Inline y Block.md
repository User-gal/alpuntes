
## Block

Elementos como las ul se componen por bloques, estos elementos ocupan el 100% del área en el que se encuentran, es por eso que si queremos ocupar la misma línea de un bloque para colocar más de un elemento debemos modificar la propiedad `display: inline-block;` esto permitirá que otros objetos se puedan colocar al lado.

```
ul{
	display: inline-block;
	vertical-align: top;
	width: 30%;
	margin-right: 15%;
}
```
La propiedad Inline-block permite que si el objeto no abarca el 100% del ancho de la página este pueda compartir el área que ocupa con otros.

El problema de esta propiedad es que si el objeto que se acomoda al lado, en este caso la imagen es mucho más alta que la lista, por default la alineación del texto quedará en el borde inferior, para corregir esto utilizamos `vertical-align: top;`  esta propiedad permite que la alineación de este objeto sea al borde superior.

Por último se crea un espaciado entre la imágen y la lisa con el `width:30%; margin-right: 15%;`
