# Introducción a la programación para el Diseño de interacción

### Trabajo final: Prototipo interactivo rápido

**Vamos a cambiar el nombre del `index.html` por `base.html`, para subir un nuevo `index.html` al mismo repositorio:**

| Nº  | Nombre           | /index.html                                        |  /page.html                                            |
|:---:|:-----------------|:---------------------------------------------------|:-------------------------------------------------------|
| 1 | [Antonia Ascencio](https://github.com/antoniaascencio/) | https://antoniaascencio.github.io/clase-9-/        | https://antoniaascencio.github.io/clase-9-/base.html   |
| 2 | [Raúl Berríos](https://github.com/raulgabrielb/)  | https://raulgabrielb.github.io/sesion-9/           | —                                                      |        
| 3 | [Francisco Cabrera](https://github.com/toomanypanchos/)  | —                               | —                                  |
| 4 | [Susan Castro](https://github.com/susancastroc/)    | https://susancastroc.github.io/avance_01/          | —                                                 |
| 5 | [Fernanda Celpa](https://github.com/fcelpa/)          | https://fcelpa.github.io/ixd_sesion_09/            | https://fcelpa.github.io/ixd_sesion_09/base.html       |
| 6 | [Cristina Chamorro](https://github.com/cristinachr)      | https://cristinachr.github.io/ixd-sesion-09/       | https://cristinachr.github.io/ixd-sesion-09/base.html  |
| 7 | [Francisca Chong](https://github.com/mochuse/)         | https://mochuse.github.io/intro-progra-dis-int-09/ | https://mochuse.github.io/intro-progra-dis-int-09/base.html |
| 8 | [Raúl Contreras](https://github.com/LoveOken/interaccion-con-faco/) | https://loveoken.github.io/interaccion-con-faco/CL_09/ | https://loveoken.github.io/interaccion-con-faco/CL_09/base.html |
| 9 | [Rocío Córdova](https://github.com/rcio99/) | https://rcio99.github.io/s10/ | — |
| 10 | [Valentina Flores](https://github.com/thevalushca/) | https://thevalushca.github.io/Avance_11-11/ | — |
| 11 | [Camila González](https://github.com/camilagonzalezga/) | — | — |
| 12 | [Tomás Hernández](https://github.com/tomashernandezmarti/) | https://tomashernandezmarti.github.io/clase-09/ | https://tomashernandezmarti.github.io/clase-09/base.html |
| 13 | [Andrea Jiménez](https://github.com/andreacjp/) | https://andreacjp.github.io/sesion_09/ | https://andreacjp.github.io/sesion_09/base.html |
| 14 | Bensu Karamustafa | — | — |
| 15 | [Hisashi Kobayashi](https://github.com/h-kobaya/) | https://h-kobaya.github.io/t1_s9/ | https://h-kobaya.github.io/t1_s9/base.html |
| 16 | [Claudia Mansilla](https://github.com/claudia2957/) | — | — |
| 17 | [Javiera Parga](https://github.com/javiparga13/) | — | — |
| 18 | [María José Pinninghoff](https://github.com/iamcoteg/) | — | — |
| 19 | [Camila Poblete](https://github.com/camilapoblete/) | — | — | 
| 20 | [Catalina Rivera](https://github.com/catari02/) | https://catari02.github.io/trabajo-final/ | – |
| 21 | [VanessaRodríguez](https://github.com/vanessa-rodriguez123/) | https://vanessa-rodriguez123.github.io/trabajo-final-1/ | https://vanessa-rodriguez123.github.io/trabajo-final-1/base.html |
| 22 | [Roberto Aliro](https://github.com/robertred-a/) | https://robertred-a.github.io/ixd-sesion-09/ | https://robertred-a.github.io/ixd-sesion-09/base.html |
| 23 | [Daniel Salas](https://github.com/dsalas1234/) | https://dsalas1234.github.io/sesion_09/ | https://dsalas1234.github.io/sesion_09/base.html |
| 24 | [Kai Smith](https://github.com/lilk4i/) | https://lilk4i.github.io/ixd_Trabajo-final/ | — |
| 25 | [Matias Vivanco](https://github.com/matiasvivancob/) | — | — |

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
