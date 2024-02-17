Eres una persona recién llegada al equipo de desarrollo de Jornada Millas, un sitio web de compra de paquetes de viaje para los principales destinos del mundo.

Como primera tarea, tu liderazgo te ha pedido que corrijas un error que ha estado ocurriendo cuando un cliente del sitio intenta utilizar sus millas de tarjeta de crédito para obtener un descuento en los paquetes de viaje. Para esto, se te ha presentado el siguiente código:

```bash
let porcentajeDescuento = 0;

if (cantidadMillas > 30000) {
    porcentajeDescuento = 20;
} else if (cantidadMillas > 5000) {
    porcentajeDescuento = 10;
} else {
    porcentajeDescuento = 0;
}
```

Para ayudarte a comprender el origen del error, tu liderazgo explicó la regla de negocio utilizada para las compras de paquetes de viaje con millas:

- Personas con una cantidad de millas inferior a 5,000 no reciben descuento.
- Personas con una cantidad de millas superior a 30,000 reciben un 20% de descuento.
- Personas con una cantidad de millas superior a 5,000, pero inferior a 30,000 reciben un 10% de descuento.

Sin embargo, según los informes de los clientes, al intentar usar el descuento de 5,000 millas, no se aplica ningún descuento. Los clientes con más de 30,000 millas están recibiendo un descuento superior al que deberían recibir.

¿Cómo podrías modificar el código para que funcione correctamente? Selecciona la opción correcta:

- Alternativa correta
    
    Hacer con que el descuento no sea somado , apenas definido con base en las millas, como:
    
    ```bash
    let porcentajeDescuento = 0;
    
    if (cantidadDeMillas > 5000) {
        porcentajeDescuento = 10;
    }
    
    if (cantidadDeMillas > 30000) {
        porcentajeDescuento = 20;
    } else {
        porcentajeDescuento = 0;
    }
    ```
    
- Alternativa correta
    
    Removendo el bloque ‘else’ de la estructura condicional
    
- Alternativa correta
    
    Agregando otro bloque ‘else’, referente al bloque ‘if(cantidad SeMillas>5000), como el código:
    
    ```bash
    if (cantidadDeMillas > 5000) {
        porcentajeDescuento = porcentajeDescuento + 10;
    } else {
        porcentajeDescuento = porcentajeDescuento + 20;
    }
    
    if (cantidadDeMillas > 30000) {
        porcentajeDescuento = porcentajeDescuento + 20;
    } else {
        porcentajeDescuento = 0;
    }
    ```
    
- Alternativa correta
    
    Haciendo la utilización de un bloque ‘if’ dentro del bloque ‘else’,como:
    
    ```bash
    let porcentajeDescuento = 0;
    
    if (cantidadDeMillas > 30000) {
        porcentajeDescuento = porcentajeDescuento + 20;
    } else {
        if (cantidadDeMillas > 5000) {
            porcentajeDescuento = porcentajeDescuento + 10;
        }
    }
    ```
    
    La inclusión del bloque 'if' dentro del bloque 'else' garantiza que si la cantidad de millas es superior a 30000, el descuento será del 20%, y si no supera este valor pero es superior a 5000, el descuento será del 10%. En el caso de que la cantidad de millas sea inferior a 5000, el descuento permanecerá en cero, ya que no se cumple el requisito mínimo para obtener un descuento.