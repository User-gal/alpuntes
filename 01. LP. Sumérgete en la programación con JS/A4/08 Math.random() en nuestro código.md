Para variar el numero secreto en nuestro código de JS, necesitamos modificar la definición de la variable de la siguiente manera.

```
let numeroSecreto = Math.floor(Math.random() * 10) + 1;
```
Ahora, el método prompt nos permite capturar un valor desde el usuario, el problema de este método es que el valor capturado es del tipo string, esto lo podemos averiguar con el método `typeof()`
```
typeof(variable);
```

| valor | tipo |
| ---- | ---- |
| 540 | int |
| 540.345 | float |
| '540' | string |
| True | boolean |
Para convertir el valor capturado desde el teclado usamos el método `ParseInt(variable)`

```
let numeroUsuario = parseInt(prompt("Ingresa un número"));
console.log(typeof(numeroUsuario))
```
