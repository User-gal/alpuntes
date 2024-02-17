Suponga que estás desarrollando una nueva función para Playcatch, el "Spotify" de Alura. Tu tarea es mostrar un texto especial en la pantalla principal del usuario siempre que agreguen una nueva canción a su lista de reproducción. Para hacerlo, necesitas cambiar el texto de un elemento HTML utilizando JavaScript.

¿Cómo puedes cambiar el texto del elemento h2 en tu página a "Has agregado una nueva canción!" usando los conceptos del curso "Lógica de programación: explore funciones y listas"?

- Alternativa correta
    
    ```javascript
    let h2 = document.getElementsByClassName('h2');
    h2.innerHTML = 'Has agregado una nueva canción!';
    ```
    
- Alternativa correta
    
    ```javascript
    let h2 = document.querySelector('h2');
    h2.innerHTML = 'Se ha añadido una nueva canción!';
    ```
    
- Alternativa correta
    
    ```javascript
    let h2 = document.querySelector('h2');
    h2.innerHTML = 'Has agregado una nueva canción!';
    ```
    
    Al seleccionar el elemento `h2` con el método `querySelector` y cambiar el texto con `innerHTML`, estás utilizando correctamente los conceptos enseñados en el curso.
    
- Alternativa correta
    
    ```javascript
    let h2 = document.querySelector('h1');
    h2.innerHTML = 'Has agregado una nueva canción!'
    ```