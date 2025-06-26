# tamara

Ctra. Estació s/n. 46870 Ontinyent (Valencia)
Telf. 962919375. Fax. 962919376
 E-mail: 46006100@edu.gva.es
Resumen LMSGI
Apuntes
DTD
<!ELEMENT >
<!ATTLIST >
<!ELEMENT br EMTY >
<!ELEMENT nombre (#PCDATA) >
<!ELEMENT a ANY>
<!ELEMENT libro (TITULO, AUTOR) >
<!ELEMENT libro (TITULO |AUTOR) >
<!ATTLIST Pelicula Genero (Ficcion | Terror) “Terror">
<!ATTLIST Autor Nacionalidad CDATA >
?
*
+
#IMPLIED
#REQUIRED
#FIXED
SCHEMA
<xs:schema></ xs:schema>
<xs:element></ xs:element>
<xs:complexType></ xs:complexType>
<xs:simpleType></ xs:simpleType>
<xs:restriction></ xs:restriction>
<xs:group></ xs:group>
<xs:secuence></ xs:secuence>
<xs:choice></ xs:choice>
<xs:all></ xs:all>
<xs:complexType mixed=true></ xs:complexType >
<xs:simpleContent></ xs:simpleContent>
<xs:extension base= ></xs:extension>
<xs:attribute></xs:attribute>
string
boolean
integer
positiveInteger
negativeInteger
decimal
dataTime
duration
time
date
gYear
gMothDay
gDay
gMonth
anyUri
ID
length
minLength
maxLength
enumeration
whitespace
(max/min)(In/Ex)clusive
totalDigits
fractionDigits
(min/max)Occurs
[A-Z a-z]
[A-Z]
[a-z]
[0-9]
\D
(A)
A|B
A?
A+
[abcd]
[^abcd]
\t
1
Ctra. Estació s/n. 46870 Ontinyent (Valencia)
Telf. 962919375. Fax. 962919376
 E-mail: 46006100@edu.gva.es
XPATH
Nodo raiz /
Nodo elemento <elemento>
Nodo atributo atributo = "A01"
Nodo texto 
Selección de atributos @atributo
Ruta Relativa /
Ruta absoluta ./
Descendiente de en cualquier nivel //
text()
Predicado [precio > 20]
Operadores (=,!=,>,<,>=,<=)
Operadores lógicos and, or
Acceso por posición [n],[last()], position()
Funciones de Cadena:
• string()
• string-length(string)
• concat(string1, string2,string3, 
string4,...)
• contains(string1, string2)
• starts-with(string1, string2)
• substring(string, start, length?)
• substring-after(string1, string2)
• substring-before(string1, string2)
• translate(string, ‘caracteresASustituir’, 
‘caracteresQueSustituyen’)
Funciones de Numéricas:
• count(node-set)
• sum(node-set)
Funciones de Booleanas:
• not()
• true()
• false()
Unión (|)
XSLT
<xsl:value-of select="."/>
<xsl:value-of select="ExpresiónXpath"/>
<xsl:for-each select="ExpresiónXpath"></ xsl:for-each>
<xsl:if test="ExpresiónXpath"> </xsl:if>
<xsl:stylesheet version="1.0"xmlns:xsl="http://www.w3.org/1999/XSL/Transform"></xsl:stylesheet>
<xsl:template match="/"> </xsl:template>
<xsl:choose>
 <xsl:when test=" = ''">
 </xsl:when>
 <xsl:when test=" = ''">
 </xsl:when>
 <xsl:otherwise>
 </xsl:otherwise>
</xsl:choose>
<xsl:sort select="ExpresiónXpath" date-type="" order=""/>
<xsl: variable name="" select=""></xsl: variable>
Plantillas con nombre:
Definición: <xsl:template name="nombrePlantilla"> </xsl:template>
Llamada:<xsl:call- template name="nombrePlantilla"/>
2
Ctra. Estació s/n. 46870 Ontinyent (Valencia)
Telf. 962919375. Fax. 962919376
 E-mail: 46006100@edu.gva.es
HTML
• <input type="button">
• <input type="checkbox">
• <input type="color">
• <input type="date">
• <input type="datetime-local">
• <input type="email">
• <input type="file">
• <input type="hidden">
• <input type="image">
• <input type="month">
• <input type="number">
• <input type="password">
• <input type="radio">
• <input type="range">
• <input type="reset">
• <input type="search">
• <input type="submit">
• <input type="tel">
• <input type="text">
• <input type="time">
• <input type="url">
• <input type="week">
• <label for=""></label> 
• <fieldset> </fieldset>
• <legend>Personalia:</legend>
• <form> </form> 
• <select name="" id="">
 <optgroup label="">
 <option value=""></option>
 <option value=""></option>
 </optgroup>
</select> 
• <table></table>
• <th></th>
• <td></td>
• colspan
• rowspan
CSS
<link rel="stylesheet" type="text/css" href="xxx.css">
selector{
property:value;
}
class=nombre .nombre
id= nombre #nombre
Atributos de color y fondo:
• color
• background-color
• background-image
Atributos de fuente:
• font-size
• font-family
• font-style
Atributos de texto:
• text-align
Atributos de caja:
• margin
• margin-rigth
• margin-top
• margin-bottom
• margin-left
• padding
• padding-rigth
• padding-top
• padding-bottom
• padding-left
• border
• border-rigth
• border-top
• border-bottom
• border-left
• border-rigth-color
• border-top-color
• border-bottom-color
• border-left-color
• width
• height
3
