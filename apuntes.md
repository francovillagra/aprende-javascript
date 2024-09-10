- ## Preparando ambiente de trabajo:

1.  #### Descargamos [VisualStudioCode](https://code.visualstudio.com/ "Visual Studio Code")
2.  #### Descargamos [NodeJS](https://nodejs.org/en "Node JS")

3.  Creamos una carpeta en el directorio, en este caso le colocamos "Ultimate JS". Arrastramos la carpeta hacia visual studio para empezar a trabajar.
4.  En el Visual Studio pinchamos en "Nuevo Archivo", y vamos a darle el nombre de index.html.
5.  En visual studio escribimos el siguiente código:

    - ! (simbolo de exclamación), y automaticamente va a aparecer una opción que dice: Emmet Abbreviat...> y mas abajo nos va a sugerir otra opcion con tres simbolos de exclamación: !!!
    - Seleccionamos la primera opción, y automaticamente, nos va a aparecer nuestro esqueleto de trabajo, que se va a ver de la siguinte manera:

```javascript
<!DOCTYPE html>
<html lang="eng">
<head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Ultimate JS</title>
</head>
<body>
      Hola Mundo
</body>
</html>
```

6. Editamos el título de nuestro código, y le vamos a poner "Ultimate JS"
7. En el cuerpo o "body", escribimos Hola Mundo.
8. Luego instalamos una extensión de Vs Code llamada 'live server' por Ritwick Dey.
9. Luego de la instalación, podemos pinchar en nuestro index.html y seleccionar "open with live server", y eso nos deberia direccionar a una URL muy parecida a esto: 12.0.0.1:5500/index.html. Pero lo que a nosotros nos interesa es que aparezca el texto 'Hola Mundo'.
   Esto quiere decir que nuestro ambiente ha sido configurado con éxito.

- ## Primera aplicación

Para que podamos utilizar código javascript dentro de nuestras aplicaciones, tenemos que utilizar la etiqueta de script en html.
Debajo de nuestro texto de 'Hola Mundo', y agregamos nuestra etiqueta de script de la siguiente manera:

```javascript
 <!DOCTYPE html>
 <html lang="eng">
 <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Ultimate JS</title>
 </head>
 <body>
       Hola Mundo
       <script>
            console.log('Hola Mundo');
       </script>
 </body>
 </html>
```

El código que vamos a escribir entre el script es _console.log('Hola Mundo')_;

Cada vez que nosotros ejecutamos una página web desde cualquier movil, o computador, los exploradores web, lo que van a hacer es que van a tomar el código que se escribió desde arriba hacia abajo, y este va a ser descargado, tal cual descargas un archivo de internet, va a ser exactamente lo mismo. Entonces, dado esto, si nosotros hacemos una aplicación, cuyo código de JavaScript es muy gerande (que, es lo mas probable que ocurra), las aplicaciones reales no cuentan con una línea, cuentan con el orden de cientos de miles de líneas de código, en ese caso, si nosotros colocamos nuestro código de JavaScript al comienzo dentro de la etiqueta de <Head>, lo que va a ocurrir, es que los usuarios cuando lleguen al sitio web, van a ver una pagina en blanco por que el explorador va a estar constantemente descargando ese código de JavaScript, para luego interpretarlo, y despues de eso, va a estar descargando el resto del contenido de la página, que es donde se encuentra el texto, imágenes que se coloquen, etc.
Entonces, si hacemos eso, le vamos a dar una mala experiencia a los usuarios, es por eso que ponemos las etiquetas de script al final de nuestro codigo.
Sin embargo, existen excepciones, van a existir algunas librerias o blibiotecas que querramos usar dentro de aplicaciones escritas en javascript, que nos van a indicar que tenemos que colocar las etiquetas de script dentro de las etiquetas HEAD. ESTO ES UNA EXCEPCION.

- ## Referenciando archivos

Cuando estamos construyendo una app, no vamos a escribir una sola línea de código, vamos a escribir muchas líneas de código, entonces, que nosotros pongamos todo el código en las etiquetas de script, no va a ser lo mejor.
Vamos a tomar el código que tenemos en las etiquetas de script: **console.log(nombre)** , vamos a cortar, guardamos, creamos otro archivo llamado **app.js**, y ahí pegamos el código que previamente se cortó.
Nos volvemos a index.html, y en las etiquetas de script, lo que tenemos que hacer es referenciar ese archivo llamado **app.js** que nosotros creamos, dentro de esta etiqueta de script, esto lo que hará sera ejecutar el código que se encuentra dentro de este archivo tal cual como si nosotros lo hubiesemos escrito dentro de estas dos etiquetas, asi que eliminamos el espacio, y luego dentro del script, hacemos un espacio de esta manera:

`<script ></script>`

Luego, nuestro código deberia quedarnos de esta manera:

`<script src="app.js"></script>`

Para verificar los cambios, nos volvemos al navegador haciendo click derecho en visual studio (Open with live server) - Nuestra aplicacion acaba de ser refactorizada por completo.

- ## Refactorizar

Vamos a suponer que nosotros tenemos nuestra aplicación dentro de un servidor, y se encuentra almacenado en la nube, luego tenemos un usuario que esta tratando de acceder a la aplicación, él realiza peticiones y el servidor le devuelve con éxito, sin embargo, nuestra aplicación empieza a crecer y estas se empieza a volver más lenta, entonces su rendimiento empieza a bajar. Lo que nosotros queremos hacer es cambiar el código que esta escrito pero sin afectar los usuarios que estan utilizando nuestra aplicación, que no se den cuenta absolutamente nada. Lo que tenemos que hacer es cambiar la estructura interna, sin alterar el comportamiento externo, a esto se le conoce como **REFACTORIZAR**, basicamente significa hacer el código más legible, agradable y con mejor rendimiento.

`<script src="app.js"></script>`

Debido a esto mismo, a que cambiamos el código, pero seguimos obteniendo el mismo resultado, es que nuestra refactorización fue un éxito.

- ## Variables

Una variable es una (caja) que va a tener información, la cual vamos a poder referenciar en un futuro, esta sería la forma lógica de pensarlo.
Ahora paso a explicar como funcionan:

- Cada dispositivo tiene una memoria RAM (random access memory)
- (Siguiendo con el concepto de la caja) Tenemos un objeto a la que le vamos a poner la etiqueta de NOMBRE, y esta va a contener el texto de 'Hola Mundo', y esta (caja) lo vamos a almacenar en el bloque de la memoria.
- Luego, en el futuro, cuando nosotros queramos saber cual es el valor que se encontraba dentro de ese bloque, de la memoria RAM, en lugar de ir a buscarlo a la memoria RAM, lo que vamos a hacer es escribir NOMBRE, que es como se llama la caja, y dentro de esta, se va a encontrar con la información 'Hola Mundo'.
- Ahora nos vamos al caso práctico:

1. Creamos un nuevo directorio (New folder) y el nombre que va a llevar será: 01-tipos.
2. Dentro de esa carpeta creamos un nuevo archivo (New file) y el nombre que va a llevar será: 01-variables.js.
3. Nos vamos a index.html, y en nuestro código, donde dice "app.js", es decir:

   `<script src="app.js"></script>`

4. Reemplazaremos "app.js" por el nombre de la carpeta y, el archivo dentro de la carpeta, que queremos referenciar, en este caso se vería de esta forma: "01-tipos/01-variables.js".
5. Nos vamos ahora a nuestro archivo "01-variables.js", y acá escribimos lo siguiente:

   `let`

**Referencia**: Let es una palabra reservada que nos permite definir variables.

6. Luego indicamos el nombre de la variable:

`let nombre = "Hola Mundo"; `

7. Debajo escribimos lo siguiente:

`console.log(nombre);`

8. Guardamos y nos vamos a nuestro navegador con nuestro atajo (Open with live server)

- ## Reglas para nombrar variables

Existen reglas para crear variables, algunas son prácticas de la industria, y otras que el lenguaje mismo no nos va a dejar realizar, por ejemplo, si nosotros queremos crear una variable, esta debe comenzar con letras, o tambien puede comenzar con un guión bajo.

1. Si nosotros quisiera comenzar una variable con numeros, javascript no nos va a dejar, y no solamente eso, visual studio nos va a empezar a mostrar errores.
2. Las variables no pueden ser nombradas al igual que palabras reservadas, por ejemplo, la primera palabra reservada es **LET**, entoncesn o se puede definir una palabra que se llame **LET**.
3. Cuando nosotros estamos creando variables, nosotros podemos seguir tres convenciones:

   - UpperCamelCase
   - camelCase
   - snake_case

   a) UpperCamelCase significa que, cuando nosotros creemos una variable, la primera letra de cada palabra que nosotros utilicemos para nombrar esa variable, tiene que ser mayúscula, y si existe otra palabra dentro de esa misma variable, también va tener que contener una mayúscula, y así también si existiese otra palabra.

   b) camelCase, por el contrario, nos exige que cada palabra empiece con mayúscula, sin embargo la primera palabra NO.

   c) Luego tenemos snake_case, la cual nos indica que cada palabra debe estar separada por un guión bajo.

4. Ahora creamos ejemplo de variables utilizando las convenciones:

- #### UpperCamelCase:

`let NombreCompleto;`

Esta convención se utiliza por lo general en algunos lenguajes para nombrar constantes.

- #### camelCase:

`let nombreCompleto;`

**Nota:** Javascript es "case sensitive", esto quiere decir que si nosotros utilizamos mayúsculas o minúsculas, e incluso indicandole exactamente el mismo texto, Javascript va a entender que son dos variables completamente distintas, por eso si nosotros en "NombreCompleto":

`let NombreCompleto;` <-- Chanchito

le asignamos el nombre Chanchito, y la siguiente variable:

`let nombreCompleto;` <-- Felipe

le asignamos el nombre "Felipe", dependiendo del valor que nosotros queramos, es el nombre de la variable que nosotso vamos a colocar, dentro de console.log(nombre) <---.
Entonces NO es los mismo, si yo coloco nombreCompleto, a poner NombreCompleto.
La tercera convención que vamos a ver es la de snake_case, que debería escribirse de la siguiente manera:

`let nombre_completo;`

La convención que mas se suele utilizar en Javascript es **camelCase**

Ademas de definir una variable y asginarle un valor, lo que podemos hacer cuando estamos cuando las estamos definiendo con **LET**
