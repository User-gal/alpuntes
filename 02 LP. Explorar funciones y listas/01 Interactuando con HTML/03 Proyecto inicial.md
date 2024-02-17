Continuar con el juego interactuando con el html

Cuando HTML trabaja con un js

Document Object Model
-Nos permite interactuar entre el HTML y el Java Script

Una web esta formada por 

CSS - 
HTML
JavaScript

Para interactuar con el DOM debemos conocer las etiquetas que tenemos

-Selectores: La forma en que seleccionamos los elementos
Usamos el método (querySelector) para poder interactuar con HTML desdeJS

```
// Este método(querySelector) permite traer un elemento del html
// este tiene una estructura más compleja que una variable

let titulo = document.querySelector('h1');

// El innerHTML nos permite colocar un valor en el Objeto
titulo.innerHTML = 'Juego del número secreto'
```

esto colocaría en la etiqueta h1 del HTML el texto 'Juego del número secreto'
