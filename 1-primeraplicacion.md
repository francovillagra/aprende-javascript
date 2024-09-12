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
