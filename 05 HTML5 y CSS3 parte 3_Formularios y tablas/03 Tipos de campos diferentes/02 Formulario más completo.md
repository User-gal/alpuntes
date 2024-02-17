existen inputs más complejos que nos permiten manipular mejor los elementos

textarea permite tener un área para ingresar texto más extenso y se puede manipular de manera dinámica el texto:
```
 <label for="mensaje" >Mensaje</label>
 <textarea cols="70" rows"10" id="mensaje"></textarea>
```

radio: Para tener una lista de selección radial
```
 <label for="radio-email" >Email</label>
 <input type="radio" name="contacto" value="email" id="radio-email"></input>
 <label for="radio-telefono" >Teléfono</label>
 <input type="radio" name="contacto" value="telefono" id="radio-telefono"></input>
 <label for="radio-whatsapp" >WhatsApp</label>
 <input type="radio" name="contacto" value="email" id="radio-whatsapp"></input>
 
```

el type define el tipo de entrada... selector radial
el name da un identificador que asocia todos los radios como para que solo se pueda marcar uno de los elementos
value es el calor que regresará el formulario una vez enviado
id es un identificador para el botón



Checkbox: Casilla de verificación

`<label><input type="submit"¿Le gustaría recibir promociones y novedades?></input></label>`
Nota que en este caso se coloco el input dentro del label
