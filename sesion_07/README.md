# Introducción a la programación para el Diseño de interacción

### Bootstrap v5 + Charts.js

- - - - - - - - 

#### Lectura

**[Chart.js] es una biblioteca de JavaScript que nos permite implementar gráficos de manera sencilla**.

Con [Chart.js](https://www.chartjs.org/) podemos implementar gráficos de [línea](https://www.chartjs.org/docs/latest/charts/line.html), [barra](https://www.chartjs.org/docs/latest/charts/bar.html), [radar](https://www.chartjs.org/docs/latest/charts/radar.html), [torta](https://www.chartjs.org/docs/latest/charts/doughnut.html), [área polar](https://www.chartjs.org/docs/latest/charts/polar.html), [burbujas](https://www.chartjs.org/docs/latest/charts/bubble.html) y [dispersión](https://www.chartjs.org/docs/latest/charts/scatter.html), que son los tipos de gráficos disponibles en otra biblioteca de JavaScript:

**[Chart.js](https://www.chartjs.org/) nos permite implementar gráficos con valores numéricos contenidos en arreglos de JavaScript, y su promesa, en inglés, es *Simple yet flexible JavaScript charting for designers & developers*. Al ubicarse en ese lugar intermedio puede provocar dolores de cabeza en los extremos caricaturizados: muy complejo para *designers* o muy simple para *developers*.** 

Para evitar dolores de cabeza, corresponde reconocer sus partes: 

```
var contexto = document.getElementById('nombre').getContext('2d');
var configuracion = {type: '…', data: {…}, options: {…}}
var chart = new Chart(contexto, configuracion);
```

1. Requiere la creación del contexto 
2. Requiere la configuración de tipo, datos y opciones para el gráfico 
3. Contexto y configuración permiten indicar que en este script vamos a crear un `new Chart()`.

Nos referimos a tres partes. No se trata de tres pasos. También sería válido escribir:

```
new Chart(document.getElementById('nombre').getContext('2d'), {type: '…', data: {…}, options: {…}});
```

Antes de partir la exploración necesaria para hacer la configuración de [Chart.js](https://www.chartjs.org/docs/latest/charts/?h=type), corresponde:

- recordar el [método `forEach()`](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Objetos_globales/Array/forEach);

- revisar el [método `push()`](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Objetos_globales/Array/push); y

- tener a mano la [documentación de Charts.js](https://www.chartjs.org/docs/latest/).

Es necesario contar con un editor de código fuente; vamos a crear un documento nuevo, pegar el código que sigue y guardarlo con el nombre ejemplo.html:

```
<!DOCTYPE html>
<html lang="es">
    <head>
        <title>Esto es un ejemplo</title>
        <script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.9.4/Chart.min.js" integrity="sha512-d9xgZrVZpmmQlfonhQUvTR7lMPtO7NkZMkA0ABN3PHCbKA5nqylQ/yWlFAyY6hYgdF1Qh6nYiuADWwKB4C2WSw==" crossorigin="anonymous"></script>
    </head>
    <body>
        <canvas id="myChart"></canvas>
        <script>
            //comunas más pobladas en la provincia de Santiago
            var santiago = [
                { comuna: "La Florida", habitante: 366.916, color: "#d32f2f" },
                { comuna: "Las Condes", habitante: 294.838, color: "#7b1fa2" },
                { comuna: "Maipú", habitante: 521.627, color: "#303f9f" },
                { comuna: "Peñalolén", habitante: 241.599, color: "#0288d1" },
                { comuna: "Santiago", habitante: 404.495, color: "#00796b" },
            ];

            var lasComunas = [];
            var losHabitantes = [];
            var losColores = [];

            santiago.forEach(function (dato) {
                lasComunas.push(dato.comuna);
                losHabitantes.push(dato.habitante);
                losColores.push(dato.color);
            });

            new Chart(document.getElementById("myChart").getContext("2d"), {
                type: "bar",
                data: {
                    labels: lasComunas,
                    datasets: [
                        {
                            data: losHabitantes,
                            backgroundColor: losColores,
                        },
                    ],
                },
                options: {},
            });
        </script>
    </body>
</html>
```

- - - - - - - 

[← CLASE ANTERIOR](https://github.com/profesorfaco/interaccion/tree/main/sesion_06) — [SIGUIENTE CLASE →](https://github.com/profesorfaco/interaccion/tree/main/sesion_08)
