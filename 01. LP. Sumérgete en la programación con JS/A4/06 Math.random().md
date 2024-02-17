La función `Math.random()` genera un número pseudo aleatorio. El numero es un valor entre 0 y 1.

Entonces si quieres generar un número entre 1 y 10 tendrás que procesar el resultado mediante una formula.

```
let numeroSecreto = Math.random();
// esto nos generara un número decimal entre 0 y 1
// supongamos que es 0.88991234
// de ese número quiero obtener un número entre 0 y 10
let numeroSecreto2 = Math.random() * 10;
//Supongamos que es el mismo numero  0.88991234
//el resultado sería  8.8991234
//Ahora para quitar los decimales usamos el método floor
let numeroSecreto3 = Math.floor(Math.random * 10);
//Suponiendo que el numero sigue siendo  8.8991234
//floor solo se queda con el entero por lo tanto
//el resultado es 8

```

El problema de este código es que genera solo numero entre 0 y 9, por lo tanto si queremos que los límites sean entre 1 y 10, tenemos que sumarle 1 a el resultado:

```
let numeroSecreto3 = Math.floor(Math.random() * 10) + 1;
```
