# analca3 Blog: Blog files
***

En este repositorio se encuentran los ficheros necesarios para generar el blog http://blog.analca3.com,
que se encuentra en [este repositorio](). El original es de @iblancasa, muchas
gracias por compartirlo :D.

## ¿Qué son estos ficheros?
Gracias a estos archivos, se puede generar un blog estático utilizando  [Jekyll](https://jekyllrb.com/). El blog utiliza la plantilla [Minimal Mistakes](http://mmistakes.github.io/minimal-mistakes) (cuyo repositorio puedes visitar en el enlace antes proporcionado).


## ¿Cómo funciona?
Busca algún tutorial de Jekyll para instalarlo. Necesitarás [Ruby](https://www.ruby-lang.org/), en una versión superior a la *2.0* .
También te vendrá bien instalar [NodeJS](https://nodejs.org/) y [NPM](https://www.npmjs.com/).

Cuando tengas todo eso instalado, clona este repositorio en tu máquina y, en un terminal, ejecuta:

```bash
bundle exec jekyll build
```

Esto permitirá que se construyan los ficheros del sitio web y se depositen en un directorio llamado "*_site*".

Si quieres ver el resultado en tu navegador, ejecuta:

```bash
bundle exec jekyll serve
```

Se te indicará la dirección a la que debes acceder para ver el sitio web en funcionamiento.

Si, además, deseas que se realicen operaciones de optimización, ejecuta:

```bash
npm install
grunt
bundle exec jekyll build
grunt compress
```

De esta forma, primero se instalarán las dependencias necesarias para realizar la optimización, se realizará una optimización de las imágenes, ficheros Javascript..., se generarán los archivos del blog y se aplica compresión de HTML sobre los ficheros generados. Esto permitirá que el peso de tus páginas disminuya, con un aumento en la velocidad de respuesta por parte del servidor.

**Importante: si tras realizar la compresión vuelves a generar los ficheros (mediante el comando *build* o *serve*), se perderá la compresión de HTML, por lo que deberás volver a ejecutarla.**


## Licencia
La licencia de estos ficheros es la MIT 2014
