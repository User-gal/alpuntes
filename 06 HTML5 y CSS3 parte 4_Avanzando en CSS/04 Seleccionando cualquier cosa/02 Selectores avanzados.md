Nos permiten llegar a cualquier elemento de nuestro html

en el CSS

```
main p{
	background:red;
}
```
Esto daría un fondo rojo a todos los párrafos de nuestro html

entonces utilizaremos el operador > para seleccionar solo los  que sean hijos directos del main

```
main > p{
	background:red;
}
```

Si necesitamos aplicar esto a el p de nuestra primera sección..

```
img + p{
	background: yellow;
}
```

Al p despues de una imágen

```
img ~ img{
	background:green;
}
```

a todos los parrafos después de la imagen

```

.principal p:not(#mision){
	background:orange;
}
```

aplica a todos los parrafos menos al id misión