Si realizaste el proyecto a medida que mirabas los videos del aula, ¡genial! Caso contrario no te preocupes. Es solo ejecutar los pasos listados a seguir.

En el archivo **index.html**, divide la página en bloques usando `<div>`, primero vamos a colocar todo el texto de la página en un bloque:

```xml
<div class="principal">
            <h1>Sobre la Barbería Alura</h1>
            <p>Ubicada en el corazón de la ciudad, la <strong>Barbería Alura</strong> trae para el mercado lo que hay de mejor para su cabello y barba. Fundada en 2020, la Barbería Alura ya es destaque en la ciudad y conquista nuevos clientes diariamente.</p>
            <p id="mision"><em>Nuestra misión es: <strong>"Proporcionar autoestima y calidad de vida a nuestros clientes"</strong>.</em></p>
            <p>Ofrecemos profesionales experimentados que están constantemente observando los cambios y movimiento en el mundo de la moda, para así ofrecer a nuestros clientes las últimas tendencias. El atendimiento posee un padrón de excelencia y agilidad, garantizando calidad y satisfacción de nuestros clientes.</p> 
</div>
```

Debajo del `div` principal, crea el `div` de los `diferenciales`, con la lista de beneficios y su imagen. Adiciona la imagen **diferenciales.jpg**, si todavía no bajaste la imagen puedes descargarla [aquí](https://github.com/alura-es-cursos/1742-HTML5-y-CSS3-parte1/raw/aula5/diferenciales.zip). Adiciona también un identificador de `class` para la etiqueta `img`:

```javascript
 <div class="diferenciales">
            <h2>Diferenciales</h2>
            <ul>
                <li class="items">Atención personalizada a los clientes</li>
                <li class="items">Espacio diferenciado</li>
                <li class="items">Localización</li>
                <li class="items">Profesionales calificados</li>
            </ul>
            <img src="diferenciales/diferenciales.jpg" class="imagenDiferenciales">
</div>
```

En el CSS **style.css**, remueve la estilización del color del fondo del `body` y colócala en el `div` principal. Y coloca un espaciamiento interno el mismo `div` principal

```css
body {

}

.principal{
    background: #CCCCCC;
    padding: 20px;
}
```

Altera la fuente de los ítems de la lista para `italic`, y estiliza el color del fondo del `div` de los `diferenciales`, alinea el texto del `h2` al centro.

```css
.diferenciales{
    background: #FFFFFF;
    padding: 30px;
}

h2{
    text-align: center;
}

.items{
    font-style: italic;
}
```

En la lista, modifica el `display` para `inline-block` y luego alinea la lista para arriba. Altera también su anchura para ocupar el 20% de la página y el margen externo a la derecha de la lista configúralo para ocupar el 15%:

```css
ul{
    display: inline-block;
    vertical-align: top;
    width: 20%;
    margin-right: 15%;
}
```

Para finalizar esta aula, configura el ancho de la imagen de los diferenciales:

```css
.imagenDiferenciales{
    width: 50%;
}
```