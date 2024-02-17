Llegó la hora de poner en práctica lo que fue visto en el aula. Para esto, ejecute los siguientes pasos:

1) En la página **index.html**, dentro del `head` , agrega la _etiqueta_ `meta` `viewport` , justo debajo de la _etiqueta_ `meta` `charset`:

```xml
<meta name="viewport" content="width=device-width">
```

2) Cambia el tamaño del video, para que ya no sea fijo, sino que ocupe todo el ancho de la pantalla, con `width="100%"`:

```xml
<iframe width="100%" height="315" src="https://www.youtube.com/embed/wcVVXUV0YUY" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```

3) En el archivo **style.css**, agrega un estilo diferente para dispositivos de hasta **480 píxeles** de ancho usando _media query_:

```css
@media screen and (max-width:480px){
    h1{
        text-align: center;
    }
    nav{
        position: static;
    }
    .caja, .principal, .mapa-contenido, .contenido-diferenciales, .video {
        width: auto;
    }
    .lista-diferenciales, .imagen-diferenciales{
        width: 100%;
    }
}
```