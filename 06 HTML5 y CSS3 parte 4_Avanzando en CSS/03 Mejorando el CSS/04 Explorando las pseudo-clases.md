Usamos las pseudo-clases para hacer selecciones especiales en los ítems de la lista de los diferenciales y aplicar algunos efectos especiales. ¿Cuál de las alternativas está usando correctamente las pseudo-clases para obtener la **lista-ingredientes** con el resultado esperado:

```xml
<ul class="lista-ingredientes">
    <li class="items">6 huevos</li>
    <li class="items">200 grs de tocino</li>
    <li class="items">1/2 pimentón</li>
    <li class="items">1 tomate</li>
    <li class="items">1 cuchara de aceite</li>
    <li class="items">150 grs de queso muzzarella</li>
    <li class="items">Sal a gusto</li>
</ul>
```

**Resultado esperado:**

- _6 huevos_
- 200 grs de tocino
- 1/2 pimentón
- **1 tomate**
- 1 cuchara de aceite
- 150 grs de queso muzzarella
- _Sal a gusto_

- Alternativa correta
    
    ```css
    .items:first-child{font-style: italic}
    .items:nth-child(4){font-weight: bold}
    .items:last-child{font-style: italic}
    ```
    
    ¡Alternativa correcta! La sintaxis de las pseudo-clases están correctamente usadas y aplicando los estilos requeridos para colocar formato itálico en el primer y último ítem. Y pintar de negrito el cuarto ítem.