El `console.log` es una función muy importante en lenguajes de programación, especialmente cuando se trabaja con JavaScript. Su función principal es imprimir mensajes en la consola del entorno de desarrollo, lo que permite probar información relevante durante la ejecución de un programa.

> Ahora, incluya comandos console.log en diferentes partes del código para verificar el flujo del programa, los valores de las variables y otra información relevante durante la fase de desarrollo.


### Opinión del instructor

- [](https://app.aluracursos.com/suggestions/new/logica-programacion-sumergete-programacion-javascript/85994/opinion)

En el siguiente código, tenemos una sugerencia para agregar el comando `console.log` para verificar si los valores se están asignando correctamente a las variables y si las condiciones se están evaluando como se espera. Echa un vistazo:

```lua
alert('Bienvenido al juego del número secreto');

// Agrega un console.log para verificar el valor de "intento" después de la entrada del usuario
let intento = prompt('Elige un número entre 1 y 10');
console.log('Valor de intento:', intento);

let numeroSecreto = 4;

// Agrega un console.log para verificar la comparación entre "intento" y "numeroSecreto"
console.log('Resultado de la comparación:', intento == numeroSecreto);

if (intento == numeroSecreto) {
    alert('Adivinaste');
} else {
    // Agrega un console.log para verificar el valor de "numeroSecreto" cuando el jugador se equivoca
    console.log('Valor del número secreto:', numeroSecreto);
    alert('El número secreto era ' + numeroSecreto);
}
```

Es importante recordar que cuando el proyecto esté disponible para todas las personas, en lo que llamamos en el contexto del software "entorno de producción", los comandos `console.log` deben eliminarse o desactivarse, ya que pueden causar problemas de rendimiento y seguridad.