Eres un desarrollador de software que trabaja con JavaScript y necesitas crear una función que verifique si un número es positivo, negativo o cero. Tu tarea es implementar una función que reciba como parámetro un número entero y muestre un mensaje en la consola según las siguientes reglas:

- Si el número es mayor que cero, el mensaje debe ser: "El número es positivo."
- Si el número es menor que cero, el mensaje debe ser: "El número es negativo."
- Si el número es igual a cero, el mensaje debe ser: "El número es cero."

Puedes utilizar la estructura de control if-else para verificar las condiciones y mostrar el mensaje correspondiente en la consola.

Analiza las siguientes alternativas y marca aquella que contiene el código que cumple con todas las reglas mencionadas anteriormente:

- Alternativa correta
    
    ```javascript
    function verificarNumero(numero) {
      if (numero > 0) {
        console.log("El número es positivo.");
      } else if (numero < 0) {
        console.log("El número es negativo.");
      } else {
        console.log("El número es zero.");
      }
    }
    ```
    
    En este código, utilizamos la estructura de control if-else para verificar las tres posibilidades: si el número es mayor que cero, si es menor que cero o si es igual a cero. Dependiendo de la condición, la función imprime el mensaje correspondiente en la consola."
    
- Alternativa correta
    
    ```javascript
    function verificarNumero(numero) {
      if (numero < 0) {
        console.log("El número es positivo.");
      } else if (numero > 0) {
        console.log("El número es negativo.");
      } else {
        console.log("El número es zero.");
      }
    }
    ```
    
- Alternativa correta
    
     ```cpp
     if (numero > 0) {
        console.log("El número es positivo.");
      } else if (numero < 0) {
        console.log("El número es negativo.");
      } else {
        console.log("El número es zero.");
      }
    ```
    
- Alternativa correta
    
     ```javascript
     function verificarNumero(numero) {
      if (numero > 0) {
        console.log("El número es positivo.");
      } else {
        console.log("El número es zero.");
      }
    }
    ```
    