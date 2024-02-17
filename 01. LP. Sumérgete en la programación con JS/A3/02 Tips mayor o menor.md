Podemos dar uso de operadores de comparación dentro del Java Script.

| No. | Operador | Nombre | Ejemplo | Resultado |
| ---- | ---- | ---- | ---- | ---- |
| 1 | > | mayor que | 5 > 6 | Falso |
| 2 | < | menor que | 5 < 6 | Verdadero |
| 3 | >= | mayor o igual | 5 >= 5 | Verdadero |
| 4 | <= | menor o igual | 5 <= 4 | Falso |
| 5 | != | Diferente | 5 != 6 | Verdadero |
| 6 | == | Igual | 5 == 6 | Falso |

Estos son muy útiles para poder comparaciones y bucles

```
if(numeroSecreto == numeroUsuario) {
	alert(`Acertaste el numero secreto es: ${numeroUsuario}`);
} else {
	if(numeroSecreto > numeroUsuario){
		alert(`El numero secreto es mayor`);
	} else {
		alert(`El numero secreto es menor`);
	}
}
```