Llegó la hora de poner en práctica lo que fue visto en el aula. Para esto, ejecute los siguientes pasos:

1) En el archivo **style.css**, cuando el mouse pase sobre la imagen de los diferenciales, déjalo un poco opaco. Agrega una transición a esto y también un sombreado en la imagen:

```css
.imagen-diferenciales{
    width: 60%;
    transition: 400ms;
    box-shadow: 10px 10px 30px 15px #000000;
}

.imagen-diferenciales:hover{
    opacity: 0.3;
}
```