Usando esta estructura:

```css
<h2>
<section>
    <h2>
    <p>
    <p>
    <h2>
</section>
```

¿Cómo hacemos para seleccionar el último `<h2>` ?


- Alternativa correta
    
    ```css
    section > p + h2
    ```
    
    ¡Alternativa correcta! El último `h2` es hijo directo de la `section` y hermano del `p`.