# Hola HiCode Student!

<h1 align="center"> 1. Simple CSS selectors</h1> 

## 1. Universal selector
El selector universal, también conocido como comodín, selecciona todo, cada elemento del documento.

Para usar el selector universal, use el carácter de asterisco, *.

```css
* {
    property: value;
}
```
Puede usar el selector universal para restablecer el relleno y el margen predeterminados del navegador a cero en la parte superior del archivo antes de agregar cualquier otro estilo:

```css
* {
    padding: 0;
    margin:  0;
}
```
## 2. Type selector

El selector de tipo CSS selecciona todos los elementos HTML del tipo especificado.

Para usarlo, menciona el nombre del elemento HTML.

Por ejemplo, si quisiera aplicar un estilo a cada párrafo del documento HTML, especificaría el elemento p:

```css
p {
    property: value;
}
```
El código anterior coincide y selecciona todos los elementos p dentro del documento y les da estilo.

## 3. Class selector
El selector de clase hace coincidir y selecciona elementos HTML en función del valor de su clase determinada. Específicamente, selecciona cada elemento en el documento con ese nombre de clase específico.

Con el selector de clases, puede seleccionar varios elementos a la vez y diseñarlos de la misma manera sin copiar y pegar los mismos estilos para cada uno por separado.

Las clases son reutilizables, lo que las convierte en una buena opción para practicar el desarrollo DRY. DRY es un principio de programación y es la abreviatura de 'Don't Repeat Yourself'. Como sugiere el nombre, el objetivo es evitar escribir código repetitivo siempre que sea posible.

Para seleccionar elementos con el selector de clase, utilice el carácter de punto, ., seguido del nombre de la clase.
```css
.my_class {
    property: value;
}
```

En el código anterior, los elementos con una clase de my_class se seleccionan y se les aplica el estilo correspondiente.


## 4. ID selector
El selector de ID selecciona un elemento HTML en función del valor de su atributo de ID.

Tenga en cuenta que la ID de un elemento debe ser única en un documento, lo que significa que solo debe haber un elemento HTML con ese valor de ID dado. No puede usar el mismo valor de ID en un elemento diferente además de ese.

Para seleccionar un elemento con una ID específica, use el carácter hash, #, seguido del nombre del valor de la ID:
```css
#my_id {
    property: value;
}
```
El código anterior coincidirá solo con el elemento único con el valor de ID de my_id.

Vale la pena mencionar que es mejor tratar de limitar el uso de este selector y optar por usar el selector de clase en su lugar. La aplicación de estilos mediante el selector de ID no es ideal porque los estilos no son reutilizables.
## 5. Grouping CSS Selector
With the grouping selector, you can target and style more than one element at once.

To use the grouping selector, use a comma, , to group and separate the different elements you want to select.

For example, here is how you would target multiple elements such as divs, ps, and spans all at once and apply the same styles to each of them:

```css
div, p, span {
    property: value;
}
```

## 5. Ejemplos
```css
body {
	background-color: blue;
}
img {
	width: 150px;
	height: 150px;
}

color: white;
font-size: 12pt;
font-weight: bold;
text-align: center;
text-align: left;
text-align: right;
font-family: Comic Sans MS;

```

> Referencias:\
> Este documento es modificado de este [sitio web](https://www.freecodecamp.org/news/css-selectors-cheat-sheet-for-beginners/)

<h1 align="center"> 2. HTML tags</h1> 

Las etiquetas HTML son como palabras clave que definen cómo el **Navegador Web** ```Google Chrome, Microsoft Edge, Brave, Duckgo, Firefox, Safari, Opera, etc.``` formateará y mostrará el contenido. Con la ayuda de las etiquetas, un navegador web puede distinguir entre un contenido HTML y un contenido simple. Las etiquetas HTML contienen tres partes principales:

<p align="center"> <strong> &lt;TAG DE APERTURA &gt; </strong> contenido <strong> &lt;/ TAG DE CIERRE&gt; </strong</p>

Observa bien que el tag de cierre contiene un ```/``` 

Un archivo HTML debe tener algunas etiquetas esenciales para que el navegador web pueda **diferenciar** entre un **texto simple** y un **texto HTML**. Puede usar tantas etiquetas como desee según los requisitos de su código.

Todos los tag HTML deben encerrarse entre estos **&lt; &gt;**  símbolos. Cada tag HTML realiza una tarea diferente. Si has usado un tag de apertura &lt;tag&gt;, entonces debes usar un tag de cierre &lt;/tag&gt;.
Pero algunas etiquetas HTML son etiquetas no cerradas. 

***
*<h3 align="right">2.1. Etiquetas que no necesitan tag de cierre</h3>*

***



```Input:```
``` html
Hello <br> World 
```
```Output:``` Inserta un salto de linea o un "enter".

Hello  
World

***

```Input:```
``` html
<hr> 
```
```Output:``` Crea una linea horizontal, como las que está dividiendo estos ejemplos.


***
*<h3 align="right">2.2. Meta tags</h3>*

***



```Input:```
```html
<!DOCTYPE html>
```
```Output:``` Esta etiqueta se utiliza para especificar la versión de HTML. Todos los documentos HTML deben comenzar con un tag <!DOCTYPE>. La declaración no es un tag HTML. Es una "información" para el navegador sobre qué tipo de documento esperar.
***

```Input:```
```html
<title> W3Docs - learn HTML, CSS, </title>
```
```Output:```  Define el título o nombre de un documento HTML.  
	
![alt text](https://www.w3docs.com/uploads/media/default/0001/01/7b3d860b4b4b4dabfeae3a12e3229b27339d9e7c.png "Title")
***

```Input:```
```html
<link href="my_style.css" rel="stylesheet" type="text/css">
```
```Output:``` Permite decirle al computador que otros archivos son parte de este documento. En el ejemplo podemos ver que lo usamos para enlazar nuestro archivo CSS. Representa una relación entre el documento actual y un recurso externo. 
***

```Input:```
```html
<meta charset="UTF-8">
<meta name="description" content="Free Web tutorials">
<meta name="keywords" content="HTML, CSS, JavaScript">
<meta name="author" content="John Doe">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
```Output:```  Define los metadatos de un documento HTML. No hay nada visible de estos tags.
***

```Input:```
```html
<style>
  h1 {
    color:red;
  }
  p {
    color:blue;
  }
</style>
```
```Output:``` Uselo para aplicar un estilo simple a un documento HTML.

***

*<h3 align="right">2.3. Tags de texto</h3>*

***




```Input:```
```html
<h1> H1 </h1> 
<h2> H2 </h2> 
<h3> H3 </h3> 
<h4> H4 </h4> 
<h5> H5 </h5> 
<h6> H6 </h6>
```
```Output:```

# H1
## H2
### H3
#### H4
##### H5
###### H6

***

```Input:```
```html
El computador <strong> no tiene partes </strong>, el sistema computacional, si.
```
```Output:```  Definir texto importante en un documento.  

El computador **no tiene partes**. El sistema computacional, si.


***

```Input:```
```html
El computador <em> no tiene partes</em>, el sistema computacional, si.
```
```Output:```  Marcar texto enfatizado en un documento.  
El computador <em> no tiene partes</em>, el sistema computacional, si.

***

```Input:```
```html
The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.
```
```Output:```  Una abreviatura está marcada de la siguiente manera. Pon el mouse encima de la palabra sin hacer click para que notes el resultado.

The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.

***

```Input:```
```html
<bdo dir="rtl">Hola! estudiante hicode.</bdo>
<bdo dir="ltr">Hola! estudiante hicode.</bdo>
```
```Output:```  Especifique la dirección del texto.  

<bdo dir="rtl">Hola! estudiante hicode.</bdo>  
<bdo dir="ltr">Hola! estudiante hicode.</bdo>

***

```Input:```
```html
<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 50 years, WWF has been protecting the future of nature. The world's leading conservation organization, WWF works in 100 countries and is supported by 1.2 million members in the United States and close to 5 million globally.
</blockquote>
```
```Output:```  Una sección que se cita de otra fuente. El computador hace un diferencia notoria cuando usas este tag.

<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 50 years, WWF has been protecting the future of nature. The world's leading conservation organization, WWF works in 100 countries and is supported by 1.2 million members in the United States and close to 5 million globally.
</blockquote>

***

```Input:```
```html
<img src="[img_the_scream.jpg](https://www.w3schools.com/tags/img_the_scream.jpg)" width="220" height="277" alt="The Scream">
<br>
<cite>The Scream</cite> by Edward Munch. Fue pintada en 1893.
```
```Output:```  Define el título de una obra con la etiqueta.

<img src="https://www.w3schools.com/tags/img_the_scream.jpg" width="220" height="277" alt="The Scream">  

<cite>The Scream</cite> by Edward Munch. Fue pintada en 1893.

***

```Input:```
```html
WWF's goal is to: <q>Build a future where people live in harmony with nature.</q> We hope they succeed.
```
```Output:```  Marque una cita corta. Lo pone entre comillas.

WWF's goal is to: <q>Build a future where people live in harmony with nature.</q> We hope they succeed.

***

```Input:```
```html
My favorite color is <del>blue</del> <ins>red</ins>!
```
```Output:```  Un texto con una parte eliminada y una nueva parte insertada.
My favorite color is <del>blue</del> <ins>red</ins>!

***

```Input:```
```html
<dfn>HTML</dfn> is the standard markup language for creating web pages.
```
```Output:```  La etiqueta representa el "elemento de definición" y especifica un término que se definirá dentro del contenido.

<dfn>HTML</dfn> is the standard markup language for creating web pages.

***

```Input:```
```html
Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy text (Windows).
```
```Output:```  Defina algún texto como entrada de teclado en un documento.

Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy text (Windows).

***

```Input:```
```html
<pre>
Text in a pre element
is displayed in a fixed-width
font, and it preserves
both      spaces and
line breaks
</pre>

```
```Output:```  El computador considerará el texto tal cual como lo coloques.
<pre>
Text in a pre element
is displayed in a fixed-width
font, and it preserves
both      spaces and
line breaks
</pre>

***
*<h3 align="right">2.4. Etiquetas de hipervínculo</h3>*

***

```Input:```
```html
Visita <a href="https://www.hicode.education"> hicode.education</a> !
```
```Output:```  Este tag sirve para crear hipervínculos.

Visita <a href="https://www.hicode.education"> hicode.education</a> !

***
*<h3 align="right">2.5. Etiquetas para imagen</h3>*

***

```Input:```
```html
<img src="https://www.w3schools.com/tags/img_girl.jpg" alt="Girl in a jacket" width="250" height="300">
```
```Output:```  Este tag sirve para colocar imágenes en nuestro documento HTML.  

<img src="https://www.w3schools.com/tags/img_girl.jpg" alt="Girl in a jacket" width="250" height="300">

***

```Input:```
```html
<img src="workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">

<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.html">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="phone.html">
  <area shape="circle" coords="337,300,44" alt="Cup of coffee" href="coffee.html">
</map>
<!-- coords
  x1,y1,x2,y2	Specifies the coordinates of the top-left and bottom-right corner of the rectangle (shape="rect")
  x,y,radius	Specifies the coordinates of the circle center and the radius (shape="circle")
  -->
```
```Output:```   Un mapa de imágenes, con áreas en las que se puede hacer clic.

<img src="https://www.w3schools.com/tags/workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">

<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.htm">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="phone.htm">
  <area shape="circle" coords="337,300,44" alt="Cup of coffee" href="coffee.htm">
</map>

***
*<h3 align="right">2.6. Etiquetas para listas</h3>*

***

```Input:```
```html
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<ol start="50">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
```Output:``` Dos listas ordenadas diferentes (la primera lista comienza en 1 y la segunda comienza en 50). 
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<ol start="50">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

***

```Input:```
```html
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```
```Output:```  Una lista HTML sin orden específico.
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>

***

```Input:```
```html
<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>
  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>
```
```Output:```  Una lista de descripción, con términos y descripciones:
<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>
  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>

***
*<h3 align="right">2.7. Etiquetas de tabla</h3>*

***

```Input:```
```html
<table>
  <caption>Monthly savings</caption>
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$80</td>
  </tr>
</table>
```
```Output:```  Una tabla HTML simple, que contiene dos columnas, dos filas y un sibtítulo.
<table>
  <caption>Monthly savings</caption>
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$80</td>
  </tr>
</table>

***
*<h3 align="right">2.8. Etiquetas de formulario</h3>*

***

```Input:```
```html
<form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
</form>
```
```Output:```   Un formulario HTML con dos campos de entrada y un botón de envío.
<form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
</form>

***

```Input:```
```html
<form action="/action_page.php">
  <p><label for="w3review">Review of W3Schools:</label></p>
  <textarea id="w3review" name="w3review" rows="4" cols="50">At w3schools.com you will learn how to make a website. They offer free tutorials in all web development technologies.</textarea>
  <br>
  <input type="submit" value="Submit">
</form>
```
```Output:```  Una entrada de texto de varias líneas (área de texto).
<form action="/action_page.php">
  <p><label for="w3review">Review of W3Schools:</label></p>
  <textarea id="w3review" name="w3review" rows="4" cols="50">At w3schools.com you will learn how to make a website. They offer free tutorials in all web development technologies.</textarea>
  <br>
  <input type="submit" value="Submit">
</form>

***

```Input:```
```html
<form action="/action_page.php">
  <label for="cars">Choose a car:</label>
  <select name="cars" id="cars">
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
    <option value="opel">Opel</option>
    <option value="audi">Audi</option>
  </select>
  <br><br>
  <input type="submit" value="Submit">
</form>
```
```Output:```  Una lista desplegable con cuatro opciones.
<form action="/action_page.php">
  <label for="cars">Choose a car:</label>
  <select name="cars" id="cars">
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
    <option value="opel">Opel</option>
    <option value="audi">Audi</option>
  </select>
  <br><br>
  <input type="submit" value="Submit">
</form>

***

```Input:```
```html
<form action="/action_page.php">
  <label for="cars">Choose a car:</label>
  <select name="cars" id="cars">
    <optgroup label="Swedish Cars">
      <option value="volvo">Volvo</option>
      <option value="saab">Saab</option>
    </optgroup>
    <optgroup label="German Cars">
      <option value="mercedes">Mercedes</option>
      <option value="audi">Audi</option>
    </optgroup>
  </select>
  <br><br>
  <input type="submit" value="Submit">
</form>
```
```Output:```  Agrupe las opciones relacionadas con las etiquetas.  
<form action="/action_page.php">
  <label for="cars">Choose a car:</label>
  <select name="cars" id="cars">
    <optgroup label="Swedish Cars">
      <option value="volvo">Volvo</option>
      <option value="saab">Saab</option>
    </optgroup>
    <optgroup label="German Cars">
      <option value="mercedes">Mercedes</option>
      <option value="audi">Audi</option>
    </optgroup>
  </select>
  <br><br>
  <input type="submit" value="Submit">
</form>

***

```Input:```
```html
<button type="button" onclick="alert('Hello world!')">Click Me!</button>
```
```Output:```  Un botón en el que se puede hacer clic.  

<button type="button" onclick="alert('Hello world!')">Click Me!</button>

***

```Input:```
```html
<form action="/action_page.php">
 <fieldset>
  <legend>Personalia:</legend>
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <label for="email">Email:</label>
  <input type="email" id="email" name="email"><br><br>
  <label for="birthday">Birthday:</label>
  <input type="date" id="birthday" name="birthday"><br><br>
  <input type="submit" value="Submit">
 </fieldset>
</form>
```
```Output:```  Agrupar elementos relacionados en un formulario.  
<form action="/action_page.php">
 <fieldset>
  <legend>Personalia:</legend>
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <label for="email">Email:</label>
  <input type="email" id="email" name="email"><br><br>
  <label for="birthday">Birthday:</label>
  <input type="date" id="birthday" name="birthday"><br><br>
  <input type="submit" value="Submit">
 </fieldset>
</form>
