# Practica 1

## Ejercicio 1

1. HTML(hyper text markup language) es un lenguaje marcado para la elaboración de páginas web. Define una estructura básica y un código para la definición de contenido. Está a cargo de la W3C. HTML fue creado en 1990, paso por las versiones 3.0, 3.2, 4.01. Actualmente se utiliza la version HTML5

2. Las tecnologías deben ser compatibles con versiones anteriores, las especificaciones y las implementaciones deben coincidir.

3. Con la llegada de las hojas de estilo vinieron métodos más potentes para presentar la información lo que ocasionó la obsolescencia de muchos elementos y atributos de presentación.

4. DTD: declaración del tipo de documento. Se ubica en la primera linea del archivo HTML.
   Segun HTML 4.01, una declaracion transitoria se puede escribir de la siguiente manera:

    <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">

   Aunque con HTML5 se puede resumir a:
    
    <!DOCTYPE HTML>

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

    <a href="http://www.e-style.com.ar/resumen.html" type="text/html" hreflang="es" charset="utf-8" rel="help">Resumen HTML </a>

    a indica un hyperlink, en href se indica la url, type especifica el tipo de contenido, hreflang el idioma, charset el conjunto de caracteres y rel la relacion entre los dos documentos

f.

    <table width="200" summary="Datos correspondientes al ejercicio vencido">
    <caption align="top"> Título </caption>
        <tr>
            <th scope="col">&nbsp;</th>
            <th scope="col">A</th>
            <th scope="col">B</th>
            <th scope="col">C</th>
        </tr>
        <tr>
            <th scope="row">1º</th>
            <td>&nbsp;</td>
            <td>&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <th scope="row">2º</th>
            <td>&nbsp;</td>
            <td>&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
    </table>

    Es la estructura de una tabla, tr indica cada fila y dentro de estas, con td(th para el header), se indican los valores de cada columna
    con scope indicamos si esa celda es header de columna o de fila. &nbsp; inserta un espacio entre las palabras en sus extremos y evita saltos de linea. Se usa para evitar que ante
    una pantalla chica el texto se corte, por ejemplo al poner "$ 5". si en vez del espacio uso nbsp nunca va a haber salto de linea entre el 5 y el $


## Ejercitacion 3

a. 

    <a href="http://www.google.com.ar">Click aquí para ir a Google</a>

    Abre google.com en la misma pestaña

    <a href="http://www.google.com.ar" target="_blank">Click aquí para ir a Google</a>

    Abre google en una pestaña nueva

    <a href="http://www. google.com.ar" type="text/html" hreflang="es" charset="utf-8" rel="help">

    Abre google en la misma pestaña, especifica tipo de pagina, idioma, conjunto de caracteres y relacion

    <a href="#">Click aquí para ir a Google</a>

    Hiperlink que no hace nada

    <a href="#arriba">Click aquí para volver arriba</a>

    Hiperlink que lleva a donde se encuentra la etiqueta arriba en la pagina

    <a name="arriba" id="arriba"></a>

    hiperlink sin texto por lo que no se puede clickear

b.

    <p><img src="im1.jpg" alt="imagen1" /><a href="http://www.google.com.ar">Click aquí</a></p>

    una imagen dentro de un parrafo con un hiperlik debajo

    <p><a href="http://www.google.com.ar"><img src="im1.jpg" alt="imagen1" /></a> Click aquí</p>

    una imagen que funciona como hiperlink dentro de un parrafo

    <p><a href="http://www.google.com.ar"><img src="im1.jpg" alt="imagen1" />Click aquí</a></p>

    una imagen y un texto que funcionan con hiperlink dentro de un parrafo

    <p><a href="http://www.google.com.ar"><img src="im1.jpg" alt="imagen1" /></a> <a href="http://www.google.com.ar">Click aquí</a></p>

    una imagen y una linea de texto dentro de un parrafo que funcionan como dos distintos hyperlinks

c.

    <ul> 
        <li>xxx</li>
        <li>yyy</li>
        <li>zzz</li>
    </ul>

    una lista sin orden de 3 elementos

    <ol>
        <li>xxx</li>
        <li>yyy</li>
        <li>zzz</li>
    </ol>

    una lista ordenada de 3 elementos

    <ol>
        <li>xxx</li>
    </ol>
    <ol>
        <li value="2">yyy</li>
    </ol>
    <ol>
        <li value="3">zzz</li>
    </ol>

    3 listas ordenadas distintas con un elemento cada una aparentando ser una sola

    <blockquote>
        <p>
            1. xxx <br />
            2. yyy <br />
            3. zzz
        </p>
    </blockquote>

    Es una cita que aparenta ser una lista ordenada


d.

    <table border="1" width="300">
        <tr>
            <th>Columna 1</th>
            <th>Columna 2</th>
        </tr>
        <tr>
            <td>Celda 1</td>
            <td>Celda 2</td>
        </tr>
        <tr>
            <td>Celda 3</td>
            <td>Celda 4</td>
        </tr>
    </table>

    Una tabla con un borde de 1 pixel entre las celdas y un ancho de 300 pixeles.

    <table border="1" width="300">
        <tr>
            <td><div align="center"><strong>Columna 1</strong></div></td>
            <td><div align="center"><strong>Columna 2</strong></div></td>
        </tr>
        <tr>
            <td>Celda 1</td>
            <td>Celda 2</td>
        </tr>
        <tr>
            <td>Celda 3</td>
            <td>Celda 4</td>
        </tr>
    </table>

    La misma tabla pero sin especificar los header, se utilzan align center y strong para "imitar".


e.

    <table width="200">
        <caption>    
            Título
        </caption>
        <tr>
            <td bgcolor="#dddddd">&nbsp;</td>
            <td bgcolor="#dddddd">&nbsp;</td>
            <td bgcolor="#dddddd">&nbsp;</td>
        </tr>
        <tr>
            <td bgcolor="#dddddd">&nbsp;</td>
            <td bgcolor="#dddddd">&nbsp;</td>
            <td bgcolor="#dddddd">&nbsp;</td>
        </tr> 
    </table>

    <table width="200">
        <tr>
            <td colspan="3">
                <div align="center">
                    Título
                </div>
            </td>
        </tr>
        <tr>
            <td bgcolor="#dddddd">&nbsp;</td>
            <td bgcolor="#dddddd">&nbsp;</td>
            <td bgcolor="#dddddd">&nbsp;</td>
        </tr>
        <tr>
            <td bgcolor="#dddddd">&nbsp;</td>
            <td bgcolor="#dddddd">&nbsp;</td>
            <td bgcolor="#dddddd">&nbsp;</td>
        </tr>
    </table>

    En la primer tabla se usa el elemento caption para definir el título de la tabla, lo que lo centra mientras que en la segunda se imita el efecto al crear una fila de 3 celdas de ancho con "Título" centrado.


f.

    <table width="200">
        <tr>
            <td colspan="3">
                <div align="center">Título</div>
            </td>
        </tr>
        <tr>
            <td rowspan="2" bgcolor="#dddddd">&nbsp;</td>
            <td bgcolor="#dddddd">&nbsp;</td>
            <td bgcolor="#dddddd">&nbsp;</td>
        </tr>
        <tr>
            <td bgcolor="#dddddd">&nbsp;</td>
            <td bgcolor="#dddddd">&nbsp;</td>
        </tr>
    </table>

    <table width="200">
        <tr>
            <td colspan="3">
                <div align="center">Título</div>
            </td>
        </tr>
        <tr>
            <td colspan="2" bgcolor="#dddddd">&nbsp;</td>
            <td bgcolor="#dddddd">&nbsp;</td>
        </tr>
        <tr>
            <td bgcolor="#dddddd">&nbsp;</td>
            <td bgcolor="#dddddd">&nbsp;</td>
            <td bgcolor="#dddddd">&nbsp;</td>
        </tr>
    </table>

    En la primer tabla se utiliza colspan para crear una celda que ocupe dos columnas y en la segunda tabla se utiliza rowspan para que la celda ocupe dos filas

g.

    <table width="200" border="1">
        <tr>
            <td colspan="3">
                <div align="center">Título</div>
            </td>
        </tr>
        <tr>
            <td colspan="2" rowspan="2">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="50%">&nbsp;</td>
        </tr>
    </table>


    <table width="200" border="1" cellpadding="0" cellspacing="0">
        <tr>
            <td colspan="2">
                <div align="center">Título</div>
            </td>
        </tr>
        <tr>
            <td rowspan="2">&nbsp;</td>
            <td>&nbsp;</td>
        </tr>
        <tr>
            <td width="50%">&nbsp;</td>
        </tr>
    </table>

    Ambas tablas tienen un borde de 1 pixel y pero la segunda tiene un padding de 0 para que no haya separación entre las tablas.
    La primer tabla tiene un colspan de 3 en el titulo aunque la tabla solo tiene 2 columnas. Ya que el número es mayor a la cantidad de columnas en el error no es aparente.


h.

    <form id="form1" name="form1" action="procesar.php" method="post" target="_blank">
        <fieldset>
            <legend>LOGIN</legend>
            Usuario: <input type="text" id="usu1" name="usu1" value="xxx" /><br />
            Clave: <input type="password" id="clave1" name="clave1" value="xxx" />
        </fieldset>
        <input type="submit" id="boton1" name="boton1" value="Enviar" />
    </form>

    <form id="form2" name="form2" action="" method="get" target="_blank">
        LOGIN<br />
        <label>Usuario: <input type="text" id="usu2" name="usu2" /></label><br />
        <label>Clave: <input type="text" id="clave2" name="clave2" /></label><br />
        <input type="submit" id="boton2" name="boton2" value="Enviar" />
    </form>

    <form id="form3" name="form3" action="mailto:xx@xx.com” enctype=text/plain method="post" target="_blank">
        <fieldset>
            <legend>LOGIN</legend>
            Usuario: <input type="text" id="usu3" name="usu3" /><br />
            Clave: <input type="password" id="clave3" name="clave3" />
        </fieldset>
        <input type="reset" id="boton3" name="boton3" value="Enviar" />
    </form>

    El primer y tercer formulario utilzan fieldset, lo que delimita lo de dentro en un recuadro.
    El primer form tiene valor predeterminados en los campos.
    El segundo formulario no utiliza el type pass por lo que al escribir la contraaseña no aparece como *
    El primer y tercer form usan post lo cual es correcto, ya que el get no debe ser usado para enviar información, ya que aparece todo en el url
    en el segundo form se usa la etiqueta label, y dentro el texto y los inputs.

i.

    <label>Botón 1
        <button type="button" name="boton1" id="boton1">
        <img src="logo.jpg" alt="Botón con imagen " width="30" height="20" /><br />
        <b>CLICK AQUÍ</b></button>
    </label>
    
    La frase "boton 1" con un boton conformado por una imagen y la frase "click aqui"
    
    <label>Botón 2
        <input type="button" name="boton2" id="boton2" value="CLICK AQUÍ" />
    </label>

    La frase "boton 2" con un boton que dice "click aqui"

j.

    <p>
        <label><input type="radio" name="opcion" id="X" value="X" />X</label><br />
        <label><input type="radio" name="opcion" id="Y" value="Y" />Y</label>
    </p>

    <p>
        <label><input type="radio" name="opcion1" id="X" value="X" />X</label><br />
        <label><input type="radio" name="opcion2" id="Y" value="Y" />Y</label>
    </p>

    El segundo grupo de radios tienen distinto name, por lo que se pueden elegir los dos a la vez y si estan en un form, al ser enviado, se enviarían los dos por separado. Mientras que en el primero se enviaría en el mismo atributo cual de ambos fue seleccionado.

k.

    <select name="lista">
        <optgroup label="Caso 1">
            <option>Mayo</option>
            <option>Junio</option>
        </optgroup>
        <optgroup label="Caso 2">
            <option>Mayo</option>
            <option>Junio</option>
        </optgroup>
    </select>

    <select name="lista[]" multiple="multiple">
        <optgroup label=" Caso 1">
            <option>Mayo</option>
            <option>Junio</option>
        </optgroup>
        <optgroup label=" Caso 2">
            <option>Mayo</option>
            <option>Junio</option>
        </optgroup>
    </select>

    el segundo select utiliza la opcion "multiple", lo que permite al usuario seleccionar más de una opción.

