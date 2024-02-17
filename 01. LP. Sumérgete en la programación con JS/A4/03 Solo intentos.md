Eres la persona encargada del sistema informático de Serenatto - Café & Bistró. La gerente desea mejorar el sistema de lotería del bistró implementando un juego en el cual los clientes adivinan un número secreto para ganar un descuento especial. Empleando tus conocimientos del curso "Lógica de programación: sumérgete en la programación con JavaScript", decides implementar esta funcionalidad utilizando la instrucción "break".

Pregunta: ¿Cómo implementarás un límite de 5 intentos para que los clientes adivinen el número secreto?

- Alternativa correta
    
    [ ] Utilizando un bucle while sin la instrucción `break`.
    
    ```javascript
    let numeroSecreto = Math.floor(Math.random() * 10);
    let intentos = 0;
    while (intentos < 5) {
      let intento = parseInt(prompt("Ingrese un número del 0 al 9:"));
      intentos++;
      if (intento == numeroSecreto) {
        alert(`¡Eso es! Descubriste el número secreto ${numeroSecreto}`);
      }
    }
    ```
    
- Alternativa correta
    
    [ ] Utilizando un bucle while con la instrucción break cuando el cliente adivine el número.
    
    ```javascript
    let numeroSecreto = Math.floor(Math.random() * 10);
    let intentos = 0;
    while (intentos < 5) {
      let intento = parseInt(prompt("Ingrese un número del 0 al 9:"));
      intentos++;
      if (intento == numeroSecreto) {
        alert(`¡Eso es! Descubriste el número secreto ${numeroSecreto}`);
        break;
      }
    }
    ```
    
    Este código implementa correctamente un límite de 5 intentos y también utiliza la instrucción break cuando se adivina el número secreto.
    
- Alternativa correta
    
    [ ] Utilizando un bucle for sin la instrucción `break`.
    
    ```javascript
    let numeroSecreto = Math.floor(Math.random() * 10);
    for (let intentos = 0; intentos < 5; intentos++) {
      let intento = parseInt(prompt("Ingrese un número del 0 al 9:"));
      if (intento == numeroSecreto) {
        alert(`¡Eso es! Descubriste el número secreto ${numeroSecreto}`);
      }
    }
    ```
    
- Alternativa correta
    
    [ ] Usando un bucle for junto con la instrucción break cuando el cliente adivine el número o cuando el número de intentos llegue a 5.
    
    ```javascript
    let numeroSecreto = Math.floor(Math.random() * 10);
    for (let intentos = 0; intentos < 5; intentos++) {
      let intento = parseInt(prompt("Ingrese un número del 0 al 9:"));
      if (intento == numeroSecreto) {
        alert(`¡Eso es! Descubriste el número secreto ${numeroSecreto}`);
        break;
      }
    }
    ```
    
    Este código implementa correctamente un límite de 5 intentos. Utiliza un bucle for y finaliza el bucle cuando se adivina el número secreto o cuando se alcanzan 5 intentos.