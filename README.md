# Resumen LMSGI - Guía de Referencia Completa

## DTD (Document Type Definition)

### Declaraciones básicas
```dtd
<!ELEMENT nombre (#PCDATA)>
<!ELEMENT br EMPTY>
<!ELEMENT a ANY>
<!ELEMENT libro (TITULO, AUTOR)>
<!ELEMENT libro (TITULO | AUTOR)>
<!ATTLIST Pelicula Genero (Ficcion | Terror) "Terror">
<!ATTLIST Autor Nacionalidad CDATA>
```

### Modificadores de frecuencia
- `?` - Opcional (0 o 1 vez)
- `*` - Cero o más veces
- `+` - Una o más veces

### Atributos
- `#IMPLIED` - Atributo opcional
- `#REQUIRED` - Atributo obligatorio
- `#FIXED` - Atributo con valor fijo

## XML Schema

### Elementos principales
```xml
<xs:schema></xs:schema>
<xs:element></xs:element>
<xs:complexType></xs:complexType>
<xs:simpleType></xs:simpleType>
<xs:restriction></xs:restriction>
<xs:group></xs:group>
<xs:sequence></xs:sequence>
<xs:choice></xs:choice>
<xs:all></xs:all>
<xs:complexType mixed="true"></xs:complexType>
<xs:simpleContent></xs:simpleContent>
<xs:extension base=""></xs:extension>
<xs:attribute></xs:attribute>
```

### Tipos de datos
- `string`
- `boolean`
- `integer`
- `positiveInteger`
- `negativeInteger`
- `decimal`
- `dateTime`
- `duration`
- `time`
- `date`
- `gYear`
- `gMonthDay`
- `gDay`
- `gMonth`
- `anyUri`
- `ID`

### Restricciones
- `length`
- `minLength`
- `maxLength`
- `enumeration`
- `whitespace`
- `maxInclusive/maxExclusive`
- `minInclusive/minExclusive`
- `totalDigits`
- `fractionDigits`
- `minOccurs/maxOccurs`

### Expresiones regulares
- `[A-Z a-z]` - Letras mayúsculas, minúsculas y espacios
- `[A-Z]` - Solo mayúsculas
- `[a-z]` - Solo minúsculas
- `[0-9]` - Dígitos
- `\D` - No dígitos
- `(A)` - Grupo
- `A|B` - A o B
- `A?` - A opcional
- `A+` - Una o más A
- `[abcd]` - Cualquiera de estos caracteres
- `[^abcd]` - Cualquier carácter excepto estos
- `\t` - Tabulación

## XPath

### Tipos de nodos
- **Nodo raíz**: `/`
- **Nodo elemento**: `<elemento>`
- **Nodo atributo**: `atributo = "A01"`
- **Nodo texto**: contenido textual

### Navegación
- **Selección de atributos**: `@atributo`
- **Ruta relativa**: `/`
- **Ruta absoluta**: `./`
- **Descendiente en cualquier nivel**: `//`
- **Texto**: `text()`

### Predicados y operadores
- **Predicado**: `[precio > 20]`
- **Operadores**: `=`, `!=`, `>`, `<`, `>=`, `<=`
- **Operadores lógicos**: `and`, `or`
- **Acceso por posición**: `[n]`, `[last()]`, `position()`

### Funciones de cadena
- `string()`
- `string-length(string)`
- `concat(string1, string2, string3, string4, ...)`
- `contains(string1, string2)`
- `starts-with(string1, string2)`
- `substring(string, start, length?)`
- `substring-after(string1, string2)`
- `substring-before(string1, string2)`
- `translate(string, 'caracteresASustituir', 'caracteresQueSustituyen')`

### Funciones numéricas
- `count(node-set)`
- `sum(node-set)`

### Funciones booleanas
- `not()`
- `true()`
- `false()`

### Unión
- `|` - Operador de unión

## XSLT

### Estructura básica
```xml
<xsl:stylesheet version="1.0" xmlns:xsl="http://www.w3.org/1999/XSL/Transform">
</xsl:stylesheet>

<xsl:template match="/">
</xsl:template>
```

### Elementos principales
```xml
<xsl:value-of select="."/>
<xsl:value-of select="ExpresiónXpath"/>
<xsl:for-each select="ExpresiónXpath"></xsl:for-each>
<xsl:if test="ExpresiónXpath"></xsl:if>
```

### Estructuras de control
```xml
<xsl:choose>
    <xsl:when test=" = ''">
    </xsl:when>
    <xsl:when test=" = ''">
    </xsl:when>
    <xsl:otherwise>
    </xsl:otherwise>
</xsl:choose>
```

### Ordenamiento y variables
```xml
<xsl:sort select="ExpresiónXpath" data-type="" order=""/>
<xsl:variable name="" select=""></xsl:variable>
```

### Plantillas con nombre
```xml
<!-- Definición -->
<xsl:template name="nombrePlantilla">
</xsl:template>

<!-- Llamada -->
<xsl:call-template name="nombrePlantilla"/>
```

## HTML

### Tipos de input
```html
<input type="button">
<input type="checkbox">
<input type="color">
<input type="date">
<input type="datetime-local">
<input type="email">
<input type="file">
<input type="hidden">
<input type="image">
<input type="month">
<input type="number">
<input type="password">
<input type="radio">
<input type="range">
<input type="reset">
<input type="search">
<input type="submit">
<input type="tel">
<input type="text">
<input type="time">
<input type="url">
<input type="week">
```

### Elementos de formulario
```html
<label for=""></label>
<fieldset></fieldset>
<legend>Personalia:</legend>
<form></form>

<select name="" id="">
    <optgroup label="">
        <option value=""></option>
        <option value=""></option>
    </optgroup>
</select>
```

### Tablas
```html
<table></table>
<th></th>
<td></td>
<!-- Atributos: colspan, rowspan -->
```

### Estructura básica
```html
<!DOCTYPE HTML PUBLIC...>
<html></html>
<title></title>
<head></head>
<body></body>
```

### Atributos del body
```html
background="url"
bgproperties="fixed"
bgcolor="color"
text="color"
link="color"
vlink="color"
alink="color"
```

### Etiquetas básicas de formato
```html
<b></b>         <!-- Negrita -->
<i></i>         <!-- Cursiva -->
<u></u>         <!-- Subrayado -->
<sub></sub>     <!-- Subíndice -->
<sup></sup>     <!-- Superíndice -->
<tt></tt>       <!-- Typewriter -->
<pre></pre>     <!-- Preformateado -->
<em></em>       <!-- Énfasis -->
<strong></strong> <!-- Fuerte -->
<big></big>     <!-- Grande -->
<small></small> <!-- Pequeño -->
```

### Estructura de contenidos
```html
<p></p>         <!-- Párrafo -->
<br>            <!-- Salto de línea -->
<hnúm></hnúm>   <!-- Encabezados h1-h6 -->
<hr>            <!-- Línea horizontal -->
<div></div>     <!-- División -->
<span></span>   <!-- Span -->
```

### Hipervínculos
```html
<a href="url"></a>
<a href="url#nombre_ancla"></a>
<a href="#nombre_ancla"></a>
<a href="mailto:@"></a>
<a href="mailto:@?subject=cad_caracteres"></a>
<a name="cad_caracteres"></a>
```

### Listas
```html
<ul></ul>       <!-- Lista no ordenada -->
<ol></ol>       <!-- Lista ordenada -->
<li></li>       <!-- Elemento de lista -->
<dl></dl>       <!-- Lista de definiciones -->
<dt></dt>       <!-- Término de definición -->
<dd></dd>       <!-- Definición -->
```

## CSS

### Enlace de hoja de estilos
```html
<link rel="stylesheet" type="text/css" href="xxx.css">
```

### Sintaxis básica
```css
selector {
    property: value;
}
```

### Selectores
- **Clase**: `.nombre`
- **ID**: `#nombre`
- **Universal**: `*`
- **Elemento**: `div`
- **Descendiente**: `div span`
- **Hijo directo**: `div > span`
- **Hermano adyacente**: `div + span`
- **Atributo**: `a[class]`, `a[class='x']`

### Atributos de color y fondo
- `color`
- `background-color`
- `background-image`

### Atributos de fuente
- `font-size`
- `font-family`
- `font-style`

### Atributos de texto
- `text-align`

### Modelo de caja
```css
margin
margin-right
margin-top
margin-bottom
margin-left
padding
padding-right
padding-top
padding-bottom
padding-left
border
border-right
border-top
border-bottom
border-left
width
height
```

### Posicionamiento
```css
position: static | relative | absolute | fixed;
left: auto | longitud;
top: auto | longitud;
right: auto | longitud;
bottom: auto | longitud;
z-index: auto | número;
```

### Pseudo-clases y pseudo-elementos
```css
:active         /* Elemento seleccionado */
:focus          /* Elemento enfocado */
:hover          /* Cursor encima */
:link           /* Vínculo no visitado */
:visited        /* Vínculo visitado */
:first-child    /* Primer hijo */
:first-letter   /* Primera letra */
:first-line     /* Primera línea */
:before         /* Antes del elemento */
:after          /* Después del elemento */
```

### Unidades de medida
- `px` - Píxeles
- `em` - Relativo al tamaño de fuente
- `%` - Porcentaje
- `pt` - Puntos
- `cm`, `mm`, `in` - Unidades absolutas

### Colores
- Hexadecimal: `#ff6633`, `#f63`
- RGB: `rgb(0,255,0)`, `rgb(0%,100%,50%)`
- Nombres: `red`, `blue`, `green`, etc.

## Comentarios
- **HTML**: `<!-- comentario -->`
- **CSS**: `/* comentario */`
- **XML/XSLT**: `<!-- comentario -->`
