Contexto: Imagina que eres una persona desarrolladora que trabaja para Buscante, una importante tienda en línea de libros. Tu jefe te ha pedido que crees una función para sortear libros a los clientes. El sorteo debe hacerse de manera que todos los libros tengan la oportunidad de ser sorteados al menos una vez, y después de eso, el sorteo debe comenzar de nuevo. Recordaste la lección sobre la adición de la variable "numeroLimite" en el curso "Lógica de programación: explore funções e listas". ¿Cómo implementarás el sorteo del libro teniendo en cuenta lo que se enseñó?

- Alternativa correta
    
    ```javascript
    function sortearLibro() {
        let libroElegido = Math.floor(Math.random() * listaDeLibros.length);
        return listaDeLibros[libroElegido];
    }
    ```
    
    En este código, aunque se elige un libro al azar, no se verifica si todos los libros ya han sido sorteados para reiniciar el proceso.
    
- Alternativa correta
    
    ```javascript
    function sortearLibro() {
        let libroElegido = parseInt(Math.random() * numeroLimite + 1);
        let cantidadDeLibrosSorteados = listaDeLibrosSorteados.length;
        if (cantidadDeLibrosSorteados == numeroLimite) {
            listaDeLibrosSorteados = [];
        }
        // Código omitido
    }
    ```
    
    Correcta! Esta respuesta es correcta porque sigue la lógica enseñada en el curso de programación. En este código, se genera un número aleatorio para elegir un libro y luego se verifica si se ha alcanzado el límite de libros sorteados. Si es así, la lista de libros sorteados se reinicia para comenzar de nuevo el sorteo.
    
- Alternativa correta
    
    ```javascript
    function sortearLibro() {
        let libroElegido = listaDeLibros[numeroLimite];
        return listaDeLibros[libroElegido];
    }
    ```
    
    En este código, el libro se elige en función del número límite, lo que no garantiza que todos los libros tengan la oportunidad de ser sorteados.