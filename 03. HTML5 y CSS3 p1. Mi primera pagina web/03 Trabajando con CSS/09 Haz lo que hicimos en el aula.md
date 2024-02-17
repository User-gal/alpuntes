Si realizaste el proyecto a medida que mirabas los videos del aula, ¡genial! Caso contrario no te preocupes. Es solo ejecutar los pasos listados a seguir.

En la misma carpeta de nuestro archivo **index.html**. crea un archivo CSS **style.css**. En este archivo, modifica el color del fondo el `body`, centra los párrafos y altera el color de las etiquetas `strong` que están dentro de las etiquetas `em`

```css
body{
    background: #CCCCCC;
}

p{
    text-align: center;
}

em strong{
    color:red;
}
```

En la página **index.html**, importa el archivo CSS **style.css**, ubícalo en la última posición del `head`:

```bash
<link rel="stylesheet" href="style.css">
```

Centra el del `h1`:

```xml
<h1 style="text-align: center;">Sobre la Barbería Alura</h1>
```

Altera el tamaño de la fuente del segundo párrafo:

```xml
<p style="font-size: 20px"><em>Nuestra misión es: <strong>"Proporcionar autoestima y calidad de vida a nuestros clientes"</strong>.</em></p>
```

Hasta aquí, la página completa debe quedar de la siguiente forma:

```xml
<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="UTF-8"> 
        <title>Barbería Alura</title>
        <link rel="stylesheet" href="style.css">
    </head>

    <body>
        <h1 style="text-align: center;">Sobre la Barbería Alura</h1>
        <p>Ubicada en el corazón de la ciudad, la <strong>Barbería Alura</strong> trae para el mercado lo que hay de mejor para su cabello y barba. Fundada en 2020, la Barbería Alura ya es destaque en la ciudad y conquista nuevos clientes diariamente.</p>
        <p style="font-size: 20px"><em>Nuestra misión es: <strong>"Proporcionar autoestima y calidad de vida a nuestros clientes"</strong>.</em></p>
        <p>Ofrecemos profesionales experimentados que están constantemente observando los cambios y movimiento en el mundo de la moda, para así ofrecer a nuestros clientes las últimas tendencias. El atendimiento posee un padrón de excelencia y agilidad, garantizando calidad y satisfacción de nuestros clientes.</p> 
    </body>
</html>
```
