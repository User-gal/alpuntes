Si realizaste el proyecto a medida que mirabas los videos del aula, ¡genial! Caso contrario no te preocupes. Es solo ejecutar los pasos listados a seguir.

Remueve todo el CSS inline de la página `index.html`.

Como primer item del `body`, adiciona la imagen **banner.jpg**, si todavía no bajaste la imagen descargarla [aquí](https://github.com/alura-es-cursos/1742-HTML5-y-CSS3-parte1/raw/aula4/banner.zip). Adiciona también un identificador para la etiqueta `img`:

```bash
<img id="banner" src="banner.jpg">
```

Adiciona un identificador para el segundo párrafo del texto:

```xml
<p id="mision"><em>Nuestra misión es: <strong>"Proporcionar autoestima y calidad de vida a nuestros clientes"</strong>.</em></p>
```

En el archivo **style.css**, adiciona el CSS que fue removido de la página **index.html**, o sea, alinea el `h1` y los párrafos en el centro de la página y aumenta la fuente del segundo párrafo (usa tu identificador para hacer la referencia):

```css
h1{
    text-align: center;
}

p{
    text-align: center;
}
#mision{
    font-size: 20px;
}
```

En el mismo archivo _style.css*_ altera el ancho de la imagen:

```css
#banner {
    width: 100%;
}
```

El CSS completo debe quedar así:

```css
body{
    background: #CCCCCC;
}

#banner{
    width:100%;
}

h1{
    text-align: center;
}

p{
    text-align: center;
}

em strong{
    color:red;
}

#mision{
    font-size: 20px;
}
```