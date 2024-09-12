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
