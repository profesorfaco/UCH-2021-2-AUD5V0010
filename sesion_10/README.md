# Introducción a la programación para el Diseño de interacción

### Trabajo final: Prototipo interactivo rápido

**Vamos a cambiar el nombre del `index.html` por `base.html`, para subir un nuevo `index.html` al mismo repositorio:**

| Nº  | Nombre         |   GitHub Page                               |   Repo GitHub                        |
|:---:|:---------------|:--------------------------------------------|:-------------------------------------|
| 1 | Antonia Ascencio | https://antoniaascencio.github.io/clase-9-/ | https://github.com/antoniaascencio/clase-9-/ |
| 2 | Raúl Berríos |  https://raulgabrielb.github.io/sesion-9/ | https://github.com/raulgabrielb/sesion-9/ |
| 3 | Francisco Cabrera | https://toomanypanchos.github.io/IDI_Sesion_09/ | https://github.com/toomanypanchos/IDI_Sesion_09/ |
| 4 | Susan Castro | https://susancastroc.github.io/avance_01/ | https://github.com/susancastroc/avance_01/ |
| 5 | Fernanda Celpa | https://fcelpa.github.io/ixd_sesion_09/ | https://github.com/fcelpa/ixd_sesion_09/ |
| 6 | Cristina Chamorro | https://cristinachr.github.io/ixd-sesion-09/ | https://github.com/cristinachr/ixd-sesion-09/ |
| 7 | Francisca Chong | https://mochuse.github.io/intro-progra-dis-int-09/ | https://github.com/mochuse/intro-progra-dis-int-09/ |
| 8 | Raúl Contreras | https://loveoken.github.io/interaccion-con-faco/CL_09/ | https://github.com/LoveOken/interaccion-con-faco/tree/main/CL_09 |
| 9 | Rocío Córdova | https://rcio99.github.io/s09/ | https://github.com/rcio99/s09/ | 
| 10 | Valentina Flores | https://thevalushca.github.io/ixd_sesion_9/ | https://github.com/thevalushca/ixd_sesion_9/ |
| 11 | Camila González | https://camilagonzalezga.github.io/Definicion-trabajo-final-/ | https://github.com/camilagonzalezga/Definicion-trabajo-final-/ |
| 12 | Tomás Hernández | https://tomashernandezmarti.github.io/clase-09/ | https://github.com/tomashernandezmarti/clase-09/ |
| 13 | Andrea Jiménez | https://andreacjp.github.io/sesion_09/ | https://github.com/andreacjp/sesion_09/ |
| 14 | Bensu Karamustafa | — | — |
| 15 | Hisashi Kobayashi | https://h-kobaya.github.io/t1_s9/ | https://github.com/h-kobaya/t1_s9/ |
| 16 | Claudia Mansilla | https://claudia2957.github.io/Definicion/ | https://github.com/claudia2957/Definicion/ |
| 17 | Javiera Parga | https://javiparga13.github.io/sesion_09/ | https://github.com/javiparga13/sesion_09/ |
| 18 | María José Pinninghoff  | https://iamcoteg.github.io/ixd_sesion09/ | https://github.com/iamcoteg/ixd_sesion09/ |
| 19 | Camila Poblete | https://camilapoblete.github.io/sesion_09/ | https://github.com/camilapoblete/sesion_09/ |
| 20 | Catalina Rivera | https://catari02.github.io/ejercicios-sesion-09/ | https://github.com/catari02/ejercicios-sesion-09/ |
| 21 | VanessaRodríguez | https://vanessa-rodriguez123.github.io/Avance-trabajo-final-1/ | https://github.com/vanessa-rodriguez123/Avance-trabajo-final-1/ |
| 22 | Roberto Aliro | https://robertred-a.github.io/ixd-sesion-09/ | https://github.com/robertred-a/ixd-sesion-09/ |
| 23 | Daniel Salas | https://dsalas1234.github.io/sesion_09/ | https://github.com/dsalas1234/sesion_09/ |
| 24 | Kai Smith | https://lilk4i.github.io/ixd_sesion_09/ | https://github.com/lilk4i/ixd_sesion_09/ |
| 25 | Matias Vivanco | https://matiasvivancob.github.io/propuesta/ | https://github.com/matiasvivancob/propuesta/ |

**En el mismo repositorio, con un nuevo `index.html`, deben comenzar a implementar su trabajo final**.

Se recomienda que aquellos trabajos agrupados como *blogs*, aprovechen los documentos en esta carpeta para enfocarse en la estructura de una "base de datos" para crear páginas: 

- https://profesorfaco.github.io/interaccion/sesion_10/blog.html
- https://profesorfaco.github.io/interaccion/sesion_10/blog_varias_paginas.html
- https://profesorfaco.github.io/interaccion/sesion_10/blog_alternativo.html

¡Pero esos documentos tienen un problema! Sí. El problema es Google… 
- https://support.google.com/docs/thread/56845119/getting-new-cors-errors-on-querying-published-google-csv-sheet?hl=en
- https://forum.playcanvas.com/t/solved-cannot-get-cvs-google-spreadsheet-because-cors/1386
- https://issueexplorer.com/issue/mholt/PapaParse/809

Google, como "buen monopolio", cambia sus políticas según su conveniencia. Y lo más conveniente para Google es que se usen sólo sus herramientas, bajo sus condiciones; en este caso pasa algo como lo que sigue: *¡no me gusta nada eso de que anden usando drive como base de datos, así que les ofreceré mi súper API mientras bloqueo tal uso!*. 

La solución parche en [`blog.html`](https://profesorfaco.github.io/interaccion/sesion_10/blog.html) es usar https://sheet.best/, a la que dejamos lidiar con las condiciones de Google a cambio de [muy pocas consultas si no pagamos por más](https://sheet.best/#pricing); la solución parche en [`blog-alternativo.html`](https://profesorfaco.github.io/interaccion/sesion_10/blog_alternativo.html) es usar https://cors-anywhere.herokuapp.com/corsdemo… un parche que tiene "muy poco pegamento". 

Hay más posibilidades, más allá de los parches: 

- La más simple y segura, pero lenta, es exportar un nuevo CSV con cada actualización de su Base de Datos, y reemplazar la versión anterior en línea (puede ser en GitHub).

- Aun más seguro, pero complejo y lento por el aprendizaje que exige, es decidirse a usar tecnologías tales como https://strapi.io/ u otras que necesitan de programación del lado del servidor. Esto último suma otra complicación: [*GitHub Pages does not support server-side languages such as PHP, Ruby, or Python.*](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages)

- - - - - - - 

[← CLASE ANTERIOR](https://github.com/profesorfaco/interaccion/tree/main/sesion_09) — [SIGUIENTE CLASE →](https://github.com/profesorfaco/interaccion/tree/main/sesion_11)
