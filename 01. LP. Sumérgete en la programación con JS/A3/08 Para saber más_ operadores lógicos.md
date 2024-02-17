Cuando escribimos programas en JavaScript, a menudo nos encontramos con la necesidad de tomar decisiones basadas en condiciones. Es aquí donde los operadores lógicos entran en escena y nos ayudan a crear una lógica sólida y eficaz.

A continuación, vamos a explorar los operadores lógicos de una manera simple y fácil de entender. Tendremos ejemplos claros para ilustrar su funcionamiento.

**AND (&&)**

El operador AND, representado por el símbolo "&&", se utiliza para combinar dos condiciones y evaluar si ambas son verdaderas. Si ambas condiciones son verdaderas, el resultado será... verdadero. De lo contrario, lógicamente será falso. Por ejemplo:

```javascript
let idad = 25;
let tieneLicencia = true;

// si la edad es mayor de 18 y tiene una licencia...
if (idad > 18 && tieneLicencia) {
  console.log("Puede conducir!");
} else {
  console.log("No puede conducir!");
}
```

**OR( | | )**

El operador OR, representado por los símbolos "||", se utiliza para verificar si al menos una de las condiciones es verdadera. Si una de las condiciones es verdadera, el resultado será verdadero. Si ambas son falsas, el resultado será falso. Aquí tienes un ejemplo: let tieneManzana = false; let tieneBanana = true;

```cpp
// si tiene manzana o tiene banama…
if (tieneManzana|| tieneBanana) {
  console.log("Tienes frutas!");
} else {
  console.log("No tienes frutas.");
}
```

**Otros tipos de operadores lógicos**

|Operador|Nombre|Ejemplo|Resultado|
|---|---|---|---|
|==|Igual|A == B|Verdadero si A es igual a B|
|!=|Diferente|A != B|Verdadero si A no es igual a B|
|<|Menor que|A < B|Verdadero si A es menor que B|
|>|Mayor que|A > B|Verdadero si A es mayor que B|
|<=|Menor o igual|A <= B|Verdadero si A es menor o igual a B|
|>=|Mayor o igual|A >= B|Verdadero si A es mayor o igual a B|

**Operadores Lógicos**

|Operador|Nombre|Ejemplo|Resultado|
|---|---|---|---|
|&&|Y / AND|(A > B) && (B == C)|Verdadero si A es mayor que B y B es igual a C|
|\||O / OR|(A > B) \| (B == C)|Verdadero si A es mayor que B o B es igual a C|
|!|NEGACIÓN|!(A == B)|Verdadero si A NO es igual a B|

¿Te gustó este conocimiento y quieres más? Rafa Ballerini tiene un artículo increíble hablando sobre ‘Cómo usar operadores de comparación en Javascript’ que vale la pena leer