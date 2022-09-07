# Test de JavaScript
Cumplendo con el [Test de JavaScript][Test URL] del [Nuevo Curso Práctico de JavaScript][Curso URL] de [Platzi][Platzi URL] 🚀

[Test URL]: https://platzi.com/clases/3271-javascript-practico/51004-test-de-javascript/
[Curso URL]: https://platzi.com/cursos/javascript-practico/
[Platzi URL]: https://platzi.com/

## Instrucciones para tomar esta prueba
- Evalúa muy críticamente tu conocimiento.
- Si logras resolver la prueba, no importa cuánto te cueste, puedo asegurarte que tienes todo para continuar a las siguientes clases y tomar el resto del curso.
- Si no lo logras, no te preocupes, absolutamente nadie puede juzgarte, solo tú. Vuelve al [Curso Básico de JavaScript](https://platzi.com/cursos/basico-javascript/), anota los temas clave donde puedes mejorar, ubica las clases donde puedes aprenderlos y estudia vigorosamente.
- Es completamente válido hacer búsquedas en Google, cursos y tutoriales de Platzi, incluso usar tu cuaderno de notas sin importar si es físico o virtual.

Recuerda que el éxito no se mide por cuánto tiempo te toma aprender, esa métrica es relativamente inútil. Mejor concéntrate en completar los cursos de tu ruta de aprendizaje profesional y desarrollar los proyectos que realmente demuestran que dominas cada tecnología.

¡Mucha suerte!

## Variables y operaciones
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
- **¿Qué es una variable y para qué sirve?**

    Una variable es un valor que ocupa un espacio en memoria, este valor tiene un tipo de dato (String, Number, Bolean, etc.), podemos usarla para llamar ese valor cuando sea necesario, pero donde podrá ser llamada, depende del alcance (Scope) que tenga. Las variables se definen con las palabras reservadas _var_, _let_ y _const_, sin embargo, debemos tener cuidado con el tipo de dato, porque JavaScript es un lenguaje dinámico y está sujeto a la coerción.

- **¿Cuál es la diferencia entre declarar e inicializar una variable?**
  
    Cuando declaramos una variable, solo le asignando un espacio en memoria, pero al inicializarla se da un valor y declarara el tipo de dato automáticamente; en caso de no inicializarla, se le asignara el valor undefined.
  
- **¿Cuál es la diferencia entre sumar números y concatenar strings?**

    Al sumar datos numéricos estamos haciendo una operación matemática donde obtenemos un resultado según los valores ingresados, mientras que al concatenar strings, estamos uniendo los textos.

- **¿Cuál operador me permite sumar o concatenar?**

    Usamos el operador `+`, suma o concatena, dependiendo del tipo de dato de las variables.

### 2️⃣ Determina el nombre y tipo de dato para almacenar en variables la siguiente información:
- Nombre: **__String__**
- Apellido: **__String__**
- Nombre de usuario en Platzi: **__String__**
- Edad: **__Number__**
- Correo electrónico: **__String__**
- Mayor de edad: **__Bolean__**
- Dinero ahorrado: **__Number__**
- Deudas: **__Number__**

### 3️⃣ Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en los comentarios.

```js
let nombre = 'Josue';
let apellido = 'Sanchez';
let nombreUsuario = 'josueSN1402';
let edad = 20;
let mail = 'josue.sn402@gmail.com';
let mayorEdad  = true;
let dineroAhorrado  = 100;
let deudas  = 300;
```

### 4️⃣ Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:
- Nombre completo (nombre y apellido)
    ```js
    let nombre = 'Josue';
    let apellido = 'Sanchez';

    let nombreCompleto = nombre + ' ' + apellido;
    console.log('•> Nombre completo: ' + nombreCompleto);
    ```

- Dinero real (dinero ahorrado menos deudas)
    ```js
    let dineroAhorrado  = 100;
    let deudas  = 300;

    let dineroReal = dineroAhorrado - deudas;
    console.log('•> Dinero real: ' + dineroReal);
    ```

## Funciones
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
- **¿Qué es una función?**

    Una función, es un bloque de código que podemos llamar en cualquier momento, puede ser de tipo _Declarativa_ o _Expresiva_ y tener o no parámetros.

- **¿Cuándo me sirve usar una función en mi código?**

    Nos sirve cuando tenemos acciones que queremos repetir en cualquier momento y evitar reducancias en el código. Un ejemplo sencillo seria:

    ```js
    function sumar(x, y) {
        console.log(`La suma de ${x} y ${y} es igual a ${x + y}`);
    }

    sumar(3, 5);
    ```

- **¿Cuál es la diferencia entre parámetros y argumentos de una función?**

    Los parámetros son los valores pasados en los paréntesis al declarar una función, como se muestra aquí:
    ```js
    function miFuncion(parametro_01, parametro_02) {
        // Bloque de código
    }
    ```

    Y los argumentos son los valores pasados en los paréntesis al momento de llamar la función, nuevamente como se muestra aquí:
    ```js
    miFuncion(argumento_01, argumento_02);
    ```


### 2️⃣ Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:

```js
const name = "Juan David";
const lastname = "Castro Gallego";
const completeName = name + lastname;
const nickname = "juandc";

console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");
```

Solución:

```js
function saludo(name, lastname, nickname) {
    const completeName = name + ' ' + lastname;        
    console.log(`Mi nombre es ${completeName}, pero prefiero que me digas ${nickname}.`);
}

saludo('Josue', 'Sanchez', 'josueSN1402');
```

## Condicionales
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
- **¿Qué es un condicional?**

    Es una estructura que permite ejecutar determinado código, dependiendo de si la condición pasada por parámetro se cumple o no, devolviendo un valor Boleano.

- **¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?**
- **¿Puedo combinar funciones y condicionales?**

### 2️⃣ Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:
```js
const tipoDeSuscripcion = "Basic";

switch (tipoDeSuscripcion) {
   case "Free":
       console.log("Solo puedes tomar los cursos gratis");
       break;
   case "Basic":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
       break;
   case "Expert":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
       break;
   case "ExpertPlus":
       console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
       break;
}
```

Solución:
```js
const tipoDeSuscripcion = 'Basic';

if (tipoDeSuscripcion === 'Free') {
    console.log('Solo puedes tomar los cursos gratis');
} else if (tipoDeSuscripcion === 'Basic') {
    console.log('Puedes tomar casi todos los cursos de Platzi durante un mes');
} else if (tipoDeSuscripcion === 'Expert') {
    console.log('Puedes tomar casi todos los cursos de Platzi durante un año');
} else if (tipoDeSuscripcion === 'ExpertPlus') {
    console.log('Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año');
} else {
    console.log('El tipo de suscripción ingresado no es valido');
}
```

### 3️⃣ Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).
💡 Bonus: si ya eres una experta o experto en el lenguaje, te desafío a comentar cómo replicar este comportamiento con arrays u objetos y un solo condicional. 😏

**Solución con if (sin else ni else if):**
```js
const tipoDeSuscripcion = 'Basic';

if (tipoDeSuscripcion === 'Free') {
    console.log('Solo puedes tomar los cursos gratis');
}
if (tipoDeSuscripcion === 'Basic') {
    console.log('Puedes tomar casi todos los cursos de Platzi durante un mes');
}
if (tipoDeSuscripcion === 'Expert') {
    console.log('Puedes tomar casi todos los cursos de Platzi durante un año');
}
if (tipoDeSuscripcion === 'ExpertPlus') {
    console.log(
        'Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año'
    );
}
if (
    tipoDeSuscripcion !== 'Free' &&
    tipoDeSuscripcion !== 'Basic' &&
    tipoDeSuscripcion !== 'Expert' &&
    tipoDeSuscripcion !== 'ExpertPlus'
) {
    console.log('El tipo de suscripción ingresado no es valido');
}
```

**Solución del Bonus:**
```js
// No soy experto, así que no se que tal quedo, pero lo intente 😅

const tipoDeSuscripcion = 'Basic';

const suscripcion = [
    { type: 'Free', info: 'Solo puedes tomar los cursos gratis' },
    {
        type: 'Basic',
        info: 'Puedes tomar casi todos los cursos de Platzi durante un mes',
    },
    {
        type: 'Expert',
        info: 'Puedes tomar casi todos los cursos de Platzi durante un año',
    },
    {
        type: 'ExpertPlus',
        info: 'Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año',
    }
];

suscripcion.forEach(suscripcion => {
    if (suscripcion.type === tipoDeSuscripcion) {
        console.log(suscripcion.info);
    }
});
```


## Ciclos
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
- **¿Qué es un ciclo?**

    Es una estructura que hace que el código dentro se repita multiples veces, hasta que se cumpla una condición.

- **¿Qué tipos de ciclos existen en JavaScript?**

    Existen los ciclos while, for, for...in, for...of y do...while

- **¿Qué es un ciclo infinito y por qué es un problema?**

    Se denomina ciclo infinito, cuando un bucle no nunca cumple con su la condición para finalizar, esto genera un consumo de recursos muy alto y que se cuelgue el ordenador.

- **¿Puedo mezclar ciclos y condicionales?**

    Si, puede anidarse un ciclo en un condicional o viceversa, según lo amerite la situación.


### 2️⃣ Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

```js
for (let i = 0; i < 5; i++) {
    console.log("El valor de i es: " + i);
}

for (let i = 10; i >= 2; i--) {
    console.log("El valor de i es: " + i);
}
```

Solución:

```js
let i = 0;
while (i < 5) {
  console.log('El valor de i es: ' + i);
  i += 1;
}

i = 10;
while (i >= 2) {
  console.log('El valor de i es: ' + i);
  i -= 1;
}
```

### 3️⃣ Escribe un código en JavaScript que le pregunte a los usuarios cuánto es 2 + 2. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.
💡 Pista: puedes usar la función prompt de JavaScript.
```js
let x = true;
while (x) {
  let userInput = prompt('Hola! Te pregunto, ¿Cuánto es 2 + 2?');

  if (userInput == '4') {
    alert('¡Felicitaciones! has respondido correctamente');
    x = false;
  } else {
    alert('Al parecer algo fallo, ¡Intentemoslo otra vez!');
  }
}
```

## Listas
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
- **¿Qué es un array?**

    Un **array** es una variable que contiene una estructura de datos de diferentes valores, por ejemplo:

    ```js
    let array1 = [1, 2, 3, 4, 5];
    let array2 = ['Mandarina', 'Tomate', 'Pollo', 'Uña de T-Rex', 'Maíz'];
    let array3 = [
      { name: 'José Atonio', age: 23 },
      { name: 'Roberto Carlos', age: 19 },
      { name: 'Marco Aurelio', age: 27 }
    ];
    ```

- **¿Qué es un objeto?**

    Un **objeto** es una colección de datos, que se relacionan con un nombre y valor, como a continuación:

    ```js
    let object1 = { name: 'Michi', age: 2, type: 'Gato' };
    let object2 = { name: 'Zeus', age: 1, type: 'Canraio' };
    let object3 = { name: 'Loki', age: 3, type: 'Perro' };
    ```

- **¿Cuándo es mejor usar objetos o arrays?**

    Depende de la situación, los array los usaremos para agrupar datos y los objetos cuando necesitemos que los datos esten mejor relacionados, como esto:

    ```js
    let estudiante = {
        nombre: 'Carlos',
        apePaterno: 'Rojas',
        apeMaterno: 'Tapia',
        edad: 15,
        grado: '3ro',
        nivel: 'Secundaria'
    };
    ```

    Sin embargo, siempre podemos agrupar varios objetos dentro de un array como hice anteriormente en el ejemplo de arriba ☝️ (lo copiare y pegare mejor :3)

    ```js
    // ...
    let array3 = [
      { name: 'José Atonio', age: 23 },
      { name: 'Roberto Carlos', age: 19 },
      { name: 'Marco Aurelio', age: 27 }
    ];
    ```

- **¿Puedo mezclar arrays con objetos o incluso objetos con arrays?**

    Si, es perfectamente posible, tanto objetos en un array, como array con valor de las propiedades de un objeto.


### 2️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.

```js
let array = ["fs", 6, 8, 3, 'dsd'];

function firstElement(array) {
    console.log(array[0]);
}

firstElement(array);
```

### 3️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

```js
let array = [1,6,8,3,"dsd"];

function allElements(array) {
    array.forEach(element => console.log(element));
}

allElements(array);
```

### 4️⃣ Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).

```js
let estudiante = {
    nombre: 'Carlos',
    apePaterno: 'Rojas',
    apeMaterno: 'Tapia',
    edad: 15,
    grado: '3ro',
    nivel: 'Secundaria',
};

function allElements(object) {
    Object.entries(object).forEach(([key, value]) => {
        console.log(`•> ${key.toUpperCase()}: ${value}`);
    });
}

allElements(estudiante);
```

## ¿Cómo te fue? 🏆
**¡Felicidades por completar la prueba de JavaScript!** Confío en que hayas completado cada paso y hayas pausado para repasar los temas de los ejercicios que se te complicaron.

Ahora sí, continúa a la siguiente clase, pero recuerda que **ya no puedes abandonar el curso**, debes completarlo hasta el final. No importa cuánto tiempo te tome. **Yo sé que tú puedes. Y tú deberías de saberlo también.**

¡Te espero en la siguiente clase para comenzar!
