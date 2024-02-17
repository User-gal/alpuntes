Hay un gran problema con los blucles, si no se cumple nunca con la condición de salida, por que no logramos llegar a ella, puede ser que forcemos la salida del mismo.

La sentencia 'break' nos permitirá salir de un blucle cuando lleguemos a ella.

```
if( intentos > 3){
	alert('Llegaste al numero máximo de intentos');
	break;
}
```
En el código se indica al programa que si el usuario tiene solo 3 intentos para averiguar el número secreto, si se pasa, entra a esta condición if, muestra el mensaje con el 'alert' y enseguida con uso del 'break' sale del bucle.

