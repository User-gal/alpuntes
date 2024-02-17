Llegó la hora de poner en práctica lo que fue visto en el aula. Para esto, ejecute los siguientes pasos:

1) En la página **index.html**, coloca la lista de los diferenciales dentro de una `div` , agrega una clase a `ul` y agrega 2 nuevos diferenciales en la lista. Además, coloca la imagen de diferenciales en la misma línea que el cierre de la `ul` (clase `</ul>`) y cambie su clase a `imagen-diferenciales`:

```javascript
<div class="contenido-diferenciales">
    <ul class="lista-diferenciales">
        <li class="items">Atención personalizada a los clientes</li>
        <li class="items">Espacio diferenciado</li>
        <li class="items">Localización</li>
        <li class="items">Profesionales calificados</li>
        <li class="items">Puntualidad</li>
        <li class="items">Limpieza</li>
    </ul><img src="diferenciales/diferenciales.jpg" class="imagen-diferenciales">
</div>
```

2) Coloca también el mapa dentro de una `div`:

```xml
<div class="mapa-contenido">
    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d34784.869470159!2d-46.65499870427411!3d-23.593248407555798!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94ce5a2b2ed7f3a1%3A0xab35da2f5ca62674!2sCaelum%20-%20Education%20and%20Innovation!5e0!3m2!1ses-419!2sbr!4v1602972945026!5m2!1ses-419!2sbr" width="100%" height="300" frameborder="0" style="border:0;" allowfullscreen="" aria-hidden="false" tabindex="0"></iframe>
</div>
```

3) En el **style.css**, elimina los estilos de `main`:

```css
main {
}
```

4) Además de eso, agrega los estilos de los diferenciales:

```css
.diferenciales {
    padding: 3em 0;
    background: #888888;
}

.contenido-diferenciales {
    width: 640px;
    margin: 0 auto;
}

.lista-diferenciales {
    width: 40%;
    display: inline-block;
    vertical-align: top;
}

.items {
    line-height: 1.5;
}

.items:first-child {
    font-weight: bold;
}

.imagen-diferenciales {
    width: 60%;
}
```

5) Estilice la `div` del mapa y la `section` `principal`:

```css
.mapa-contenido {
    width: 940px;
    margin: 0 auto;
}

.principal {
    padding: 3em 0;
    background: #FEFEFE;
    width: 940px;
    margin: 0 auto;
}
```

6) Agrega un `background` al `mapa`:

```css
.mapa {
    padding: 3em 0;
    background: linear-gradient(#FEFEFE, #888888);
}
```

7) Finalmente, agrega una estrella antes de todos los ítems de la lista de diferenciales:

```css
.items:before{
    content:"★"
}
```