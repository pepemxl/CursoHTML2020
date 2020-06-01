# Introducción a HTML

## HTML Hyper Text Mark Language

HTML podemos traducirlo como lenguaje de etiquetado de texto.


El lenguaje HTML es un estándar definido y mantenido por el consorcio internacional World Wide Web Consortium (W3C) creado el 1 de octubre de 1994, por Tim Berners-Lee en el Instituto Tecnológico de Massachusetts (MIT), actual sede central del consorcio [w3c](https://www.w3.org/).

Las marcas, conocidas como etiquetas, describen la forma en la que se estructura el contenido de una página web.
Todas las nuevas etiquetas que existen las podemos aprender en 
[w3school](https://www.w3schools.com/), actualmente el estandar es HTML5, que introdujo una serie de mejoras que permiten crear páginas dinamicas, utilizar recursos de sistema, como tarjetas de video, archivos, memoria dinamica en el explorador web(chrome, firefox, explorer, etc...).

## Inicio de una pagina web
Todo empieza con un archivo HTML.
El encargado de interpretar las etiquetas dentro del este arhivo html es un programa llamado navegador o browser, ejemplos, el navegador Chrome de Google o el Firefox de Mozilla. Los archivos que contienen el código HTML tienen la extensión .htm o .html, y son archivos de texto plano (sin formato). Una página web debe estar escrita en HTML pero también suele incorporar otros elementos como hojas de estilo CSS y programación como el lenguaje Javascript/PHP/ASP. 

Iniciaremos con en el lenguaje HTML y con hojas de estilo CSS.

Lo primero que necesitamos es crer un archivo html.
Dentro del archivo html creamos la etiqueta `<html>`  que marca el inicio de una página web y `</html>`  que marca el fin.
Etiquetas de inicio y fin de una página web.

```
<html>

</html>
```

## Header

```
<html>
    <head>

    </head>
</html>
```

La meta data se inserta usando los meta tags en la cabecera de la página, entre las etiquetas `<head></head>`. La función de estos tags puede varíar entre ser informativos, para los buscadores y usuarios, indicándoles el tipo de contenido de la web, entre otros. En esta parte podemos incluir hojas de estilo o javascript.

## Cuerpo
```
<html>
    <body>

    </body>
</html>
```

[Ejemplo](codigos/clase_01_practica_01.html)

## Titulo o encabezado
Dentro del titulo podemos poner metadata de la página web
```
<html>
    <head>

    </head>
    <body>

    </body>
</html>
```

### Ejemplo

```
<html>
    <head>
        <title>
            Encabezado web
        </title>
    </head>
    <body>
    <h1>
        Titulo
    </h1>
    </body>
</html>
```

[Ejemplo](codigos/clase_01_practica_02.html)

## Tarea 

- Bajar e Instalar WAMP(Windows, Apache, MySQL, PHP/Perl/Python) de 
[link](https://sourceforge.net/projects/wampserver/).
- Crear nuestro primer archivo html con la leyenda `HOLA MUNDO`

