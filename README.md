# Test de JavaScript
## Instrucciones para tomar esta prueba
- Evalúa muy críticamente tu conocimiento.
- Si logras resolver la prueba, no importa cuánto te cueste, puedo asegurarte que tienes todo para continuar a las siguientes clases y tomar el resto del curso.
- Si no lo logras, no te preocupes, absolutamente nadie puede juzgarte, solo tú. Vuelve al [Curso Básico de JavaScript](https://platzi.com/cursos/basico-javascript/), anota los temas clave donde puedes mejorar, ubica las clases donde puedes aprenderlos y estudia vigorosamente.
- Es completamente válido hacer búsquedas en Google, cursos y tutoriales de Platzi, incluso usar tu cuaderno de notas sin importar si es físico o virtual.

Recuerda que el éxito no se mide por cuánto tiempo te toma aprender, esa métrica es relativamente inútil. Mejor concéntrate en completar los cursos de tu ruta de aprendizaje profesional y desarrollar los proyectos que realmente demuestran que dominas cada tecnología.

¡Mucha suerte!

## Variables y operaciones
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
- ¿Qué es una variable y para qué sirve?

    Una variable es un valor que ocupa un espacio en memoria, este valor tiene un tipo de dato (String, Number, Bolean, etc.), podemos usarla para llamar ese valor cuando sea necesario, pero donde podrá ser llamada, depende del alcance (Scope) que tenga. Las variables se definen con las palabras reservadas _var_, _let_ y _const_, sin embargo, debemos tener cuidado con el tipo de dato, porque JavaScript es un lenguaje dinámico y está sujeto a la coerción.

- ¿Cuál es la diferencia entre declarar e inicializar una variable?
  
    Cuando declaramos una variable, solo le asignando un espacio en memoria, pero al inicializarla se da un valor y declarara el tipo de dato automáticamente; en caso de no inicializarla, se le asignara el valor undefined.
  
- ¿Cuál es la diferencia entre sumar números y concatenar strings?

    Al sumar datos numéricos estamos haciendo una operación matemática donde obtenemos un resultado según los valores ingresados, mientras que al concatenar strings, estamos uniendo los textos.

- ¿Cuál operador me permite sumar o concatenar?

    

### 2️⃣ Determina el nombre y tipo de dato para almacenar en variables la siguiente información:
- Nombre
- Apellido
- Nombre de usuario en Platzi
- Edad
- Correo electrónico
- Mayor de edad
- Dinero ahorrado
- Deudas

### 3️⃣ Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en los comentarios.

### 4️⃣ Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:
- Nombre completo (nombre y apellido)
- Dinero real (dinero ahorrado menos deudas)

## Funciones
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
- ¿Qué es una función?
- ¿Cuándo me sirve usar una función en mi código?
- ¿Cuál es la diferencia entre parámetros y argumentos de una función?

### 2️⃣ Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:
```js
const name = "Juan David";
const lastname = "Castro Gallego";
const completeName = name + lastname;
const nickname = "juandc";}

console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");
```
## Condicionales
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
- ¿Qué es un condicional?
- ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?
- ¿Puedo combinar funciones y condicionales?

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

### 3️⃣ Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).
💡 Bonus: si ya eres una experta o experto en el lenguaje, te desafío a comentar cómo replicar este comportamiento con arrays u objetos y un solo condicional. 😏

## Ciclos
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
- ¿Qué es un ciclo?
- ¿Qué tipos de ciclos existen en JavaScript?
- ¿Qué es un ciclo infinito y por qué es un problema?
- ¿Puedo mezclar ciclos y condicionales?

### 2️⃣ Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:
```js
for (let i = 0; i < 5; i++) {
    console.log("El valor de i es: " + i);
}

for (let i = 10; i >= 2; i--) {
    console.log("El valor de i es: " + i);
}
```

### 3️⃣ Escribe un código en JavaScript que le pregunte a los usuarios cuánto es 2 + 2. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.
💡 Pista: puedes usar la función prompt de JavaScript.


## Listas
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
¿Qué es un array?
¿Qué es un objeto?
¿Cuándo es mejor usar objetos o arrays?
¿Puedo mezclar arrays con objetos o incluso objetos con arrays?

### 2️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.

### 3️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

### 4️⃣ Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).

## ¿Cómo te fue? 🏆
**¡Felicidades por completar la prueba de JavaScript! ** Confío en que hayas completado cada paso y hayas pausado para repasar los temas de los ejercicios que se te complicaron.

Ahora sí, continúa a la siguiente clase, pero recuerda que **ya no puedes abandonar el curso**, debes completarlo hasta el final. No importa cuánto tiempo te tome. **Yo sé que tú puedes. Y tú deberías de saberlo también.**

¡Te espero en la siguiente clase para comenzar!