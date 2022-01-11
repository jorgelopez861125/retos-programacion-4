## ¿Qué es una variable y para qué sirve?
Es una forma de alamacenar un valor en la memoria RAM para poder reutilizarlas y calcularlas, etc.

## ¿Cuál es la diferencia entre declarar e inicializar una variable?
declarar: es dar nombre a la variable ej: `let numero`
inicializar: es **asignar** un valor a la variable ej: `numero = 1`

## ¿Cuál es la diferencia entre sumar números y concatenar strings?
-la suma se realiza unicamente con variables de tipo number
-la concatenacion se realiza uniendo string con otros valores

## ¿Qué operador me permite sumar o concatenar?
el operador suma: +

## Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

-Nombre `const nombre = 'jorge`
Apellido `const apellido = 'lopez`
Nombre de usuario `const username = 'jflopez'`
Edad `let edad = 36`
Correo electrónico `let email = 'fabricio861125@gmail.com`
Mayor de edad `let mayorEdad = true`
Dinero ahorrado `let ahorro = 20000.00`
Deudas `let deudas = 0`

## Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en un archivo nuevo.
`const persona = {
    nombre: 'jorge',
    apellido: 'lopez',
    username: 'jflopez',
    edad: 36,
    mail: 'fabricio861125@gmail.com'
    
}`

## Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

- Nombre completo (nombre y apellido)
`const nombreCompleto = persona.nombre + ' '+ persona.apellido`

- Dinero real (dinero ahorrado menos deudas)
`const patrimonio = persona.ahorro - persona.deudas`

## Funciones
## Responde las siguientes preguntas en un nuevo archivo:

## ¿Qué es una función?
-Es un conjunto de instrucciones agrupados en bloque de codigo

## ¿Cuándo me sirve usar una función en mi código?
- me sirve para dividir mis tareas en diferentes funciones que realizan una unica tarea

## ¿Cuál es la diferencia entre parámetros y argumentos de una función?
- parametros son cuando inicializamos la funcion 
- argumentos son cuando llamamos a la funcion

## Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:

`const name = "Juan David";
const lastname = "Castro Gallego";
const completeName = name + lastname;
const nickname = "juandc";

console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");`

`function presentacion (comopleteName, nickName) {
    const frase = `mi nombre es ${completeName}, pero prefiero que me digas ${nickName}.`
    return frase;
}
const res = presentacion(completeName, nickName);
console.log(res);
`

## Responde las siguientes preguntas en un nuevo archivo:

- ¿Qué es una condicional?
los condicionales es una forma de controlar el flujo de ejecuccion de mi codigo. por el lado verdadero y falso

- ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?
existen 4 tipos: if else, else if, switch y if ternario. Cuando tenemos varios if conviene usar swtich

¿Puedo combinar funciones y condicionales?
si

## Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:

const tipoDeSuscripcion = "Basic";

switch (tipoDeSuscripcion) {
   case "Free":
       console.log("Solo puedes tomar los cursos gratis");
       break;
   case "Basic":
       console.log("Puedes tomar casi todos los cursos durante un mes");
       break;
   case "Expert":
       console.log("Puedes tomar casi todos los cursos durante un año");
       break;
   case "ExpertPlus":
       console.log("Tú y alguien más pueden tomar TODOS los cursos durante un año");
       break;
}


`if (tipoDeSubscripcion === 'free'){
    console.log("Solo puedes tomar los cursos gratis");
} else if (tipoDeSubscripcion === 'free'){
}`
## Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).
`if (tipoDeSubscripcion === 'free') console.log("Solo puedes tomar los cursos gratis");`
`if (tipoDeSubscripcion === 'basic') console.log("Puedes tomar casi todos los cursos durante un mes"); `
`if (tipoDeSuscripcion === 'Expert') console.log("Puedes tomar casi todos los cursos durante un año"); `
`if (tipoDeSuscripcion === 'ExpertPlus') console.log("Tú y alguien más pueden tomar TODOS los cursos durante un año");`

## Bonus: si ya eres una experta o experto en el lenguaje, te desafío a comentar cómo replicar este comportamiento con arrays y un solo condicional. 
`const subs = ['free', 'basic', 'expert, expertPlus']`
`const mensaje = ['mensj1', mensj2, mensj3, mensj4]`
`const posicion = subs.indexOf(tipoDeSubscripcion)`

`if (pos !== -1){
    console.log()
}`

## Responde las siguientes preguntas en un nuevo archivo:
- ¿Qué es un ciclo?
son intrucciones dentro de un bucle, que se repiten o acciones que se repiten

- ¿Qué tipos de ciclos existen en JavaScript?
ciclos: for, while, do while

- ¿Qué es un ciclo infinito y por qué es un problema?
un ciclo infinito es cuando el bucle no tiene la condicion de salida del programa
por que si nunca termina la ram se termina

- ¿Puedo mezclar ciclos y condicionales?
si

## Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

for (let i = 0; i < 5; i++) {
    console.log("El valor de i es: " + i);
}
for (let i = 10; i >= 2; i--) {
    console.log("El valor de i es: " + i);
}

`let i = 0;
while (i < 5) {
 console.log("El valor de i es: " + i);
 i++;
}

let j = 10;
while (i >= 2) {
 console.log("El valor de i es: " + i);
 i--;
}
`

## Escribe un código en JavaScript que le pregunte a los usuarios cuánto es 2 + 2. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.

Pista: puedes usar la función prompt de JavaScript.
`let esIncorrecto = true;
while(incorrecto){
    const respuesta = promp('cuanto es 2 + 2 ?')
    if(respuesta == 4) {
        esIncorrecto = false;
        console.log('felicidades la respuesta es correcta')
    }
}`


## Responde las siguientes preguntas en un nuevo archivo:

- ¿Qué es un array?
Un array es una coleccion de datos 

¿Qué es un objeto?
es una colecccion de datos con clave y valor y constan de variables llamadas propiedades y funciones llamados metodos

¿Cuándo es mejor usar objetos o arrays?
Se puede usar arrays que contengan objetos como asi tambien objetos que contengan arrays

¿Puedo mezclar arrays con objetos o incluso objetos con arrays?
si se puede

- Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.

`const componentesPc = ['cpu', 'motherboard', 'ram', 'ssd'];
function firstElement(componentesPc){
    console.log(componentesPc[0];
}
firstElement(compoentesPc)`

- Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

`let cosas = ['vaso', 'pelota', 'trapo'];
function imprimir (cosas){ 
    cosas.forEach(nombre => {console.log(` ${nombre})`});
}
imprimir(cosas)`

- Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).

`const persona = {
    nombre: 'jorge',
    apellido: 'lopez',
    edad: 36
};
function descripcion(persona){
    let infoPersona.forEach((item) => {
        console.log(item)
    });

}
descripcion(persona);