Para dar sombra a un elemento en CSS usamos `box-shadow`

```
box-shadow: 10px 10px #dedede;
```
el primer parametro es sombra vertical, si es positivo sería hacia abajo, si es negativo hacia arriba
el segundo es en horizantal, el cual si es positivo será hacia la izquierda y si es negativo a la derecha
el tercer parametro es el desenfoque(opcional)
el cuarto la expansión..(opcional)
y el quinto el color

además podemos colocar más de una sombra si separamos por coma(,) y volvemos a aplicar los 5 parametros

```
box-shadow: 10px 10px 15px #474343;
```

También podemos crear sombras internas si antes de los parametros colocamos el parametro `inset`



Esta propiedad aplica para objetos, si la necesitas en textos usamos

`text-shadow: 10px 10px red;`


Podemos usar la página https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_backgrounds_and_borders/Box-shadow_generator

para generar un elemento con sombra a nuestra medida de manera un poco más gráfica.
