En nuestra clase anterior, exploramos la función 'reiniciarJuego' y aprendimos a organizar nuestro código utilizando comentarios para guiar nuestras acciones paso a paso. Ahora, te presentamos un desafío práctico para poner en práctica tus conocimientos sobre el uso de funciones y buenas prácticas de programación.

El siguiente código en JavaScript calcula el doble y el triple de un número proporcionado. Tu tarea consiste en seleccionar las opciones que sigan las mejores prácticas de programación y ayuden a mejorar la legibilidad y mantenibilidad del código.

```javascript
function calcularDobleTriple(numero) {
  const doble = numero * 2;
  const triple = numero * 3;

  return `El doble de ${numero} es ${doble} y el triple es ${triple}.`;
}

const numero = 5;
const resultado = calcularDobleTriple(numero);
console.log(resultado);
```

- Alternativa correta
    
    ```javascript
    function calcularDobleTriple(numero) {
      return numero * 2 + " es el doble y " + numero * 3 + " es el triple.";
    }
    
    const numero = 5;
    const resultado = calcularDobleTriple(numero);
    console.log(resultado);
    ```
    
    Esta opción es incorrecta porque devuelve una cadena de texto que incluye resultados y descripciones en la misma cadena. Esto puede dificultar la reutilización de los valores numéricos en otros cálculos y afecta la legibilidad del código.
    
- Alternativa correta
    
    ```javascript
    function calcularDoble(numero) {
      return numero * 2;
    }
    
    function calcularTriple(numero) {
      return numero * 3;
    }
    
    const numero = 5;
    const doble = calcularDoble(numero);
    const triple = calcularTriple(numero);
    
    console.log(`El doble de ${numero} es ${doble} y el triple es ${triple}.`);
    ```
    
    Esta opción es correcta porque divide la funcionalidad en dos funciones separadas, calcularDoble y calcularTriple, lo que mejora la modularidad y facilita la comprensión del código. Además, utiliza variables explícitas (doble y triple) para almacenar los resultados, lo que hace que el código sea más legible.
    
- Alternativa correta
    
    ```javascript
    function calcularDobleTriple(numero) {
      const resultado = {};
      resultado.doble = numero * 2;
      resultado.triple = numero * 3;
      return resultado;
    }
    
    const numero = 5;
    const resultado = calcularDobleTriple(numero);
    
    console.log(`El doble de ${numero} es ${resultado.doble} y el triple es ${resultado.triple}.`);
    
    ```
    
    Esta opción es incorrecta porque utiliza un objeto para almacenar los resultados, lo que es innecesario para este cálculo simple. Esto agrega complejidad al código sin ningún beneficio claro en términos de legibilidad o mantenibilidad.