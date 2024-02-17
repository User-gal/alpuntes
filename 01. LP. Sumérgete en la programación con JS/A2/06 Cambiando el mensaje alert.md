Eres un desarrollador de software en una clínica médica llamada Médica Voll. La empresa desea que crees un pequeño juego de adivinanzas para sus pacientes mientras esperan en la sala de espera. Entonces, decides crear un juego del número secreto utilizando JavaScript, como se muestra a continuación:

```csharp
javascript
alert('Bienvenido al juego del número secreto');
let intento = prompt('Elige un número entre 1 y 10');

let numeroSecreto = 4;

console.log(intento  == numeroSecreto);
if (intento  == numeroSecreto) {
    alert('Acertaste');
} else {
    alert('El número secreto era ' + numeroSecreto);
}
```

Dada esta estructura básica de código que creaste, ¿cómo modificarías el mensaje del alert para incluir el número que el paciente eligió en caso de no acertar el número secreto? Elige la opción correcta:

- Alternativa correta
    
    `alert('El número secreto era ' + numeroSecreto, ' y elegiste ' + intento)`
    
- Alternativa correta
    
    `alert('El número secreto era ' + numeroSecreto + intento)`
    
- Alternativa correta
    
    `alert('El número secreto era ' + numeroSecreto + ', pero elegiste ' + intento);`
    
    Este código concatena correctamente el número secreto y la elección del paciente en el mensaje de alerta.
    
- Alternativa correta
    
    `alert('El número secreto era numeroSecreto y elegiste intento');`