# Introducción a la programación para el Diseño de interacción

# Bootstrap

### Lectura

**Existen marcos de trabajo de código abierto que nos pueden ayudar a avanzar más rápido desde relaciones predefinidas de HTML y CSS**. Por su popularidad, corresponde mencionar a:

- [Bootstrap](https://getbootstrap.com/): *The world’s most popular front-end open source toolkit, featuring Sass variables and mixins, responsive grid system, extensive prebuilt components, and powerful JavaScript plugins.*

- [Foundations](https://get.foundation/): *The most advanced responsive front-end framework in the world* 

- [Semantic UI](https://semantic-ui.com/): *A development framework that helps create beautiful, responsive layouts using human-friendly HTML*

Nos quedaremos con el primero de los mencionados, en su versión más reciente, la 5.1. 

[Bootstrap](https://getbootstrap.com/) nos permite implementar tanto prototipos rápidos como productos acabados, esto mediante el uso de Elementos de HTML5 relacionados con [reglas de CSS3 predefinidas](https://cdn.jsdelivr.net/npm/bootstrap@5.1.1/dist/css/bootstrap.css) con [Sass](https://sass-lang.com/) ([Less](http://lesscss.org/) en versiones de Boostrap anteriores a la 4), además de Javascript simplificado por una biblioteca (que debe complementarse con [jQuery](https://jquery.com/) en versiones de Bootstrap anteriores a la 5).

Hay distintas maneras de comenzar a trabajar con Boostrap. Nosotros vamos a partir con una adaptación de la [Starter template](https://getbootstrap.com/docs/5.1/getting-started/introduction/#starter-template), con un documento HTML que debe verse así: 

```
<!doctype html>
<html lang="es">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-F3w7mX95PdgyTmZZMECAngseQB83DfGTowi0iMjiWaeVhAn4FJkqJByhZMI3AhiU" crossorigin="anonymous">
    <title>Hello, world!</title>
  </head>
  <body>
    <h1>Hello, world!</h1>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.1/dist/js/bootstrap.bundle.min.js" integrity="sha384-/bQdsTh/da6pkI1MST/rWKFNjaCP5gBSY4sEBT38Q/9RBh9AH40zEOg7Hlq2THRZ" crossorigin="anonymous"></script>
  </body>
</html>
```

En el cuerpo de tal documento HTML (`<body></body>`) podemos comenzar a utilizar las clases del CSS de Bootstrap, que nos permiten tomar de 1 a 12 columnas (`class="col"`) en cada fila (`class="row"`) que esté dentro de un contenedor (`class="container"`). 

- - - - - - 

### Exploración

Antes de continuar, es recomendable revisar:

- Containers → https://getbootstrap.com/docs/5.1/layout/containers/
- Grid system → https://getbootstrap.com/docs/5.1/layout/grid/
- Columns → https://getbootstrap.com/docs/5.1/layout/columns/
- Gutters → https://getbootstrap.com/docs/5.1/layout/gutters/

- - - - - - - 

#### Práctica

https://profesorfaco.github.io/interaccion/sesion_04/

- - - - - - - 

###### [← CLASE ANTERIOR](https://github.com/profesorfaco/interaccion/tree/main/sesion_03) — [SIGUIENTE CLASE →](https://github.com/profesorfaco/interaccion/tree/main/sesion_05)
