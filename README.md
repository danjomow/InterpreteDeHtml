# InterpreteDeHtml
## Pasos para desarrollar el proyecto:

1. Entender los componentes particulares de un archivo HTML.
2. Clasificar los diferentes componentes que tiene un archivo HTML.
3. Almacenar el contenido clasificado por las distintas partes del archivo HTML.
4. Exponer / imprimir el contenido clasificado por las partes del archivo HTML.

## Entender un archivo HTML

Para entender un archivo HTML y sus diferentes partes hay que tener en cuenta que un archivo HTML se compone de código identificado por etiquetas, las cuales se pueden encontrar con una estructura básica de apertura mediante los símbolos "<>".

Teniendo esto en cuenta podríamos entender que los diferentes elementos de un archivo HTML se ven identificados por las distintas etiquetas que tiene el archivo y estas definen los componentes y su comportamiento dentro del archivo.

## Clasificar los componentes del archivo

Para poder clasificarlos y hacer una guía simple de como diferenciar las etiquetas lo haremos mediante el siguiente ejemplo:

```HTMl
<!DOCTYPE html>
<html> 
<head>
	<title>Mi primera página</title> 
</head> 
<body> 
	<h1>¡Hola, mundo!</h1> 
	<p>Este es mi primer párrafo.</p> 
</body> 
</html>
```

Teniendo esto en cuenta, podemos identificar y clasificar los elementos mediante las etiquetas que se le han dado.

- **"!DOCTYPE html"**: Indica el tipo de documento HTML.
- **"html"**:  Raíz de todo el documento.
- **"head"**: Contiene información sobre la página como el título.
- **"title"**: Define el título que aparece en la pestaña del navegador.
- **"body"**: Contiene el contenido visible de la página como el cuerpo de un artículo.
- **"h1"**: Define un encabezado de nivel 1 (se puede llevar a más niveles dependiendo de la necesidad).
- **"p"**: Define un párrafo.

## Almacenar el contenido definido por las etiquetas

En este punto tendremos que plantear una solución que recorra todo el archivo evaluando las etiquetas, es decir, clasificando mediante la lectura de los elementos que se encuentren dentro de los "<>" para que nos permita almacenarlos en arreglos y almacenar el contenido comprendido dentro de la etiqueta mediante conversiones de datos.

## Imprimir el contenido clasificado

Luego de haber recopilado la información, podremos imprimir la información ya clasificada de manera que nos permita recibir el contenido diferenciado entre, cabeceras, títulos, párrafos, etc... para que podamos tener la información a la mano y entender e interpretar de manera sencilla un archivo HTML.
