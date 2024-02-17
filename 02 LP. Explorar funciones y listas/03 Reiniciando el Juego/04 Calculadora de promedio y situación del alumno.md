Has sido contratado(a) para desarrollar una calculadora que calcula el promedio y así verificar la situación de aprobación de un estudiante en función de sus cuatro notas. El promedio requerido para aprobar es de mínimo 5. Tu tarea es implementar dos funciones en JavaScript:

- `calcularPromedio(nota1, nota2, nota3, nota4)` => Esta función recibe las cuatro notas del estudiante como parámetros y devuelve el promedio calculado con base en esas notas.
- `verificarAprobacion(promedio)` => Esta función recibe el promedio del estudiante como parámetro y devuelve "Aprobado" si el promedio es mayor o igual a 5, en caso contrario, devuelve "Reprobado".

Utiliza estos valores para las calificaciones:

```bash
let nota1 = 7;
let nota2 = 6;
let nota3 = 3;
let nota4 = 5;
```

- Alternativa correta
    
    [ ] ```javascript
    function calcularPromedio(nota1, nota2, nota3, nota4){
            let promedio = (nota1 +  nota2 +  nota3 +  nota4)/4
            return promedio;
    }
    ```
    
    Esa función realiza el calculo del promedio y devuelve el valor como retorno de la función.
    
- Alternativa correta
    
    [ ] ```javascript
    function calcularPromedio(nota1, nota2, nota3, nota4){
            let promedio = (nota1 +  nota2 +  nota3 +  nota4)/4
    }
    ```
    
- Alternativa correta
    
    [ ] ```csharp
    function verificarAprobacion(){
             return promedio >= 6;
    }
    ```
    
- Alternativa correta
    
    [ ] ```javascript
    function verificarAprobacion(promedio){
             return promedio >= 5 ? “Aprobado” : “Reprobado”;
    }
    ```
    
    ¡Exacto! La función verifica si el promedio pasado como parámetro es mayor o igual a 5 y devuelve un valor en formato de texto que informa si fue aprobado o reprobado.