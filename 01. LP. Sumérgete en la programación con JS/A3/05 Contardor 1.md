SSaber cómo trabajar con bucles de repetición, como el 'while', es esencial en la programación. Los bucles permiten automatizar tareas repetitivas y manejar grandes cantidades de datos de manera eficiente.

Sin embargo, es importante utilizarlos con precaución para evitar bucles infinitos (cuando la condición nunca se vuelve falsa, lo que puede bloquear el programa).

Siempre se recomienda tener una lógica que eventualmente haga que la condición se vuelva falsa para que el bucle termine correctamente.

A continuación, tenemos un ejemplo de código:

```javascript
let contador = 1;

while (contador < 4) {
  console.log('Ejecutando la iteración ' + contador);
  contador = contador + 1;
}
```

Al ejecutar código, podemos afirmar que:

- Alternativa correta
    
    [ ] 
    
    La instrucción 'while (contador < 4){ }' inicia el bucle 'while'. Este continuará repitiendo el bloque de código dentro de las llaves { } mientras la condición 'contador < 4' sea verdadera.
    
    ¡Exactamente! Esa condición significa que el bucle continuará mientras el valor de la variable 'contador' sea menor que 4.
    
- Alternativa correta
    
    [ ] 
    
    El resultado final será la impresión de los mensajes "Ejecutando la iteración 1", "Ejecutando la iteración 2" y "Ejecutando la iteración 3" en la consola.
    
    ¡Exacto! El bucle se ejecutó tres veces, y el valor final de la variable 'contador' es 4. En la cuarta iteración, el valor de 'contador' es 4. En ese momento, la condición 'contador < 4' se vuelve falsa, ya que 4 no es menor que 4. El bucle deja de ejecutar el código dentro de las llaves y termina.
    
- Alternativa correta
    
    [ ] 
    
    El resultado final será la impresión de los mensajes "Ejecutando la iteración 1", "Ejecutando la iteración 2", "Ejecutando la iteración 3" y "Ejecutando la iteración 4" en la consola.
    
- Alternativa correta
    
    [ ] 
    
    Se mostrará un error en la consola indicando que el contador no está definido.