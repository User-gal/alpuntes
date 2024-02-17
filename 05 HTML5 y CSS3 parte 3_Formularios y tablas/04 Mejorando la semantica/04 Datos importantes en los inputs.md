En formulários podemos asegurar que ciertos datos sean obligatorios, esto dependera del tipo de fomrulario que estemos desarrollando, es decir el diseñador del formulario determinará cuales datos marcar la obligatoriedad del mismo.

Esto se logra agregando el atributo `required` al input

además de esto, podemos agregar una sugerencia de dato para agregar...
Lo logramos con el atributo `placeholder="estilo a respetar">`

Por último para radio buttons y checklist podemos definir alguno de los elementos marcado por defecto con el atributo `checked`

```
<label for="telefono">Telefono</label>

<input type="tel" id="telefono" class="input-padron" required placeholder="(xxx) xxx xxxx">

<label for="radio-whatsapp" ><input type="radio" name="contacto" value="email" id="radio-whatsapp" checked>WhatsApp</label>
```
