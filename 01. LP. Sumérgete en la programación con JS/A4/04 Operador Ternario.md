Dentro de JS se pueden utilizar diferentes formas de incrementar. La forma común es:
```
intentos = intentos + 1;
```

Sin embargo este mismo proceso lo podemos realizar de la siguiente manera:

```
intentos += 1;
```

Este método es una herencia de lenguajes como C++. Una tercera opción que es incluso más utilizada por los programadores es la siguiente:

```
intentos++;
```

Una de las bondades de usar String Template en JS es la posibilidad de agregar código en las sentencias `${  }` , esto es gracias al operador ternario, la estructura es:

```
	${Condición ? Valor si es verdadero : Valor si es falso}
```

Lo primero que se realiza es comprobar la condición, esta arrojará los valores booleanos `True`  o  `False. 
Si el resultado es Verdadero,  entonces ejecutar el código que se encuentra entre el '?' y los ':'. 
Si el resultado es falso entonces ejecuta el código después de los ':'

Ejemplo:

```
${Intento == 1 ? 'vez' : 'veces'}
```
