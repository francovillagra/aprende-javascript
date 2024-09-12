## Tipos de datos

Existen los datos:

- ### Primitivos:

  1. Number
  2. String
  3. Boolean
  4. Undefined
  5. Null

- ### De referencia:

  1. Array
  2. Object
  3. Functions
  4. Clases

La razón de la cual algunos datos se llaman primitivos y otros de referencia, es por lo siguiente:

- las variables se guardan en la memoria RAM de un ordenador, y éste, se puede representar como una tableta de chocolate, el sistema operativo, puede ser Mac, Linux, Windows, etc., se va a encargar de asignarle unas secciones a la memoria RAM.
  Supongamos que vamos a tomar una sección de la memoria RAM (1/4), esta seccion va a quedar completamente fija, no se va a poder modificar en el tiempo, es decir, toda la memoria que se le asignó no se va a poder expandir, a este tipo de memoria que no se puede expandir, y que además cumple con la caraterística de ser muy rapida se llama **STACK**, y acá se van a almacenar los tipos de `Datos Primitivos`. Por ejemplo, si yo tengo dentro de una variable el texto de **Hola Mundo**, y luego yo vaya a guardarlo en uno de esos bloques, y luego yo quiera revisar qué es lo que se encuentra dentro de esos bloques, voy a encontra el texto de **Hola Mundo**.
  Ahora vamos a hablar de otra memoria, llamada **Heap**. La característica, principal de esta memoria es que esta es dinámica, si por alguna razón quisieramos asignarle mas espacio a esta memoria, el sistema operativo se a encargar de hacerlo, asi que esta puede crecer de manera dinámica, a medida que necesite mas memoria, se le asigna más. En la memora **Heap** es donde se van a guardar todos los tipos de datos `De Referencia`. La memoria **Heap** es mas lenta que la memoraia **Stack**, por que tiene que cumplir con la característica de poder ser dinámica, esto quiere decir que puede crecer, o achicarse a medida que lo necesite. Además, los tipos `De Referencia`, se llaman de referencia, porque, si yo guardo un objeto, y éste lo guardo en un bloque, cuando yo vaya a ver el contenido de este bloque, no voy a encontrar el objeto, sino una dirección que podria perfectamente apuntar a otro bloque, es decir, no se encuentra el dato mismo, sino **una referencia**
