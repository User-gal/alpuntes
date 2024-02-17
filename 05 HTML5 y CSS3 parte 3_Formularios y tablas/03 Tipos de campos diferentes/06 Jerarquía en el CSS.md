CSS en base a los selectores que usamos, se comporta de maneras distinta.

Los selectores que se utilizan son 
- Etiquetas
- Clases
- Identificadores

si tenemos el siguiente CSS
```
p{
	color: red;
}

form p{
	color: blue;
}
```
El color que prevalecerá es el azul, y no por encontrarse después del rojo, sino por la manera de aplicar
CSS trata de sumar los pesos relativos de los selectores para saber cual es el que prevalecera

![[Pasted image 20240202000632.png]]

Sin embargo si hacemos configuraciones de estilo en el HTML... estas serán las que prevalecerán.
![[Pasted image 20240202000815.png]]
