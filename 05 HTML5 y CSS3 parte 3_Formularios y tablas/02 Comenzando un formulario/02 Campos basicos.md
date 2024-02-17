en HTML existe una etiqueta específica para crear formularios
```
<form>
	<label> Nombre completo>
	<input type="text">
</form>
```

la etiqueta `<label>` es el título del campo 
la etiqueta `<input>` es para entradas de texto

Una fomra de vincular una con esta es aplicar un id para relacionarlas

```
<form>
	<label for="nombre"> Nombre completo</label>
	<input type="text" id=""nombre>
</form>