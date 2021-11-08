# Introducción a la programación para el Diseño de interacción

### Trabajo final: Prototipo interactivo rápido

**Vamos a cambiar el nombre del `index.html` por `base.html`, para subir un nuevo `index.html` al mismo repositorio:**

| Nº  | Nombre         |   URL                                       |
|:---:|:---------------|:--------------------------------------------|
| 1 | Antonia Ascencio | https://antoniaascencio.github.io/clase-9-/ |
| 2 | Raúl Berríos |  https://raulgabrielb.github.io/sesion-9/ |
| 3 | Francisco Cabrera |  https://toomanypanchos.github.io/IDI_Sesion_09/ |
| 4 | Susan Castro | https://susancastroc.github.io/avance_01/ |
| 5 | Fernanda Celpa | https://fcelpa.github.io/ixd_sesion_09/ |
| 6 | Cristina Chamorro | https://cristinachr.github.io/ixd-sesion-09/ |
| 7 | Francisca Chong | https://mochuse.github.io/intro-progra-dis-int-09/ |
| 8 | Raúl Contreras | https://loveoken.github.io/interaccion-con-faco/CL_09/ |
| 9 | Rocío Córdova | https://rcio99.github.io/s09/ |
| 10 | Valentina Flores | https://thevalushca.github.io/ixd_sesion_9/ |
| 11 | Camila González | https://camilagonzalezga.github.io/Definicion-trabajo-final-/ |
| 12 | Tomás Hernández | https://tomashernandezmarti.github.io/clase-09/ |
| 13 | Andrea Jiménez | https://andreacjp.github.io/sesion_09/ |
| 14 | Bensu Karamustafa | — |
| 15 | Hisashi Kobayashi | https://h-kobaya.github.io/t1_s9/ |
| 16 | Claudia Mansilla | https://claudia2957.github.io/Definicion/ |
| 17 | Javiera Parga | https://javiparga13.github.io/sesion_09/ |
| 18 | María José Pinninghoff  | https://iamcoteg.github.io/ixd_sesion09/ |
| 19 | Camila Poblete | https://camilapoblete.github.io/sesion_09/ |
| 20 | Catalina Rivera | https://catari02.github.io/ejercicios-sesion-09/ |
| 21 | VanessaRodríguez |  https://vanessa-rodriguez123.github.io/Avance-trabajo-final-1/ |
| 22 | Roberto Aliro | https://robertred-a.github.io/ixd-sesion-09/ |
| 23 | Daniel Salas | https://dsalas1234.github.io/sesion_09/ |
| 24 | Kai Smith | https://lilk4i.github.io/ixd_sesion_09/ |
| 25 | Matias Vivanco | https://matiasvivancob.github.io/propuesta/ |

En este nuevo `index.html` deben comenzar a implementar su trabajo final. Se recomienda que aquellos trabajos agrupados como *blogs*, aprovechen los documentos en esta carpeta para enfocarse en la estructura de una "base de datos" antes que la estructura de cada página:

- https://profesorfaco.github.io/interaccion/sesion_10/blog.html
- https://profesorfaco.github.io/interaccion/sesion_10/blog_alternativo.html

¡Pero esos documentos tienen un problema! Sí. El problema es Google… 
- https://support.google.com/docs/thread/56845119/getting-new-cors-errors-on-querying-published-google-csv-sheet?hl=en
- https://forum.playcanvas.com/t/solved-cannot-get-cvs-google-spreadsheet-because-cors/1386
- https://issueexplorer.com/issue/mholt/PapaParse/809

Google, como "buen monopolio", cambia sus políticas según su conveniencia. Y lo más conveniente para Google es que se usen sólo sus herramientas, bajo sus condiciones; en este caso pasa algo como lo que sigue: *¡no me gusta nada eso de que anden usando drive como base de datos, así que les ofreceré mi API mientras bloqueo tal uso!*. 

La solución parche en `blog.html` es usar https://sheet.best/, a la que dejamos lidiar con las condiciones de Google bajo la condición de [pocas consultas si no pagamos por más](https://sheet.best/#pricing); la solución parche en `blog-alternativo.html` es usar https://cors-anywhere.herokuapp.com/corsdemo… un parche que tiene "muy poco pegamento". Habría más trucos. Pero la solución lenta y segura es exportar un nuevo CSV con cada actualización y dejarlo en un lugar donde no se cambien las reglas (como GitHub). 

- - - - - - - 

[← CLASE ANTERIOR](https://github.com/profesorfaco/interaccion/tree/main/sesion_09) — [SIGUIENTE CLASE →](https://github.com/profesorfaco/interaccion/tree/main/sesion_11)
