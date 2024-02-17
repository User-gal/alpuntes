En un proyecto práctico dentro del curso "Iniciando con JavaScript", estás desarrollando un juego en el cual los usuarios tienen que adivinar el número secreto. Has escrito un código que muestra un mensaje de bienvenida a los jugadores, les pide que elijan un número entre 1 y 10 y les da una respuesta si aciertan, siguiendo la secuencia a continuación:

```csharp
javascript
alert('Bienvenidos al juego del número secreto');
let eleccion = prompt('Elige un número entre 1 y 10');

let numeroSecreto = 4;

if (eleccion == numeroSecreto) {
    alert('Adivinaste');
} 
```

¿Qué variable tendrías que cambiar para cambiar el número secreto en cada ronda del juego?

- Alternativa correta
    
    `if (elección == númeroSecreto) {`
    
- Alternativa correta
    
    `let numeroSecreto = 4`
    
    Esta es la variable que debes cambiar para cambiar el número secreto en cada ronda del juego. Al modificar el valor asignado a esta variable, estarás estableciendo un nuevo número secreto para el juego.
    
- Alternativa correta
    
    `let elección = prompt('Elige un número entre 1 y 10')`
    
- Alternativa correta
    
    `alert('Bienvenidos al juego del número secreto')`