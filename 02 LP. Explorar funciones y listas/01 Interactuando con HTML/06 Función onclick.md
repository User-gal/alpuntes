Después de completar el curso "Lógica de programación: explore funciones y listas" en Alura, fuiste invitado a participar en un proyecto desafiante para crear un nuevo producto llamado "Screen Match", que pretende ser una especie de "YouTube" de Alura. Tu papel es crear una función que active una alerta cuando una persona hace clic en un botón específico.

Teniendo en cuenta lo que se enseñó sobre la función `onclick`, ¿cuál es la forma correcta de crear esta funcionalidad, utilizándose de las buenas prácticas de escritura de las funciones?

- Alternativa correta
    
    ```bash
    <button>Haz clic aquí</button>
    
    function alertFunction() {
      alert("¡Hola, has hecho clic en el botón!");
    }
    ```
    
- Alternativa correta
    
    ```bash
    <button onclick="alertFunction()">Haz clic aquí</button>
    
    function alertFunction() {
      alert("¡Hola, has hecho clic en el botón!");
    }
    ```
    
    Este es el uso correcto de la función `onclick` en un botón. La función `alertFunction()` se llamará cuando el usuario haga clic en el botón, mostrando la alerta.
    
- Alternativa correta
    
    ```xml
    <button onclick="alertFunction()">Haz clic aquí</button>
    ```
    
- Alternativa correta
    
    ```xml
    <button onclick="alert('¡Hola, has hecho clic en el botón!')">Haz clic aquí</button>
    ```
    

¡Enhorabuena, has acertado!

 [DISCUTIR EN EL FORO](https://app.aluracursos.com/forum/curso-logica-programacion-explorar-funciones-listas/exercicio-funcion-onclick/86093/novo)