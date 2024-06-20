# ¿Qué diferencia a Javascript de cualquier otro lenguaje de programación?

### **_JavaScript es un lenguaje de programación único en varios aspectos, lo que lo distingue de otros lenguajes de programación. Aquí hay una explicación extendida sobre sus características distintivas:_**

### 1. Orientación al Cliente (Client-Side)

JavaScript se desarrolló originalmente para ejecutarse en el navegador del usuario, lo que se conoce como programación del lado del cliente (client-side). Esta capacidad le permite manipular el contenido de una página web en tiempo real sin necesidad de recargar la página, proporcionando una experiencia de usuario interactiva. Aunque otros lenguajes como PHP o Python también pueden generar contenido web, normalmente lo hacen del lado del servidor, enviando páginas completas en respuesta a cada solicitud del usuario.

### 2. Ejecución Asíncrona

JavaScript tiene capacidades de programación asíncrona integradas a través de callbacks, promesas y la sintaxis async/await. Esto es crucial para operaciones como solicitudes HTTP, temporizadores y eventos de usuario, permitiendo que el código continúe ejecutándose mientras espera que estas operaciones se completen. Otros lenguajes tienen características asíncronas, pero JavaScript lo hace de manera muy integrada y natural, debido a su uso intensivo en navegadores web.

### 3. Event-Driven

JavaScript se basa en un modelo de programación orientado a eventos, donde la ejecución del código está impulsada por eventos como clics del usuario, movimientos del ratón, y respuestas del servidor. Esto contrasta con muchos lenguajes de programación tradicionales que siguen un flujo de ejecución más lineal.

### 4. Interpretado y Dinámico

JavaScript es un lenguaje interpretado, lo que significa que se ejecuta directamente en el entorno de ejecución (como el navegador web o Node.js) sin necesidad de un paso de compilación previo. Además, es dinámico, permitiendo la definición y redefinición de funciones y variables en tiempo de ejecución. Aunque otros lenguajes también pueden ser interpretados y dinámicos, en JavaScript estas características son fundamentales para su flexibilidad y adaptabilidad en el desarrollo web.

### 5. Prototipado

A diferencia de muchos lenguajes de programación que utilizan la herencia basada en clases, JavaScript utiliza un sistema de herencia basado en prototipos. En lugar de definir clases y crear instancias, en JavaScript se crean objetos que pueden servir como prototipos para otros objetos. Este modelo proporciona un enfoque diferente y más flexible para la reutilización de código y la creación de estructuras de datos complejas.

### 6. Integración con HTML/CSS

JavaScript está estrechamente integrado con HTML y CSS, los lenguajes de marcado y estilo utilizados para construir páginas web. Puede manipular el DOM (Document Object Model), que representa la estructura de un documento HTML, permitiendo cambios dinámicos en el contenido y el estilo de las páginas web. Ningún otro lenguaje de programación tiene una integración tan profunda y natural con HTML y CSS.

### 7. Ecosistema y Herramientas

El ecosistema de JavaScript es vasto y en constante crecimiento. Herramientas y librerías como React, Angular, Vue.js, y frameworks como Node.js y Express.js han revolucionado la manera en que se desarrollan aplicaciones web y de servidor. Este rico ecosistema facilita la creación de aplicaciones complejas y de alto rendimiento, tanto en el lado del cliente como en el servidor.

### 8. Uso Universal

JavaScript es el único lenguaje de programación que puede ejecutarse nativamente en todos los navegadores web modernos sin necesidad de complementos o configuraciones adicionales. Además, con la introducción de Node.js, JavaScript ha trascendido el ámbito del navegador para convertirse en una opción popular para el desarrollo de backend, lo que permite a los desarrolladores usar un solo lenguaje en ambos lados de la aplicación.

### 9. Comunidad y Soporte

JavaScript tiene una de las comunidades de desarrolladores más grandes y activas del mundo. Esto se traduce en una vasta cantidad de recursos de aprendizaje, bibliotecas de código abierto, foros de soporte, y conferencias. La comunidad contribuye continuamente a la evolución del lenguaje y sus herramientas, asegurando que JavaScript se mantenga relevante y actualizado.

### 10. Actualización Constante

JavaScript, a través del estándar ECMAScript, se actualiza regularmente, introduciendo nuevas características y mejoras. Estas actualizaciones frecuentes aseguran que el lenguaje se mantenga competitivo y capaz de manejar las demandas de las aplicaciones modernas.

**_En resumen, JavaScript se distingue de otros lenguajes de programación por su enfoque en la interactividad web del lado del cliente, su modelo de ejecución asíncrona y orientada a eventos, su sistema de prototipos, su profunda integración con HTML y CSS, su amplio y creciente ecosistema de herramientas, y su capacidad para ejecutarse de manera nativa en todos los navegadores web._**

# ¿Cuáles son algunos tipos de datos JS?

En JavaScript, los tipos de datos son fundamentales para la manipulación de valores en el código. Estos tipos se dividen en dos categorías principales: primitivos y objetos. A continuación, se presenta una explicación detallada de cada tipo de dato con ejemplos.

### 1. Tipos de Datos Primitivos

Los tipos de datos primitivos son los más básicos y no se pueden descomponer en otros tipos. En JavaScript, hay siete tipos de datos primitivos.

- a. Number
  Este tipo de dato incluye tanto números enteros como números de punto flotante. JavaScript utiliza un único tipo de datos numéricos para representar ambos.

```javascript
let entero = 42;
let decimal = 3.14;

console.log(entero); // Salida: 42
console.log(decimal); // Salida: 3.14
```

- b. String
  Los strings (cadenas de caracteres) representan texto. Pueden definirse usando comillas simples ('), comillas dobles ("), o backticks (`) para plantillas literales.

```javascript
let simple = "Hola";
let doble = "Mundo";
let template = `Hola, ${doble}`;

console.log(simple); // Salida: Hola
console.log(doble); // Salida: Mundo
console.log(template); // Salida: Hola, Mundo
```

- c. Boolean
  Este tipo de dato solo puede tener dos valores: true o false.

```javascript
let verdadero = true;
let falso = false;

console.log(verdadero); // Salida: true
console.log(falso); // Salida: false
```

- d. Null
  null es un valor especial que representa la ausencia de valor. Es intencionadamente asignado a una variable para indicar que no tiene valor.

```javascript
let vacio = null;

console.log(vacio); // Salida: null
```

- e. Undefined
  undefined indica que una variable ha sido declarada pero no ha sido asignada un valor.

```javascript
let indefinido;

console.log(indefinido); // Salida: undefined
```

- f. Symbol
  Symbol es un tipo de dato único y no modificable que se utiliza para crear identificadores únicos.

```javascript
let simbolo1 = Symbol("descripcion");
let simbolo2 = Symbol("descripcion");

console.log(simbolo1 === simbolo2); // Salida: false
```

- g. BigInt
  BigInt se utiliza para representar números enteros que son demasiado grandes para ser representados por el tipo Number.

```javascript
let numeroGrande = BigInt(123456789012345678901234567890);

console.log(numeroGrande); // Salida: 123456789012345678901234567890n
```

### 1. Tipos de Datos Objeto

Los objetos en JavaScript son colecciones de pares clave-valor y pueden contener otros tipos de datos, incluidos primitivos y otros objetos.

- a. Object
  Un objeto es una colección de propiedades, y una propiedad es una asociación entre un nombre (o clave) y un valor.

```javascript
let persona = {
  nombre: "Juan",
  edad: 30,
  esEstudiante: true,
};

console.log(persona.nombre); // Salida: Juan
console.log(persona["edad"]); // Salida: 30
```

- b. Array
  Un array es una colección de elementos ordenados que pueden ser accedidos por un índice.

```javascript
let numeros = [1, 2, 3, 4, 5];

console.log(numeros[0]); // Salida: 1
console.log(numeros.length); // Salida: 5
```

- c. Function
  Las funciones son objetos que pueden ser invocados. En JavaScript, las funciones son ciudadanos de primera clase, lo que significa que pueden ser asignadas a variables, pasadas como argumentos y retornadas por otras funciones.

```javascript
function saludar(nombre) {
  return `Hola, ${nombre}`;
}

console.log(saludar("Ana")); // Salida: Hola, Ana
```

- d. Date
  El objeto Date se utiliza para trabajar con fechas y horas.

```javascript
let ahora = new Date();

console.log(ahora); // Salida: La fecha y hora actuales
```

- e. RegExp
  El objeto RegExp representa una expresión regular y se utiliza para hacer coincidir texto con un patrón.

```javascript
let patron = /hola/i; // La 'i' indica que es insensible a mayúsculas

console.log(patron.test("Hola mundo")); // Salida: true
```

Ejemplos Prácticos
A continuación, algunos ejemplos prácticos que combinan diferentes tipos de datos.

Ejemplo 1:

Combinando Primitivos y Objetos

```javascript
let libro = {
  titulo: "El Quijote",
  autor: "Miguel de Cervantes",
  publicacion: new Date(1605, 0, 1),
  generos: ["Novela", "Aventura", "Ficción"],
  disponible: true,
};

console.log(
  `${libro.titulo} fue escrito por ${
    libro.autor
  } y publicado el ${libro.publicacion.toDateString()}`
);
console.log(`Géneros: ${libro.generos.join(", ")}`);
console.log(`Disponible: ${libro.disponible ? "Sí" : "No"}`);
```

Ejemplo 2:

Funciones y Arrays

```javascript
let numeros = [1, 2, 3, 4, 5];

function sumar(array) {
  let suma = 0;
  for (let numero of array) {
    suma += numero;
  }
  return suma;
}

console.log(`La suma de los números es: ${sumar(numeros)}`); // Salida: La suma de los números es: 15
```

"**_Estos ejemplos ilustran cómo se utilizan los diferentes tipos de datos en JavaScript y cómo se combinan para crear estructuras de datos complejas y funcionales. Cada tipo de dato tiene sus propias características y usos específicos, lo que hace que JavaScript sea un lenguaje versátil y poderoso._**"

# ¿Cuáles son las tres funciones de String en JS?

En JavaScript, las cadenas de caracteres (strings) tienen varios métodos integrados que permiten realizar diversas operaciones sobre ellas. A continuación se detallan tres de estas funciones, junto con ejemplos para ilustrar su uso:

### 1. substring()

El método substring() devuelve una parte del string entre dos índices especificados. El primer índice es inclusivo y el segundo es exclusivo. Si solo se proporciona un índice, substring() extrae caracteres desde esa posición hasta el final del string.

Ejemplos:

```javascript
let texto = "Hola, Mundo";

// Extraer desde el índice 0 hasta el 4 (sin incluir el 4)
let subTexto1 = texto.substring(0, 4);
console.log(subTexto1); // Salida: Hola

// Extraer desde el índice 7 hasta el final
let subTexto2 = texto.substring(7);
console.log(subTexto2); // Salida: Mundo

// Extraer desde el índice 7 hasta el 12 (sin incluir el 12)
let subTexto3 = texto.substring(7, 12);
console.log(subTexto3); // Salida: Mundo

// Si el primer índice es mayor que el segundo, se invierten
let subTexto4 = texto.substring(12, 7);
console.log(subTexto4); // Salida: Mundo
```

### 2. toLowerCase()

El método toLowerCase() convierte todos los caracteres de un string a minúsculas y devuelve el nuevo string. Este método no modifica el string original, sino que devuelve una nueva cadena con los cambios aplicados.

Ejemplos:

```javascript
Copiar código
let texto = "Hola, Mundo";

// Convertir todo el texto a minúsculas
let minusculas = texto.toLowerCase();
console.log(minusculas); // Salida: hola, mundo

// Texto original permanece sin cambios
console.log(texto); // Salida: Hola, Mundo

// Convertir un string que ya está en minúsculas
let textoMin = "javascript";
let resultadoMin = textoMin.toLowerCase();
console.log(resultadoMin); // Salida: javascript
```

### 3. replace()

El método replace() reemplaza un substring específico dentro de una cadena por otro substring. Solo reemplaza la primera ocurrencia del substring a menos que se use una expresión regular global.

Ejemplos:

```javascript
Copiar código
let texto = "Hola, Mundo";

// Reemplazar la primera aparición de "Mundo" por "JavaScript"
let nuevoTexto1 = texto.replace("Mundo", "JavaScript");
console.log(nuevoTexto1); // Salida: Hola, JavaScript

// Reemplazar usando una expresión regular (sin global)
let texto2 = "Perro, perro, perro";
let nuevoTexto2 = texto2.replace(/perro/i, "gato");
console.log(nuevoTexto2); // Salida: Gato, perro, perro

// Reemplazar todas las ocurrencias usando una expresión regular global
let nuevoTexto3 = texto2.replace(/perro/gi, "gato");
console.log(nuevoTexto3); // Salida: Gato, gato, gato

// Reemplazar utilizando una función
let texto3 = "1 + 2 = 3";
let nuevoTexto4 = texto3.replace(/\d+/g, (match) => parseInt(match) * 2);
console.log(nuevoTexto4); // Salida: 2 + 4 = 6
```

Resumen de los Métodos

- substring(start, end): Extrae una parte de la cadena entre los índices start (inclusivo) y end (exclusivo).
- toLowerCase(): Convierte todos los caracteres de la cadena a minúsculas.
- replace(searchValue, newValue): Reemplaza la primera aparición de searchValue con newValue. Puede usar expresiones regulares para reemplazar múltiples ocurrencias

"**_Estos métodos son fundamentales para la manipulación de strings en JavaScript y se utilizan ampliamente en diversas aplicaciones y situaciones de desarrollo."_**

# ¿Qué es un condicional?

Un condicional es una estructura de control en programación que permite ejecutar diferentes bloques de código basados en la evaluación de una condición. En JavaScript, los condicionales más comunes son if, else if, else y el operador ternario. A continuación, se presentan explicaciones detalladas y ejemplos para cada uno de estos tipos de condicionales.

### 1. if

La declaración if evalúa una condición dentro de paréntesis. Si la condición es verdadera, ejecuta el bloque de código asociado.

Sintaxis:

```javascript
if (condición) {
  // bloque de código que se ejecuta si la condición es verdadera
}
```

Ejemplo:

```javascript
let edad = 20;

if (edad >= 18) {
  console.log("Eres mayor de edad");
}
// Salida: Eres mayor de edad
```

### 2. else

La declaración else se usa junto con if para ejecutar un bloque de código diferente si la condición en el if es falsa.

Sintaxis:

```javascript
if (condición) {
  // bloque de código que se ejecuta si la condición es verdadera
} else {
  // bloque de código que se ejecuta si la condición es falsa
}
```

Ejemplo:

```javascript
let edad = 16;

if (edad >= 18) {
  console.log("Eres mayor de edad");
} else {
  console.log("Eres menor de edad");
}
// Salida: Eres menor de edad
```

### 3. else if

La declaración else if permite verificar múltiples condiciones. Si la condición del if inicial es falsa, se evalúan las condiciones de los else if sucesivos. Si ninguna de las condiciones es verdadera, se puede usar un else final.

Sintaxis:

```javascript
if (condición1) {
  // bloque de código que se ejecuta si condición1 es verdadera
} else if (condición2) {
  // bloque de código que se ejecuta si condición2 es verdadera
} else {
  // bloque de código que se ejecuta si ninguna de las condiciones anteriores es verdadera
}
```

Ejemplo:

```javascript
let hora = 15;

if (hora < 12) {
  console.log("Buenos días");
} else if (hora < 18) {
  console.log("Buenas tardes");
} else {
  console.log("Buenas noches");
}
// Salida: Buenas tardes
```

### 4. Condicionales Anidados

Los condicionales anidados son if dentro de otro if. Permiten manejar decisiones más complejas.

Ejemplo:

```javascript
let puntuacion = 85;

if (puntuacion >= 60) {
  console.log("Aprobado");
  if (puntuacion >= 90) {
    console.log("Excelente");
  } else if (puntuacion >= 75) {
    console.log("Bueno");
  } else {
    console.log("Suficiente");
  }
} else {
  console.log("Reprobado");
}
// Salida: Aprobado
//         Bueno
```

### 5. Operador Ternario

El operador ternario es una forma concisa de realizar una verificación if-else. Tiene la forma condición ? expresión_verdadera : expresión_falsa.

Sintaxis:

```javascript
condición ? expresión_verdadera : expresión_falsa;
```

Ejemplo:

```javascript
let edad = 20;
let mensaje = edad >= 18 ? "Eres mayor de edad" : "Eres menor de edad";

console.log(mensaje); // Salida: Eres mayor de edad
```

### 6. switch

La declaración switch se utiliza para ejecutar uno de varios bloques de código según el valor de una expresión. Es útil cuando se necesitan múltiples comparaciones basadas en el mismo valor.

Sintaxis:

```javascript
switch (expresión) {
  case valor1:
    // bloque de código que se ejecuta si expresión === valor1
    break;
  case valor2:
    // bloque de código que se ejecuta si expresión === valor2
    break;
  // más casos...
  default:
  // bloque de código que se ejecuta si ninguno de los casos anteriores es verdadero
}
```

Ejemplo:

```javascript
let dia = 3;
let nombreDia;

switch (dia) {
  case 1:
    nombreDia = "Lunes";
    break;
  case 2:
    nombreDia = "Martes";
    break;
  case 3:
    nombreDia = "Miércoles";
    break;
  case 4:
    nombreDia = "Jueves";
    break;
  case 5:
    nombreDia = "Viernes";
    break;
  case 6:
    nombreDia = "Sábado";
    break;
  case 7:
    nombreDia = "Domingo";
    break;
  default:
    nombreDia = "Día inválido";
}

console.log(nombreDia); // Salida: Miércoles
```

## Resumen

- if: Evalúa una condición y ejecuta un bloque de código si la condición es verdadera.
- else: Se ejecuta si la condición del if es falsa.
- else if: Evalúa una nueva condición si la condición del if inicial es falsa.
- Condicionales Anidados: Permiten manejar decisiones más complejas anidando if dentro de otro if.
- Operador Ternario: Proporciona una forma concisa de escribir una declaración if-else.
- switch: Ejecuta uno de varios bloques de código según el valor de una expresión.
- Los condicionales son fundamentales para la toma de decisiones en el flujo del programa y permiten ejecutar diferentes bloques de código basados en diversas condiciones.

# ¿Qué es un operador ternario?

El operador ternario es una forma concisa de realizar una verificación if-else en una sola línea. En JavaScript, se utiliza para asignar valores a variables basándose en una condición. Su sintaxis es:

```javascript
condición ? expresión_si_verdadera : expresión_si_falsa;
```

Desglose de la Sintaxis

- condición: Es una expresión que se evalúa como verdadera (true) o falsa (false).
  expresión_si_verdadera: Es la expresión que se ejecuta y devuelve un valor si la condición es verdadera.
- expresión_si_falsa: Es la expresión que se ejecuta y devuelve un valor si la condición es falsa.
  Ejemplos

- Ejemplo 1:
  Asignación de un valor basado en una condición
  En este ejemplo, se determina si una persona es mayor de edad basándose en su edad.

```javascript
let edad = 20;
let mensaje = edad >= 18 ? "Eres mayor de edad" : "Eres menor de edad";

console.log(mensaje); // Salida: Eres mayor de edad
```

Aquí, la condición edad >= 18 se evalúa. Si es verdadera, mensaje se establece en "Eres mayor de edad"; de lo contrario, se establece en "Eres menor de edad".

- Ejemplo 2:
  Asignación múltiple
  El operador ternario se puede encadenar para manejar múltiples condiciones. Sin embargo, para mejorar la legibilidad, es recomendable usar estructuras if-else if-else cuando se encadenan muchas condiciones.

```javascript
let puntuacion = 85;
let calificacion =
  puntuacion >= 90
    ? "A"
    : puntuacion >= 80
    ? "B"
    : puntuacion >= 70
    ? "C"
    : puntuacion >= 60
    ? "D"
    : "F";

console.log(calificacion); // Salida: B
```

En este ejemplo, se evalúan varias condiciones secuencialmente. Si puntuacion es 85, se cumple puntuacion >= 80, por lo que calificacion se establece en "B".

- Ejemplo 3:
  Valores por defecto
  El operador ternario puede ser útil para asignar valores predeterminados si no se cumplen ciertas condiciones.

```javascript
let usuario = {
  nombre: "Juan",
  edad: 30,
};

let nombreUsuario = usuario.nombre ? usuario.nombre : "Anónimo";

console.log(nombreUsuario); // Salida: Juan`
```

Si usuario.nombre es verdadero (existe y no es una cadena vacía), nombreUsuario se establece en usuario.nombre. Si no, se establece en "Anónimo".

- Ejemplo 4:
  Uso en funciones
  El operador ternario también se puede utilizar dentro de funciones para retornar valores basados en una condición.

```javascript
function obtenerEstado(edad) {
  return edad >= 18 ? "Mayor de edad" : "Menor de edad";
}

console.log(obtenerEstado(20)); // Salida: Mayor de edad
console.log(obtenerEstado(16)); // Salida: Menor de edad
```

Consideraciones y Buenas Prácticas

- Legibilidad: Aunque el operador ternario es útil para simplificar código, su uso excesivo o anidado puede reducir la legibilidad del código. En casos de múltiples condiciones, es mejor usar estructuras if-else tradicionales.

- Uso Anidado: Si es necesario anidar operadores ternarios, considera usar paréntesis para mejorar la claridad.

```javascript
Copiar código
let estado = (puntuacion >= 90) ? "Excelente" :
             (puntuacion >= 75) ? "Bueno" :
             (puntuacion >= 60) ? "Suficiente" : "Insuficiente";

console.log(estado); // Basado en la puntuación
```

- Valores Retornados: Asegúrate de que las expresiones expresión_si_verdadera y expresión_si_falsa devuelvan valores del mismo tipo o que sean comparables para evitar comportamientos inesperados.

"**_El operador ternario es una herramienta poderosa y flexible en JavaScript, pero debe usarse con cuidado para mantener la claridad y legibilidad del código._**"

# ¿Cuál es la diferencia entre una declaración de función y una expresión de función?

En JavaScript, tanto las declaraciones de funciones como las expresiones de funciones se utilizan para definir funciones, pero existen diferencias clave en su sintaxis, comportamiento y uso. A continuación, se presentan una explicación detallada y ejemplos para ilustrar estas diferencias.

### Declaración de Función

Una declaración de función define una función con un nombre específico. Estas funciones son elevadas (hoisted) al inicio de su contexto de ejecución, lo que significa que se pueden llamar antes de ser definidas en el código.

Sintaxis:

```javascript
function nombreDeLaFuncion(parámetros) {
  // cuerpo de la función
}
```

Ejemplo:

```javascript
// Llamada a la función antes de su definición debido a hoisting
saludar();

function saludar() {
  console.log("Hola, mundo!");
}

// Llamada a la función después de su definición
saludar();
// Salida: Hola, mundo!
```

En este ejemplo, la función saludar puede ser llamada antes de su declaración debido a que las declaraciones de funciones son elevadas al comienzo de su contexto de ejecución.

### Expresión de Función

Una expresión de función define una función como parte de una expresión. Puede ser anónima (sin nombre) o tener un nombre. Las expresiones de funciones no son elevadas, lo que significa que no se pueden llamar antes de ser definidas.

Sintaxis:

```javascript
Copiar código
let nombreDeLaFuncion = function(parámetros) {
    // cuerpo de la función
};
```

Ejemplo:

```javascript
// Llamada a la función antes de su definición resultará en un error
// saludar(); // Error: Cannot access 'saludar' before initialization

let saludar = function () {
  console.log("Hola, mundo!");
};

// Llamada a la función después de su definición
saludar();
// Salida: Hola, mundo!
```

En este ejemplo, intentar llamar a la función saludar antes de su definición resultará en un error porque las expresiones de funciones no son elevadas.

### Diferencias Clave

1. Hoisting (Elevación)
   Declaraciones de Función: Las funciones declaradas son elevadas, por lo que se pueden llamar antes de su declaración en el código.
   Expresiones de Función: Las funciones expresadas no son elevadas, por lo que no se pueden llamar antes de su definición en el código.
   Ejemplo de Hoisting:

```javascript
// Declaración de función
miFuncionDeclarada();

function miFuncionDeclarada() {
  console.log("Esto es una declaración de función.");
}

// Expresión de función
// miFuncionExpresada(); // Error: Cannot access 'miFuncionExpresada' before initialization

let miFuncionExpresada = function () {
  console.log("Esto es una expresión de función.");
};

miFuncionExpresada(); // Salida: Esto es una expresión de función.
```

2. Anonimato
   Declaraciones de Función: Siempre tienen un nombre.
   Expresiones de Función: Pueden ser anónimas.
   Ejemplo de Función Anónima:

```javascript
let funcionAnonima = function () {
  console.log("Soy una función anónima");
};

funcionAnonima(); // Salida: Soy una función anónima
```

3. Contexto de Ejecución
   Las expresiones de función pueden ser utilizadas en cualquier contexto donde se pueda usar una expresión, como argumentos de otras funciones, valores de retorno, etc.

Ejemplo como Argumento:

```javascript
setTimeout(function () {
  console.log("Esto es una función anónima pasada como argumento");
}, 1000);
```

4. Nombres de Funciones en Expresiones de Función
   Las expresiones de función también pueden tener nombres, lo que puede ser útil para la recursión o para mejorar la legibilidad en los stack traces.

```javascript
let factorial = function f(n) {
  if (n <= 1) return 1;
  return n * f(n - 1); // Uso del nombre interno de la función
};

console.log(factorial(5)); // Salida: 120
```

En este ejemplo, f es el nombre interno de la función, lo que permite que la función se llame a sí misma recursivamente.

## Resumen

- Declaración de Función: Se eleva (hoisted), tiene un nombre y puede ser llamada antes de su definición.

```javascript
function saludar() {
  console.log("Hola");
}
```

Expresión de Función: No se eleva, puede ser anónima, y debe ser definida antes de ser llamada.

```javascript
let saludar = function () {
  console.log("Hola");
};
```

Ambas formas son útiles y se utilizan en diferentes situaciones dependiendo de las necesidades específicas del código.

# ¿Qué es la palabra clave "this" en JS?

En JavaScript, la palabra clave this es un identificador especial que hace referencia al contexto de ejecución en el que se está invocando la función. El valor de this puede variar dependiendo de cómo y dónde se utiliza. A continuación, se ofrece una explicación detallada sobre this con ejemplos para ilustrar sus diferentes comportamientos.

1. Contexto Global
   En el contexto global, fuera de cualquier función, this hace referencia al objeto global. En navegadores web, el objeto global es window.

Ejemplo:

```javascript
console.log(this); // En un navegador, esto imprimirá el objeto `window`

this.nombre = "Global";
console.log(window.nombre); // Salida: Global
```

2. Dentro de una Función (Modo No Estricto)
   Dentro de una función, cuando no se utiliza el modo estricto, this también hace referencia al objeto global (window en navegadores).

Ejemplo:

```javascript
function mostrarThis() {
  console.log(this); // En un navegador, esto imprimirá `window`
}

mostrarThis();
```

3. Dentro de una Función (Modo Estricto)
   En modo estricto ("use strict"), this dentro de una función será undefined si la función se llama directamente sin un objeto que la invoque.

Ejemplo:

```javascript
"use strict";

function mostrarThis() {
  console.log(this); // Salida: undefined
}

mostrarThis();
```

4. Métodos de un Objeto
   Cuando this se usa dentro de un método de un objeto, hace referencia al objeto que contiene el método.

Ejemplo:

```javascript
let persona = {
  nombre: "Juan",
  saludar: function () {
    console.log("Hola, " + this.nombre);
  },
};

persona.saludar(); // Salida: Hola, Juan
```

En este caso, this.nombre se refiere a la propiedad nombre del objeto persona.

5. Constructores
   En las funciones constructoras, this hace referencia a la instancia del objeto que se está creando.

Ejemplo:

```javascript
function Persona(nombre) {
  this.nombre = nombre;
}

let juan = new Persona("Juan");
console.log(juan.nombre); // Salida: Juan
```

Aquí, this.nombre se refiere a la nueva instancia de Persona.

6. Event Handlers en el DOM
   En los controladores de eventos del DOM, this hace referencia al elemento DOM que manejó el evento.

Ejemplo:

```javascript
document.getElementById("miBoton").addEventListener("click", function () {
  console.log(this); // Salida: <button id="miBoton">Click me</button>
});
```

En este ejemplo, this se refiere al elemento .< button >. que fue clicado.

7. Arrow Functions (Funciones Flecha)
   Las funciones flecha (=>) no tienen su propio valor de this. En su lugar, this en una función flecha toma el valor del this del contexto en el que se definió la función flecha.

Ejemplo:

```javascript
Copiar código
let objeto = {
    nombre: "Objeto",
    metodo: function() {
        console.log(this); // Salida: objeto
        let funcionFlecha = () => {
            console.log(this); // Salida: objeto
        };
        funcionFlecha();
    }
};
```

- objeto.metodo();
  En este ejemplo, la función flecha funcionFlecha toma el this del método metodo, que es el objeto objeto.

8. Métodos call, apply y bind
   Estos métodos se utilizan para establecer explícitamente el valor de this en una función.

- call: Llama a una función con un this y argumentos específicos.
  Ejemplo:

```javascript
function saludar(saludo) {
  console.log(saludo + ", " + this.nombre);
}

let persona = { nombre: "Juan" };

saludar.call(persona, "Hola"); // Salida: Hola, Juan
```

- apply: Similar a call, pero los argumentos se pasan como un array.

Ejemplo:

```javascript
saludar.apply(persona, ["Hola"]); // Salida: Hola, Juan
```

- bind: Crea una nueva función que, cuando se llama, tiene su this configurado a un valor específico.

Ejemplo:

```javascript
let saludarJuan = saludar.bind(persona);
saludarJuan("Hola"); // Salida: Hola, Juan
```

Resumen

- Contexto Global: this se refiere al objeto global (window en navegadores).
- Función (No Estricto): this se refiere al objeto global.
- Función (Estricto): this es undefined.
- Métodos de Objeto: this se refiere al objeto que contiene el método.
- Constructores: this se refiere a la nueva instancia creada.
- Event Handlers: this se refiere al elemento DOM que maneja el evento.
- Arrow Functions: this toma el valor del contexto donde se definió.
- call, apply, bind: Métodos para establecer explícitamente el valor de this.
- "**_Entender el comportamiento de this es crucial para escribir código JavaScript eficaz y evitar errores comunes relacionados con el contexto de ejecución._**"
