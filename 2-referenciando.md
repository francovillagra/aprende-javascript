- ## Referenciando archivos

Cuando estamos construyendo una app, no vamos a escribir una sola línea de código, vamos a escribir muchas líneas de código, entonces, que nosotros pongamos todo el código en las etiquetas de script, no va a ser lo mejor.
Vamos a tomar el código que tenemos en las etiquetas de script: **console.log(nombre)** , vamos a cortar, guardamos, creamos otro archivo llamado **app.js**, y ahí pegamos el código que previamente se cortó.
Nos volvemos a index.html, y en las etiquetas de script, lo que tenemos que hacer es referenciar ese archivo llamado **app.js** que nosotros creamos, dentro de esta etiqueta de script, esto lo que hará sera ejecutar el código que se encuentra dentro de este archivo tal cual como si nosotros lo hubiesemos escrito dentro de estas dos etiquetas, asi que eliminamos el espacio, y luego dentro del script, hacemos un espacio de esta manera:

`<script ></script>`

Luego, nuestro código deberia quedarnos de esta manera:

`<script src="app.js"></script>`

Para verificar los cambios, nos volvemos al navegador haciendo click derecho en visual studio (Open with live server) - Nuestra aplicacion acaba de ser refactorizada por completo.
