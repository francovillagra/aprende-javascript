- ## Reglas para nombrar variables

Existen reglas para crear variables, algunas son prácticas de la industria, y otras que el lenguaje mismo no nos va a dejar realizar, por ejemplo, si nosotros queremos crear una variable, esta debe comenzar con letras, o tambien puede comenzar con un guión bajo.

1. Si nosotros quisiera comenzar una variable con numeros, javascript no nos va a dejar, y no solamente eso, visual studio nos va a empezar a mostrar errores.
2. Las variables no pueden ser nombradas al igual que palabras reservadas, por ejemplo, la primera palabra reservada es **LET**, entoncesn o se puede definir una palabra que se llame **LET**.
3. Cuando nosotros estamos creando variables, nosotros podemos seguir tres convenciones:

```
   - UpperCamelCase
   - camelCase
   - snake_case
```

a) UpperCamelCase significa que, cuando nosotros creemos una variable, la primera letra de cada palabra que nosotros utilicemos para nombrar esa variable, tiene que ser mayúscula, y si existe otra palabra dentro de esa misma variable, también va tener que contener una mayúscula, y así también si existiese otra palabra.

b) camelCase, por el contrario, nos exige que cada palabra empiece con mayúscula, sin embargo la primera palabra NO.

c) Luego tenemos snake_case, la cual nos indica que cada palabra debe estar separada por un guión bajo.

4. Ahora creamos ejemplo de variables utilizando las convenciones:

- #### UpperCamelCase:

```javascript
let NombreCompleto;
```

Esta convención se utiliza por lo general en algunos lenguajes para nombrar constantes.

- #### camelCase:

```javascript
let nombreCompleto;
```

**Nota:** Javascript es "case sensitive", esto quiere decir que si nosotros utilizamos mayúsculas o minúsculas, e incluso indicandole exactamente el mismo texto, Javascript va a entender que son dos variables completamente distintas, por eso si nosotros en "NombreCompleto":

```javascript
let NombreCompleto; <-- Chanchito
```

Le asignamos el nombre Chanchito, y la siguiente variable:

```javascript
let nombreCompleto; <-- Felipe
```

le asignamos el nombre "Felipe", dependiendo del valor que nosotros queramos, es el nombre de la variable que nosotso vamos a colocar, dentro de console.log(nombre) <---.
Entonces NO es los mismo, si yo coloco nombreCompleto, a poner NombreCompleto.

La tercera convención que vamos a ver es la de snake_case, que debería escribirse de la siguiente manera:

```javascript
let nombre_completo;
```

La convención que mas se suele utilizar en Javascript es **camelCase**

Ademas de definir una variable y asginarle un valor, lo que podemos hacer cuando estamos cuando las estamos definiendo con **LET**
es indicarle, por ejemplo, ningun valor, solamente la declaramos, pero luego en un futuro podemos asignarle valor:

```javascript
let apellido;

apellido = "Villagra";
```

Pero cuando hagamos eso, no tenemos que utilizar la palabra reservada de **LET**, LET solamente se utiliza para indicarle a Javascript que vamos a crear una variable, esta podría tener o no tener un valor, y luego, cuando nosotros quisieramos asignarle un valor, siempre y cuando esta ya se encuentre creada, debemos colocarle la palabra reservada de LET, basta con que solo coloquemos el nombre de la variable.
Ademas, podriamos definir más de una variable en la misma línea:

```javascript
let apellido, animal;
apellido = "Villagra";
```

Nos fijamos que no es necesario utiliza la palabra **LET**, que se entiende que la variable se encuentra separada por una coma, lo cual significa que la palabra que se encuentra luego de la coma tambien se encuentra inicializada. Sin embargo, la práctica que se utiliza hoy en día es, crear la variable en una línea independiente, de esta forma:

```javascript
let apellido;
let animal;
```

NOTA: Cuando vayamos a crear una variable, es importante indicar el valor que vaya a tener.
