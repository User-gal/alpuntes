Si realizaste el proyecto a medida que mirabas los videos del aula, ¡genial! Caso contrario no te preocupes. Es solo ejecutar los pasos listados a seguir.

Define la estructura básica del HTML **index.html**, sin olvidar definir el lenguaje de la página.

```xml
<!DOCTYPE html>
<html lang="es">
        <h1>Sobre la Barbería Alura</h1>
        <p>Ubicada en el corazón de la ciudad, la <strong>Barbería Alura</strong> trae para el mercado lo que hay de mejor para su cabello y barba. Fundada en 2020, la Barbería Alura ya es destaque en la ciudad y conquista nuevos clientes diariamente.</p>
        <p><em>Nuestra misión es: <strong>"Proporcionar autoestima y calidad de vida a nuestros clientes"</strong>.</em></p>
        <p>Ofrecemos profesionales experimentados que están constantemente observando los cambios y movimiento en el mundo de la moda, para así ofrecer a nuestros clientes las últimas tendencias. El atendimiento posee un padrón de excelencia y agilidad, garantizando calidad y satisfacción de nuestros clientes.</p> 
</html>
```

Pasa las informaciones del _encoding_ (diccionario) para la renderización correcta de la página en cualquier navegador, y define el título también:

```xml
<!DOCTYPE html>
<html lang="es">
        <meta charset="UTF-8"> 
        <title>Barbería Alura</title>
        <h1>Sobre la Barbería Alura</h1>
        <p>Ubicada en el corazón de la ciudad, la <strong>Barbería Alura</strong> trae para el mercado lo que hay de mejor para su cabello y barba. Fundada en 2020, la Barbería Alura ya es destaque en la ciudad y conquista nuevos clientes diariamente.</p>
        <p><em>Nuestra misión es: <strong>"Proporcionar autoestima y calidad de vida a nuestros clientes"</strong>.</em></p>
        <p>Ofrecemos profesionales experimentados que están constantemente observando los cambios y movimiento en el mundo de la moda, para así ofrecer a nuestros clientes las últimas tendencias. El atendimiento posee un padrón de excelencia y agilidad, garantizando calidad y satisfacción de nuestros clientes.</p> 
</html>
```

Finalmente, separa las etiquetas de informaciones de las de contenido en la página:

```xml
<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="UTF-8"> 
        <title>Barbería Alura</title>
    </head>

    <body>
        <h1>Sobre la Barbería Alura</h1>
        <p>Ubicada en el corazón de la ciudad, la <strong>Barbería Alura</strong> trae para el mercado lo que hay de mejor para su cabello y barba. Fundada en 2020, la Barbería Alura ya es destaque en la ciudad y conquista nuevos clientes diariamente.</p>
        <p><em>Nuestra misión es: <strong>"Proporcionar autoestima y calidad de vida a nuestros clientes"</strong>.</em></p>
        <p>Ofrecemos profesionales experimentados que están constantemente observando los cambios y movimiento en el mundo de la moda, para así ofrecer a nuestros clientes las últimas tendencias. El atendimiento posee un padrón de excelencia y agilidad, garantizando calidad y satisfacción de nuestros clientes.</p> 
    </body>
</html>
```