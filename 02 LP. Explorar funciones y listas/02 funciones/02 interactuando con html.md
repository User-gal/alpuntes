Si existen tareas repetitivas, podemos crear una funcion que realize ese proceso en una sola ocasión.

si estas en JS para llamar una function solo escribes el nombre de la función  y debe de encontrarse abajo de la declaración... ya que JS es un lenguaje que se ejecuta de manera secuencial.

Hoisnting..
Si tu colocas el llamado antes de la declaración JS antes de ejecutar coloca todas las funciones arriba del código


En JS  las funciones pueden recibir  parametros, los cuales nos permitirán hacer de nuestro códigoreutilizable, estos parámetros van dentro de los parentesis de nuestra función.

Evidentemente cuando ejecutes la función tendrás que enviar los parametros a reemplazar.

Tomando el ejemplo anterior tendriamos

```
let titulo = document.querySelector('h1');
titulo.innerHTML = 'Juego del numero secreto'

let parrafo = document.querySelector('p');
parrafo.innerHTML = 'Indica un número del 1 al 10'
```

La forma más simplificada sería

```
function asignarTextoElemento(elemento, texto){
	let elementoHTML = document.querySelector(elemento);
	elementoHTML.innerHTML = texto;
}

asignarTextoElemento('h1','Jugandose la vida');
asignarTextoElemento('p','Ingresa un numero del 1 al 10');
```

Que más adelante podremos reutilizar esa funcion con elementos distintos al 'h1' y 'p'