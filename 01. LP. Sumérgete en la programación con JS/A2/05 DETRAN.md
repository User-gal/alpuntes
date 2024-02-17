Eres una persona desarrolladora de software que crea aplicaciones para el Detran, que es la entidad encargada de la supervisión y regulación del tráfico, la habilitación de conductores, y el registro y licenciamiento de vehículos en Brasil.

La edad mínima para conducir en Brasil es de 18 años. Con esto en mente, tu equipo ha creado el siguiente programa:

```javascript
let edad = prompt("Ingrese su edad:");

if (edad >= 18) {
  console.log("Eres mayor de edad.");
} else {
  console.log("Eres menor de edad.");
}
```

Con esta base, analice las afirmaciones a continuación y marque solo las verdaderas.

- [x] Si la edad es mayor que 18, el mensaje que se mostrará en la consola será: "Eres menor de edad".
    
- [x] Si la edad es menor que 18, el mensaje que se mostrará en la consola será: "Eres menor de edad".
    
    Si la edad ingresada es menor que 18, la condición en el if será falsa (edad >= 18 es falso), y el flujo de ejecución pasará al bloque del else, mostrando el mensaje "Eres menor de edad"
- [x] Si la edad es igual a 18, el mensaje que se mostrará en la consola será: "Eres mayor de edad".
    
    Si la edad ingresada es igual a 18, la condición en el if será verdadera (edad >= 18 es verdadero), y se mostrará el mensaje "Eres mayor de edad", ya que el operador `>=` incluye el valor 18. Se ignorará el bloque de código dentro del else.
    
- [x] Si la edad es igual a 18, el mensaje que se mostrará en la consola será: "Eres menor de edad".