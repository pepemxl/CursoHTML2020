# Introducción a las hojas de estilo CSS


Un concepto fundamental en una página web es la separación entre el contenido y el formato, actualmente para dar formato al texto se utilizan las hojas de estilo en cascada CSS (Cascading Style Sheets). Es decir, en el archivo `.html` se escribe el contenido de la página web con etiquetas html, y en el archivo `.css` se define el estilo o formato del contenido, por ejemplo el color del texto o el tipo de alineación.


## Ejemplo

[codigo html](codigos/clase_03_practica_01.html)

[codigo css](codigos/css/clase_03_practica_01.css)

En este ejemplo, vemos que para enlazar un archivo .html con un archivo .css se utiliza la siguiente etiqueta: `<link rel="stylesheet" type="text/css" href="css/clase_03_practica_01.css" />` que indica que el archivo enlazado se llama clase_03_practica_01.css que se encuentra en la carpeta css.

```
<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="utf-8"/>
        <title>
            Clase 03 Practica 01
        </title>
        <link rel="stylesheet" type="text/css" href="css/clase_03_practica_01.css"/>
    </head>
    <body>
        <h1>Mi primer pratica usando hojas de estilo</h1>
        <p>HOLA MUNDO</p>
        <p class="miestilo01"> Mi primer estilo</p>
        <p class="miestilo02"> Mi segundo estilo</p>
        <p class="miestilo03"> Mi tercero estilo(si no esta definido no hara nada)</p>
        <p class="miestilo04"> Mi 4to estilo</p>
    </body>
</html>
```
En la hoja de estilo vemos que a la etiqueta `h1` se le ha aplicado el estilo para centrar el texto `h1 { text-align: center }`, y a la etiqueta `p` se le ha aplicado el estilo para establecer el tipo de letra y el tamaño del texto `p { (font-family: arial; font-size: 16px; }`, con lo cual a todas las etiquetas `p` se les aplicarán estos dos estilos.

Si en lugar de aplicar un estilo a todas las etiquetas queremos aplicarlo a unas etiquetas en concreto podemos declarar una clase y asignarla sólo a las etiquetas que queramos.

- `.miestilo01`
- `.miestilo02`
- `.miestilo03`
- `.miestilo04`

```
h1 { 
    text-align: center;
}

p { 
    font-family: arial; 
    font-size: 16px; 
}

.miestilo01 {
    color: blue; /* por nombre de color en ingles */
}

.miestilo02 {
    color: #00FF00;/* Hexadecimal para (RGB) */
}

.miestilo04 {
    color: #00FF00;/* Hexadecimal para (RGB) */
    font-style: italic;
    font-weight: bold;
    text-align: center;
}
```

La hoja de estilo también se puede declarar en el mismo archivo .html, concretamente dentro de la etiqueta head, como se muestra en esta página básica:

```
<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="utf-8"/>
        <title>
            Clase 03 Practica 01
        </title>
        <style type="text/css"> 
            h1 { 
    text-align: center;
}

p { 
    font-family: arial; 
    font-size: 16px; 
}

.miestilo01 {
    color: blue; /* por nombre de color en ingles */
}

.miestilo02 {
    color: #00FF00;/* Hexadecimal para (RGB) */
}

.miestilo04 {
    color: #00FF00;/* Hexadecimal para (RGB) */
    font-style: italic;
    font-weight: bold;
    text-align: center;
}
        </style>
    </head>
    <body>
        <h1>Mi primer pratica usando hojas de estilo</h1>
        <p>HOLA MUNDO</p>
        <p class="miestilo01"> Mi primer estilo</p>
        <p class="miestilo02"> Mi segundo estilo</p>
        <p class="miestilo03"> Mi tercero estilo(si no esta definido no hara nada y usará el estilo general de la página)</p>
        <p class="miestilo04"> Mi 4to estilo</p>
    </body>
</html>
```

Las reglas de las hojas de estilo están formadas por el `selector` y entre llaves las `declaraciones` separadas por punto y coma. Una declaración es un `atributo` o `propiedad` seguido por dos puntos y a continuación el valor de la propiedad.

Con la aparición de HTML5 surgieron decendas de selectores y decenas de atributos para cada selector, asi que nos tomará algun tiempo aprender la mayoria de ellos.


## Tarea

Crear página inicial donde el texto deberá estar centrado con una canción/cuento separando sus parrafos de manera apropiada.

