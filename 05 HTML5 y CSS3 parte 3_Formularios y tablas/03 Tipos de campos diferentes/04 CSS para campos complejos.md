En el CSS si queremos agregar a más de un elemento el mismo estilo agregamos los selectores separados con comas(,)

```
form input,text{
	display: block;
	margin: 0 0 20px;
	padding: 10px 25px;
	width: 50%;
}
```

Para que aparezca el label en línea con el input colocamos el input dentro del label

```
<div>
	<p>¿Cómo le gustaría que lo contactemos?</p>
	<label for="radio-email" ><input type="radio" name="contacto" value="email" id="radio-email">Email</label>
	
	  <label for="radio-telefono"><input type="radio" name="contacto" value="telefono" id="radio-telefono">Teléfono</label>
	
	  <label for="radio-whatsapp" ><input type="radio" name="contacto" value="email" id="radio-whatsapp">WhatsApp</label>
</div>

<label class="checkbox"><input type="checkbox">¿Le gustaría recibir promociones y noticias de la Barbería?</label>
```
