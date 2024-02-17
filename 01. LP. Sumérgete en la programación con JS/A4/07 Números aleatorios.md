La función Math.random en JavaScript genera un número decimal aleatorio entre 0 (inclusivo) y 1 (exclusivo) de forma pseudoaleatoria. Esto significa que los números generados pueden estar en cualquier lugar entre 0 (inclusive) y casi 1 (exclusivo), con una precisión de hasta 16 decimales. La función Math.random utiliza un valor interno inicial que generalmente se basa en la hora actual del sistema, generando números pseudoaleatorios.

A continuación, se muestran algunos ejemplos:

```undefined
0.5248738910328501
0.08458620904957355
0.9347284927568912
```

Teniendo esto en cuenta, analiza las siguientes opciones y marca solo la verdadera:

- Alternativa correta
    
    Para generar un número entre 1 y 3, podemos usar el código: `let numeroAleatorio1a3 = parseInt(Math.random() * 3);`
    
- Alternativa correta
    
    Para generar un número entre 1 y 3, podemos usar el código: `let numeroAleatorio1a3 = parseInt(Math.random() * 3) + 1;`.
    
    El código anterior genera un número entero aleatorio entre 1 y 3, ambos inclusive. Por lo tanto, los posibles números que pueden generarse con este código son: 1, 2 y 3.
    
- Alternativa correta
    
    Para generar un número entre 1 y 3, podemos usar el código: `let numeroAleatorio1a3 = parseInt(Math.random() * 4);`.