¿Cómo usar medidas proporcionales para dejar un elemento 100% de ancho con el equivalente a un tercio del elemento padre, menos 10px?

- Alternativa correta
    
    ```css
    width: calc( (100% / 3) - 10px )
    ```
    
    ¡Alternativa correcta! Es necesario calcular el un tercio del elemento, esa es una de las formas de hacer eso, luego le restamos los 10px.