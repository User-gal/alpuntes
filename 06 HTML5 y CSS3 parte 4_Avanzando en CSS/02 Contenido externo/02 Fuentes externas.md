Puedes utilizar familias de fuentes distintas  las predeterminadas, para esto necesitas incrustar el código de la fuente, tanto en el HTML como en el CSS.

Un gran repositorio de fuentes es https://fonts.google.com/

desde ahí seleccionamos la fuente a utilizar
y en el head de nuestro HTML introducimos el código que nos proporciona google fonts

```
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Protest+Riot&display=swap" rel="stylesheet">
```

y en el CSS, en el bloque, id, clase o etiqueta en la cual necesites utilizar esta fuente

```
font-family: 'Protest Riot', sans-serif;
```
