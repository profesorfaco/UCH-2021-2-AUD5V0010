# Introducción a la programación para el Diseño de interacción

### Bootstrap v5 + jQuery

- - - - - - - - 

#### Lectura

En esta sesión pasaremos a otra biblioteca de JavaScript. Partimos por [p5.js](https://p5js.org/es/), una biblioteca que busca hacer que programar sea accesible e inclusivo para artistas, diseñadores, educadores, principiantes y cualquier otra persona. Ahora vamos a "un clásico": [jQuery](https://jquery.com/). 

**[jQuery](https://jquery.com/) es una biblioteca que por muchos años ha simplificado la redacción de instrucciones en JavaScript, sobre todo cuando se busca manipular el DOM y hacer transiciones animadas**. Su primera versión estable fue lanzada el año 2006, lo que es anterior a la primera revisión importante del [estándar de JavaScript](https://en.wikipedia.org/wiki/ECMAScript), la [ES5 del 2009](https://www.w3schools.com/js/js_es5.asp), con la que se comenzó a simplificar la redacción del mismo lenguaje.

Para entender la utilidad de [jQuery](https://jquery.com/), conviene partir con un ejemplo: En una página web tenemos varios elementos con una clase a la que denominamos `tal`. Para afectar a todos los elementos que tienen esa clase con un cambio de color desde JavaScript, sin usar bibliotecas, hace algunos años habríamos escrito la siguiente instrucción:

```
var elementos = Array.from(document.getElementsByClassName("tal"));
elementos.forEach(function(elemento){
  elemento.style.color="red";
});
```

Pero con el [estándar de JavaScript actual](https://www.w3schools.com/js/js_versions.asp) se simplifica un poco:

```
var elementos = document.querySelectorAll(".tal");
elementos.forEach(elemento => elemento.style.color="red");
```

Usando [jQuery](https://jquery.com/), por años ha sido suficiente escribir:

```
$(".tal").css("color","red");
```

Para la primera década del 2000, [jQuery](https://jquery.com/) ofrecía una simplificación radical en el trabajo con JavaScript. Pero ya en la segunda década, no conviene perder de vista al lenguaje original que ha evolucionado para ser más amigable en la medida que los desafíos de programación para la interacción se complejizan; por quedarnos "muy pegados" en [jQuery](https://jquery.com/), podríamos obligar a cada navegador a leer [90kb de código fuente](https://code.jquery.com/jquery-3.6.0.min.js) para interpretar una instrucción que ya se resuelve con menos de 1kb de puro JavaScript, o podríamos tener muchas dificultades dando el primer paso a una biblioteca de JavaScript actual, para construir interfaces de usuario ([Vue.js](https://v3.vuejs.org/) o [React.js](https://es.reactjs.org/)).

Hecha la advertencia, agreguemos un nivel más al ejemplo para poder entender el uso de la biblioteca: 

```
function enrojece() {
  $(".tal").css("color","red");
}
$("#cambio").on("click", enrojece);
```

Tal instrucción está abreviando, mediante [jQuery](https://jquery.com/), lo siguiente:

```
function enrojece(){
  var elementos = document.querySelectorAll(".tal");
  elementos.forEach(elemento => elemento.style.color="red");  
}
document.querySelector("#cambio").addEventListener("click", enrojece);
```

Con la última instrucción redactada, el cambio de color sobre todos los elementos de clase `tal` se hace al presionar el botón de identidad `cambio`. Y con este segundo ejemplo ya resulta evidente que la clave del uso de [jQuery](https://jquery.com/) está en la concatenación de un selector y una acción, antecedida de un signo peso: `$(selector).action()`. 

Las opciones de selectores y acciones son descritas detalladamente en https://api.jquery.com/, y de manera muy abreviada en https://htmlcheatsheet.com/jquery/

- - - - - - -

#### Exploración

Pendiente hasta el jueves 7.

- - - - - - -

#### Práctica

https://profesorfaco.github.io/interaccion/sesion_06/

- - - - - - - 


[← CLASE ANTERIOR](https://github.com/profesorfaco/interaccion/tree/main/sesion_05) — [SIGUIENTE CLASE →](https://github.com/profesorfaco/interaccion/tree/main/sesion_07)
