# Cómo contribuir con la web de Python España

Existen muchas formas de contribuir con [Python España](http://es.python.org). Escribir contenido para la página web, mantener la información contenida actualizada, [detectar problemas](https://github.com/python-spain/web/issues/new) o corregirlos son formas efectivas de mejorar la comunidad.

Recuerda que, tanto contribuir a este repositorio como administrarlo, supone la aceptación de nuestro [código de conducta](https://github.com/python-spain/web/blob/master/CODE_OF_CONDUCT.md#code-of-conduct).

## Informando de un problema

La forma más sencilla de contribuir con la página web es informar de un error detectado. Introduce un título corto y, en el espacio para comentarios, indica la dirección web donde detectaste el problema, y añade una pequeña descripción del mismo. Recuerda que puedes **añadir imágenes**, como capturas de pantalla, arrastrando la imagen sobre el editor. Por ejemplo:

```
Dónde pone "title": Hay muy poco espacio entre títulos y contenido
Dónde pone "leave a comment":
En la sección "¡hazte socio!": https://es.python.org/pages/hazte-socio.html
Hay muy poco espacio entre los títulos grandes y los subtítulos o contenido
y esto dificulta la lectura.
```

## Escribiendo contenido

Si prefieres pasar a la acción, habrás de comenzar [creando una cuenta en GitHub](https://github.com/join). Con ella **podrás [administrar los archivos del sitio web desde el navegador](https://help.github.com/articles/managing-files-on-github/)**.

El contenido del sitio web de la asociación se encuentra en el directorio [`content`](https://github.com/python-spain/web/tree/master/content) y está escrito en [Markdown](https://daringfireball.net/projects/markdown/syntax), lenguage de marcado sencillo que habrás de utilizar.

Las revisiones por parte del equipo editorial se realizan a través de la web de GitHub y, aunque el procedimiento es bastante intuitivo, habrás de [familiarizarte con el procedimiento de revisión](#proceso-de-revisión).

> **NOTA**: si prefieres tareas más técnicas o editar el proyecto en un equipo local utilizando `git`, consulta el [README](https://github.com/python-spain/web/#sitio-web-de-la-asociación-python-españa) donde se explica cómo descargar, configurar y probar el sitio web.

### Editando contenido ya existente

Explora el [repositorio original de la asociación](https://github.com/python-spain/web/) y localiza el artículo o página donde se encuentre el error. Si se trata de un artículo, estará bajo la carpeta [`content`](https://github.com/python-spain/web/tree/master/content) directamente. Si se trata de una página, estará bajo la carpeta [`pages`](https://github.com/python-spain/web/tree/master/content/pages).

Una vez hayas encontrado el fichero, edita el contenido desde GitHub, corrige el error pertinente y envía el cambio haciendo click en el botón "_Propose file change_".

### Añadiendo un artículo

Si quieres añadir un artículo, entra en la carpeta [`content`](https://github.com/python-spain/web/tree/master/content) y haz click en el botón "_Create new file_".

Introduce un nombre para el nuevo archivo con el formato `AAAA-MM-DD-titulo-del-post.md` (donde `AAAA-MM-DD` es la fecha en la que te gustaría publicar el post). No incluyas ni tildes, ni espacios, y si no estás seguro sobre la fecha, pon la de hoy. Un ejemplo de título válido es `2017-09-03-domiciliacion-cuotas.md`.

Un artículo está compuesto de dos secciones, metadatos y contenido, separadas por dos líneas vacías. Los metadatos **son obligatorios** y sirven para clasificar el artículo. Son los siguientes:

| Clave   | Descripción                                  |
|---------|----------------------------------------------|
| Title   | Título del artículo                          |
| Date    | Fecha de publicación en formato `AAAA-MM-DD` |
| Summary | Resúmen o extracto del artículo              |
| Author  | Nombre del autor                             |

El contenido se ha de escribir utilizando [Markdown](https://daringfireball.net/projects/markdown/syntax). Un [ejemplo de artículo](https://raw.githubusercontent.com/python-spain/web/master/content/2017-09-03-domiciliacion-cuotas.md) sería:

```md
Title: Ya se puede domiciliar la cuota de Python España
Date: 2017-09-03
Summary: Los socios y las socias lleváis tiempo pidiendo poder domiciliar la cuota de la Asociación. Tras mucho esfuerzo, al fin podemos comunicaros que ¡ya se puede hacer!
Author: Yamila Moreno


Los socios y las socias lleváis tiempo pidiendo poder domiciliar la cuota de la Asociación. Tras mucho esfuerzo, al fin podemos comunicaros que ¡ya se puede hacer!

Hasta hace poco la asociación estaba atada a un banco con condiciones draconianas para varias operaciones, entre ellas la domiciliación. Desde la Junta Directiva no veíamos bien que de los 30€ de la cuota, una parte significativa se fuera para pagar la comisión del banco.
```

Cuando hayas terminado de editar, haz click sobre el botón "_Propose new file_"

### Añadiendo una asociación

El sitio web de la asociación Python España pretende facilitar el acceso a las comunidades locales de Python. Por ello, si conoces una comunidad regional o local que realice actividades relacionadas con el lenguaje, te pedimos que la [añadas a nuestro mapa de comunidades](https://github.com/python-spain/web/edit/master/content/pages/comunidades.md).

Para añadir una nueva comunidad necesitarás [encontrar su latitud y longitud](http://www.mapcoordinates.net/en) en el globo, el nombre de la comunidad y la dirección web. Localiza el texto que pone:

```js
var locations = [
```

Y, **a continuación**, incluye una línea con el siguiente formato:

```
[latitud, longitud, 'Nombre de la comunidad', 'dirección web'],
```

Respeta los corchetes (`[` y `]`), las comillas simples (`'`) que encierran el nombre de la comunidad y la dirección web; conserva también las comas y la coma tras el corchete de cierre. Un ejemplo válido sería la línea del encuentro Python de Murcia:

```
[38.01348, -1.17376, 'Python Meetup Murcia', 'http://www.meetup.com/es-ES/Meetup-de-Python-en-Murcia/'],
```

## Manteniendo el sitio web

No todo es crear contenido. La web también necesita un mantenimiento tanto de de sus capacidades, como de su estructura y diseño. Otra forma de contribuir con el sitio web de la asociación Python España es echando un [vistazo a las _issues_ abiertas](https://github.com/python-spain/web/issues), escoger una y solucionarla.

Estas tareas son técnicas y es recomendable trabajar en un entorno de desarrollo local, utilizando `git` para clonar el repositorio. Consulta el [README](https://github.com/python-spain/web/#sitio-web-de-la-asociación-python-españa) donde se explica cómo descargar, configurar y probar el sitio web.

## Mejorando la documentación

Uno de los objetivos de este repositorio es que sea accesible y fácil de editar para personas sin perfil técnico. Esta guía, por ejemplo, recoge cómo realizar modificaciones diréctamente desde la web. Sin embargo el contenido no es perfecto y seguro que hay mejores maneras de explicar algo o cuestiones que podrían aclararse con una imagen.

Mejorar los documentos [`README.md`](https://github.com/python-spain/web/tree/master/README.md) y [`CONTRIBUTING.md`](https://github.com/python-spain/web/tree/master/CONTRIBUTING.md) es también una forma útil de contribuir con la asociación. Utiliza el mismo procedimiento explicado en la sección [Editando contenido ya existente](#editando-contenido-ya-existente) para proponer cambios en estos ficheros.

## Proceso de revisión

Cuando propongas algún cambio, GitHub creará un _pull request_. Un _pull request_ es una petición en tu nombre, con las alteraciones propuestas, que permite discutir sobre las mismas. El equipo editorial realizará una revisión de la petición y GitHub te irá notificando en tu correo electrónico conforme se añadan nuevos comentarios.

Atiende los cambios que te hayan pedido y discute cívicamente aquellos en los que no estés de acuerdo, añadiendo tus propios comentarios (podrás utilizar la [variante GitHub de Markdown](https://guides.github.com/features/mastering-markdown/) para ello).

Recuerda que puedes editar el fichero directamente desde el navegador, situándote en la página del _pull request_, pestaña "_Files changed_", y haciendo click en el botón etiquetado "_Change this file using the online editor_" y representado con el icono del lápiz.

Solucionar los problemas de un _pull request_ puede no ser el paso final. El proceso de revisión puede repetirse. Atiende las sucesivas revisiones y el equipo editorial aceptará tus cambios cuando todos los problemas se hayan resuelto.

Recuerda que tanto los editores y administradores del repositorio, como tú, somos parte de esta comunidad y estamos sujetos al [código de conducta](https://github.com/python-spain/web/blob/master/CODE_OF_CONDUCT.md#code-of-conduct). Informa de los abusos que observes en las _pull request_ (incluso cuando no sean las tuyas) en contacto2018@es.python.org
