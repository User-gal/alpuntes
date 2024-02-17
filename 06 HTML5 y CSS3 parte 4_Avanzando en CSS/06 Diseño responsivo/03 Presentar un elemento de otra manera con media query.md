¿Cómo marcar un elemento para que se presente de otra manera a través de una condición, en una pantalla de hasta 480px?

- 
    
    ```python
    @media (min-width: 480px) {}
    ```
    
- 
    
    ```scss
    @media (width=device-width) {}
    ```
    
- Alternativa correta
    
    ```python
    @media (max-width: 480px) {}
    ```
    
    ¡Alternativa correcta! Dentro de esta _media query_ podemos crear un estilo visual que incluye pantallas de hasta 480px.