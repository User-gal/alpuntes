Los Template strings, o plantillas de cadenas, son características comunes en muchos lenguajes de programación y sistemas de plantillas. Estas plantillas ofrecen una manera eficiente de crear cadenas de texto donde es posible incluir marcadores o espacios reservados que posteriormente serán reemplazados por valores concretos. Estos marcadores, por lo general, se encuentran delimitados por caracteres especiales, como llaves, corchetes o signos de dólar, y desempeñan el papel de puntos de inserción para datos dinámicos.

En la gran mayoría de los lenguajes de programación, Template strings simplifican la tarea de concatenar valores variables en una cadena, sin requerir concatenación manual de cadenas o conversiones explícitas de tipos. Esto contribuye a que el código sea más legible y menos propenso a errores, lo cual es particularmente valioso en diversas situaciones, como la generación de mensajes de usuario, la construcción de consultas SQL dinámicas o la creación de documentos HTML.

Un ejemplo ilustrativo de esto se encuentra en JavaScript, donde puedes emplear las comillas invertidas (backticks) para crear plantillas de cadenas. Esto te permite incrustar expresiones dentro de la cadena utilizando el formato ${}. A continuación, un ejemplo práctico:

```javascript
const nombre = "Juan";
const edad = 30;
const mensaje = `Hola, soy ${nombre} y tengo ${edad} años.`;
console.log(mensaje);

// Salida: Hola, soy Juan y tengo 30 años.
```

En este ejemplo, la plantilla de cadena permite insertar dinámicamente los valores de las variables nombre y edad en la cadena de texto.

Si quieres profundizar más sobre Template strings te dejamos este [artículo](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Template_literals).

# Plantillas literales (plantillas de cadenas)

Las plantillas literales son cadenas literales que habilitan el uso de expresiones incrustadas. Con ellas, es posible utilizar cadenas de caracteres de más de una línea, y funcionalidades de interpolación de cadenas de caracteres.

En ediciones anteriores de la especificación ES2015, solían llamarse "plantillas de cadenas de caracteres".

## [Sintaxis](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Template_literals#sintaxis)

`texto de cadena de caracteres`

`línea 1 de la cadena de caracteres
  línea 2 de la cadena de caracteres`

`texto de cadena de caracteres ${expresión} texto adicional`

etiqueta`texto de cadena de caracteres ${expresión} texto adicional`

## [Descripción](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Template_literals#descripci%C3%B3n)

Las plantillas literales se delimitan con el caracter de comillas o tildes invertidas (` `) ([grave accent](http://en.wikipedia.org/wiki/Grave_accent)), en lugar de las comillas sencillas o dobles.

Las plantillas de cadena de caracteres pueden contener marcadores, identificados por el signo de dólar y envueltos en llaves (`${expresión}`). Las expresiones contenidas en los marcadores, junto con el texto entre ellas, son enviados como argumentos a una función.

La función por defecto sencillamente concatena las partes para formar una única cadena de caracteres. Si hay una expresión antes de la plantilla literal (aquí indicada mediante _`etiqueta`_), se le conoce como "plantilla etiquetada". En este caso, la expresión de etiqueta (típicamente una función) es llamada con la plantilla literal como parámetro, que luego puede ser manipulada antes de ser devuelta.

En caso de querer escapar una comilla o tilde invertida en una plantilla literal, se debe poner una barra invertida (`\`) antes de la comilla o tilde invertida.

JSCopy to Clipboard

```
`\`` === "`"; // --> true (cierto)
```

### [Cadenas de más de una línea](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Template_literals#cadenas_de_m%C3%A1s_de_una_l%C3%ADnea)

Los caracteres de fin de línea encontrados forman parte de la plantilla literal.

Utilizando cadenas de caracteres normales, sería necesario utilizar la siguiente sintaxes para producir cadenas de más de una línea:

JSCopy to Clipboard

```
console.log("línea 1 de cadena de texto\n" + "línea 2 de cadena de texto");
// "línea 1 de cadena de texto
// línea 2 de cadena de texto"
```

Utilizando plantillas literales, se puede obtener el mismo resultado de la siguiente forma:

JSCopy to Clipboard

```
console.log(`línea 1 de la cadena de texto
línea 2 de la cadena de texto`);
// "línea 1 de la cadena de texto
// línea 2 de la cadena de texto"
```

### [Interpolación de expresiones](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Template_literals#interpolaci%C3%B3n_de_expresiones)

Para insertar expresiones dentro de cadenas de caracteres normales, se utilizaría la siguiente sintaxis:

JSCopy to Clipboard

```
let a = 5;
let b = 10;
console.log("Quince es " + (a + b) + " y\nno " + (2 * a + b) + ".");
// "Quince es 15 y
// no 20."
```

Ahora, con las plantillas literales, se pueden utilizar sus nuevas capacidades (es decir, insertar expresiones con `${ }` e incluir caracteres de fin de linea literales dentro de la cadena) para simplificar la sintaxis:

JSCopy to Clipboard

```
let a = 5;
let b = 10;
console.log(`Quince es ${a + b} y
no ${2 * a + b}.`);
// "Quince es 15 y
// no 20."
```

### [Anidamiento de plantillas](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Template_literals#anidamiento_de_plantillas)

En ciertos casos, anidar una plantilla es la forma más fácil, e incluso más legible, de tener cadenas configurables. Dentro de una plantilla con tildes invertidas, es sencillo permitir tildes invertidas interiores simplemente usándolas dentro de un marcador de posición `${ }` dentro de la plantilla.

Por ejemplo, si la condición a es `true` (cierta): entonces `return` (devuelva) este literal con plantilla.

En ES5:

JSCopy to Clipboard

```
let classes = "header";
classes += isLargeScreen()
  ? ""
  : item.isCollapsed
    ? " icon-expander"
    : " icon-collapser";
```

En ES2015 con plantillas literales y sin anidamiento:

JSCopy to Clipboard

```
const classes = `header ${
  isLargeScreen() ? "" : item.isCollapsed ? "icon-expander" : "icon-collapser"
}`;
```

En ES5 con plantillas literales anidadas:

JSCopy to Clipboard

```
const classes = `header ${
  isLargeScreen() ? "" : `icon-${item.isCollapsed ? "expander" : "collapser"}`
}`;
```

### [Plantillas etiquetadas](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Template_literals#plantillas_etiquetadas)

Una forma más avanzada de plantillas literales son las plantillas _etiquetadas_.

Con ellas es posible modificar la salida de las plantillas utilizando una función. El primer argumento contiene un array con una o más cadenas de caracteres. El segundo y subsiguientes argumentos se asocian con las expresiones de la plantilla.

La función de etiqueta puede ejecutar cualesquiera operaciones deseadas con estos argumentos, y luego devolver la cadena manipulada. (También puede devolver algo totalmente distinto, como se muestra en uno de los siguientes ejemplos.)

El nombre de la función utilizada con la etiqueta no es nada especial, se puede utilizar cualquier nombre de función en su lugar.

JSCopy to Clipboard

```
let persona = "Mike";
let edad = 28;

function myTag(strings, expPersona, expEdad) {
  let str0 = strings[0]; // "Ese "
  let str1 = strings[1]; // " es un "

  // Tecnicamente, hay una cadena de
  // caracteres después de la expresión
  // final (en nuestro ejemplo) pero
  // está vacia (""), asi que se ignora.
  // let str2 = strings[2];

  let strEdad;
  if (expEdad > 99) {
    strEdad = "viejo";
  } else {
    strEdad = "joven";
  }

  // Podemos incluso retornar una cadena de
  // caracteres utilizando una plantilla literal.
  return `${str0}${expPersona}${str1}${strEdad}`;
}

var salida = myTag`Ese ${persona} es un ${edad}`;

console.log(salida);
// Ese Mike es un joven
```

Las funciones de etiqueta incluso pueden devolver valores que no sean cadenas de caracteres:

JSCopy to Clipboard

```
function plantilla(cadenas, ...claves) {
  return function (...valores) {
    let diccio = valores[valores.length - 1] || {};
    let resultado = [cadenas[0]];
    claves.forEach(function (clave, i) {
      let valor = Number.isInteger(clave) ? valores[clave] : diccio[clave];
      resultado.push(valor, cadenas[i + 1]);
    });
    return resultado.join("");
  };
}

let t1Closure = plantilla`¡${0}${1}${2}${2}${3}!`;
//let t1Closure = plantilla(["¡","","","","","","!"],0,1,2,3);
t1Closure("H", "U", "R", "A"); // "¡HURRA!"

let t2Closure = plantilla`${0} ${"foo"}!`;
//let t2Closure = plantilla(["¡",""," ","!"],0,"foo");
t2Closure("Hola", { foo: "Mundo" }); // "¡Hola Mundo!"

let t3Closure = plantilla`Me llamo ${"nombre"}. Tengo casi ${"edad"} años.`;
//let t3Closure = plantilla(["Me llamo ", ". Tengo casi ", " años."], "nombre", "edad");
t3Closure("foo", { nombre: "MDN", edad: 30 }); //"Me llamo MDN. Tengo casi 30 años."
t3Closure({ nombre: "MDN", edad: 30 }); //"Me llamo MDN. Tengo casi 30 años."
```

### [Cadenas en crudo (raw)](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Template_literals#cadenas_en_crudo_raw)

La propiedad especial `raw`, disponible en el primer argumento de la función de etiqueta, permite acceso a las cadenas de caracteres tal como fueron ingresadas, sin procesar [secuencias de escape](https://developer.mozilla.org/es/docs/Web/JavaScript/Guide/Grammar_and_types#literales_string).

JSCopy to Clipboard

```
function etiqueta(cadenas) {
  console.log(cadenas.raw[0]);
}

etiqueta`texto de cadena de caracteres 1 \n texto de cadena de caracteres 2`;
// muestra "texto de cadena de caracteres 1 \n texto de cadena de caracteres 2" ,
// incluyendo los caracteres '\' y 'n'
```

Adicionalmente, el método [`String.raw()`](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Global_Objects/String/raw) permite crear cadenas de caracteres en crudo tal como serían generadas por la función por defecto de plantilla, concatenando sus partes.

JSCopy to Clipboard

```
let cadena = String.raw`¡Hola\n${2 + 3}!`;
// "¡Hola\n5!"

cadena.length;
// 9

Array.from(cadena).join(",");
// "¡,H,o,l,a,\,n,5,!"
```

### [Plantillas etiquetadas y secuencias de escape](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Template_literals#plantillas_etiquetadas_y_secuencias_de_escape)

#### Comportamiento en ES2016

Comenzando con ECMAScript 2016, las plantillas etiquetadas se comportan de acuerdo con las normas de las siguientes secuencias de escape:

- Secuencias de escape de formato Unicode comenzando con "`\u`", como `\u00A9`
- Secuencias de escape de formato Unicode de punto de código, indicadas con "`\u{}`", como `\u{2F804}`
- Secuencias de escape de numeros hexadecimales comenzando con "`\x`", como `\xA9`
- Secuencias de escape de octales literales comenzando con "`\0o`" seguidas de uno o más dígitos, como `\0o251`

Esto significa que una plantilla etiquetada como la siguiente podría causar problemas, dado que, de acuerdo con la gramática de ECMAScript, un analizador buscará secuencias de escape de formato Unicode válidas pero encontrará sintaxis equivocado:

JSCopy to Clipboard

```
latex`\unicode`;
// En ECMAScript 2016 y versiones anteriores, lanza
// SyntaxError: malformed Unicode character escape sequence
```

### [Revision de secuencias de escape no permitidas en ES2018](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Template_literals#revision_de_secuencias_de_escape_no_permitidas_en_es2018)

Las plantillas etiquetadas deberías permitir la inserción de lenguages (como los [DSL](https://en.wikipedia.org/wiki/Domain-specific_language), o [LaTeX](https://en.wikipedia.org/wiki/LaTeX)), en donde otras secuencias de escape se ven comúnmente. La propuesta para ECMAScript [Template Literal Revision](https://tc39.es/proposal-template-literal-revision/) (Revisión de Plantilla Literal) (Cuarta Etapa, en camino a ser integrada al estándar de ECMAScript 2018) elimina la restricción de las secuencias de escape en ECMAScript para las plantillas etiquetadas.

Aún así, las secuencias de escape no permitidas deben ser representadas en la representación "cocinada" de la cadena. Aparecerán como elementos [no definidos](https://developer.mozilla.org/es/docs/Glossary/Undefined) en el array llamado "cocinado" en el siguiente ejemplo.

JSCopy to Clipboard

```
function latex(str) {
  return { cocinado: str[0], "en crudo": str.raw[0] };
}

latex`\unicode`;

// { cocinado: undefined, en crudo: "\\unicode" }
```

Cabe destacar que la restricción para secuencias de escape solo ha sido eliminada para plantillas _etiquetadas_. Aún permanece para plantillas literales sin etiqueta:

JSCopy to Clipboard

```
let bad = `bad escape sequence: \unicode`;
```