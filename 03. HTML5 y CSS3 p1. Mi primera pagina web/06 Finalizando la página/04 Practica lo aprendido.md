Si realizaste el proyecto a medida que mirabas los videos del aula, ¡genial! Caso contrario no te preocupes. Es solo ejecutar los pasos listados a seguir.

Crea el encabezado de la página **index.html**:

```xml
<header>
     <h1 class="titulo-principal">Barbería Alura</h1>
</header>
```

Altera la etiqueta del título **Sobre la Barbería Alura** para `<h2>` y la etiqueta del título **Diferenciales** para `<h3>`. Y define una clase que aplique para las dos etiquetas.

```xml
<h2 class="titulo-centralizado">Sobre la Barbería Alura</h2>
```

Y

```xml
<h3 class="titulo-centralizado">Diferenciales</h3>
```

En el archivo **style.css**, coloca un espaciamiento interno hacia la izquierda de 20px en el selector de clase del encabezado:

```css
.titulo-principal {
    padding-left: 30px;
}
```

Para finalizar, remueve los estilos de las etiquetas `h1` y `h2` y los colocas en un único lugar, a través de la clase `titulo-centralizado`:

```css
.titulo-centralizado{
    text-align: center;
}
```