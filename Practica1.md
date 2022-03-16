# Practica 1

## Ejercicio 1

1. HTML(hyper text markup language) es un lenguaje marcado para la elaboración de páginas web. Define una estructura básica y un código para la definición de contenido. Está a cargo de la W3C. HTML5 es la quinta revisión más importante que se hace al lenguaje. 

3. Con la llegada de las hojas de estilo vinieron métodos más potentes para presentar la información lo que ocasionó la obsolescencia de muchos elementos y atributos de presentación.

4. DTD: declaración del tipo de documento. Se ubica en la primera linea del archivo HTML.

5. Los metadatos son elementos de HTML que muestran información sobre la propia página web. Se encuentran en el head. Por ejemplo: description, que contiene una descripcion resumida sobre la pagina. Author, información sobre el autor de la pagina. Copyright, informa sobre el copyright de la página.

## Ejercicio 2

a. 
    <!-- Código controlado el día 12/08/2009 -->
    Pueden aparecer en cualquier parte del documento, sirven para comentar, este código es ignorado por el navegador

b.
    <div id="bloque1">Contenido del bloque1</div
    div define un bloque de contenido, se encuentra en el body. id especifica un identificador unico para un elemento

c.
    <img src="" alt="lugar imagen" id="im1" name="im1" width="32" height="32" longdesc="detalles.htm" />
    img se usa para insertar una imagen en la pagina, alt es el texto que se mostrará al sobreponer el mouse en la foto, id, especifica un identificador unico. name especifica un nombre para el elemento que puede ser referenciado desde JS y tambien se utiliza al enviar la informacion de los form. width y height especifican un ancho y altura, respectivamente.

d.
    <meta name="keywords" lang="es" content="casa, compra, venta, alquiler " />
    <meta http-equiv="expires" content="16-Sep-2019 7:49 PM" />

    keywords especifica palabras claves(en content) para identificar a la pagina web, lang el idioma de la misma, es utilizado por los buscadores
    http-equiv="expires" indica que pasada esa fecha(content) el navegador debe solicitar la pagina nuevamente al server y no utilizar la en cache

e.

    <a href="http://www.e-style.com.ar/resumen.html" type="text/html" hreflang="es" charset="utf-8" 
    rel="help">Resumen HTML </a>

