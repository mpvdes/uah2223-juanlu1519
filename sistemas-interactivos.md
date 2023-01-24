# Sistemas interactivos

## HTML

Viene de "Hypertext Markup Language" o lenguaje de marcado de hipertexto. Es el componente más básico de la web. Para la apariencia contamos con CSS y para la funcionalidad, con Javascript.

Utiliza marcas para etiquetar texto, imágenes, etc. Por ejemplo <head>, <title>, <body>...

### Manejo de archivos

Es importante que la estructura de los archivos sea la misma que después tendrá cuando se aloje en un servidor. Prescindimos de mayúsculas, espacios y caracteres como la "_".

### Anatomía de un elemento HTML

![Ejemplo anatomía elemento HTML](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics/grumpy-cat-small.png)

Atributos

![Ejemplo atributos HTML](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics/grumpy-cat-attribute-small.png)

#### Anidar elementos

### Atajos nano

alt + 3: Comentar una línea

alt + A: Marcar texto

alt + 6: Copiar

ctrl + U: Pegar

ctrl + shift + V: Pegar contenido de fuera de nano

alt + I : Activar sangrado

alt + S: Paginar

### Comandos cygwin

cygstart archivo.html : Para abrir en nuestro navegador un archivo html.

python -m http.server: si copiamos el puerto que nos devuelve http://[::]:8000/ y cambiamos esos corchetes en el navegador por localhost nos enseña el estado de nuestra web en nuestro servidor. Usaremos CTRL + C en la terminal para abortar misión.

### Identificadores

Permite identificar un elemento único de una página HTML. Solo se permite un único elemento por ID. Sirven para hacer marcadores y saltar a esa parte de la página. Es una forma de navegar dentro de la web

Ejemplos: 
<p>mi gato es muy gruñón <a href="#cat-info">ver link</a></p>
id="cat-info"

/#identificador al final de una url

href="web" : referencia del hiperenlace.

target="blank" : para que el usuario siga en nuestra web cuando abra el enlace

### Elementos no semánticos

#### Elemento en línea <span>

#### Elemento en bloque <div>

Ejemplo:

<div style="color: blue;">

 <h2> Ejemplo de div y span </h2>

  <p>

    Esto es un párrafo dentro de un div,

    <span style="color: red;"> y esto un span dentro de un párrafo.</span>

  </p>

</div>

Podemos añadir los diferentes atributos separados con ; .

### Estructura elemento HTML

Ejemplo: 

<!DOCTYPE html>

<html>

  <head>

    <meta charset="utf-8">

    <title>Mi pagina de prueba</title>

  </head>

  <body>

    <img src="images/firefox-icon.png" alt="Mi imagen de prueba">

  </body>

</html>

Explicación:

<!DOCTYPE html> : Nos dice que estamos en un documento HTML.

<html>

<head>

<meta charset="utf-8"> Juego de caracteres.

<title>Mi pagina de prueba</title> : El título de nuestra página web. Debe entenderse bien para el SEO.

</head>

<body> Donde van a aparecer todos los elementos visibles de la web.

<img src="images/firefox-icon.png" alt="Mi imagen de prueba">

</body>

</html>

Para ver como está hecha una web podemos darle a inspeccionar.

### Marcado de texto

- Los encabezados van de <h1> a <h6>
- Listas: ordenadas con <ol> o desordenadas con <ul>. Cada elemento de la lista se identifica con <li>.
- Vínculos: Se usan con <a> que viene de "anchor". Para poner url uso href="url". Es importante indicar el protocolo delante https://. 
- Importancia: <em> realza la importancia del texto que encierra. <strong> realza la máxima importancia del texto que encierra. 
- Cita: <blockquote> hacemos una cita textual de otro texto en el texto que encierra. <cite> dentro del blockquote para poner en cursiva quién hace la cita y cite="cita que queremos indicar".
- Abreviatura y acrónimo: usamos <abbr> y <acronym>. Ambos tienen el atributo title= delante.
- Definición: <dfn>. Ejemplo; <dfn id="def-validator">validator</dfn> 
- Inserción y borrado: Cuando queremos borrar o modificar contenido en una publicación realizada. Con <ins> indicamos la modificación y quedará subrayado. Con <del> indicamos el borrado y quedará tachado. En el atributo cite= puede indicar la fuente porque se realiza esa modificación y datetime=, la hora. Tiene que ser un formato válido de tiempo. Ejemplo: El origen del terremoto fue en <del cite="https://aemet.es">Burriana</del> <ins datetime="2023-07-07">Lorca</ins>
- Tiempo: <time> representa un periodo específico de tiempo. Con el atributo datetime= hacemos que sea machine-readable. Esto es una mejora para los resultados de motores de búsqueda o para funciones personalizadas como recordatorios. Ejemplo: Celebramos el 40º aniversario el próximo <time datetime="2010-09-09">9 de septiembre</time>
- Preformateado de texto: Cuando queremos mostrar el texto preformateado y escrito tal y como lo hacemos en el HTML. Se suele renderizar en el navegador con una fuente monoespaciada. Se respetan los espacios en blanco. Usamos <pre> y el escape de caracteres así como &lt; &gt; &quot; etc.
- Mostrar código: Para mostrar código lo hacemos con <code> y si queremos mostrar múltiples líneas de código, las encerramos en <pre>.
- Otros enlaces: <script> para enlazar un script de javascript, por ejemplo. Con este también podemos escribir el código JS directamente en nuestro HTML. Si queremos enlazar a nuestra hoja de estilo CSS, podemos hacerlo con <link>.

## Webs recomendables

w3schools
[Formatos válidos de tiempo](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/time#valid_datetime_values)
