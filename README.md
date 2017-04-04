# Bootstrap 3

## Introducción

Bootstrap es un [Framework](https://es.wikipedia.org/wiki/Framework) de [HTML](https://developer.mozilla.org/es/docs/Glossary/HTML), [CSS](https://developer.mozilla.org/es/docs/Glossary/CSS) y [JS](https://developer.mozilla.org/es/docs/Glossary/JavaScript) para implementar [diseño web adaptable](https://es.wikipedia.org/wiki/Dise%C3%B1o_web_adaptable). Es una opción entre varias que se podrían explorar: [Top 10 Front-End Frameworks of 2016](https://www.keycdn.com/blog/front-end-frameworks/), [Best Front-end frameworks to try in 2016](https://hashnode.com/post/best-front-end-frameworks-to-try-in-2016-cin1unmcn00tvrb535out1y08). Optar por Bootstrap es optar por lo más popular, por asegurarse disponibilidad de mucha ayuda en línea.

Sin más preámbulo, vamos al [sitio oficial de Bootstrap](http://getbootstrap.com). En el menú busquen la opción **customize** (quien esté usando Safari podrían tener problemas, le recomiendo el uso de otro navegador). En la página customize encontrarán muchas opciones que revisaremos más adelante. Por ahora avancen hasta el final de la página y presionen el botón: **Compile and Download**. Con esa descarga obtendrán la siguiente carpeta:

```
bootstrap/
├── config.json
├── css/
│   ├── bootstrap.css
│   ├── bootstrap.min.css
│   ├── bootstrap-theme.css
│   └── bootstrap-theme.min.css
├── fonts/
│   ├──  glyphicons-halflings-regular.eot
│   ├──  glyphicons-halflings-regular.svg
│   ├──  glyphicons-halflings-regular.ttf
│   └──  glyphicons-halflings-regular.woff
└── js/
    ├── bootstrap.js
    └── bootstrap.min.js
```

Podemos eliminar algunos documentos, porque, por el momento, sólo necesitamos: 

```
bootstrap/
├── config.json
├── css/
│   └── bootstrap.min.css
├── fonts/
│   ├──  glyphicons-halflings-regular.eot
│   ├──  glyphicons-halflings-regular.svg
│   ├──  glyphicons-halflings-regular.ttf
│   └──  glyphicons-halflings-regular.woff
└── js/
    └── bootstrap.min.js
```

Ahora vamos a otro sitio web: [http://jquery.com](http://jquery.com), para descargar **the compressed, production jQuery 3.2.0**. El código que descarguen, debe:

- renombrarse “jquery.min.js”
- incluirse en la carpeta “js”, dentro de “bootstrap”. 

Con eso queda:

```
bootstrap/
├── config.json
├── css/
|   └── bootstrap.min.css
├── fonts/
|   ├── glyphicons-halflings-regular.eot
│   ├── glyphicons-halflings-regular.svg
│   ├── glyphicons-halflings-regular.ttf
│   └── glyphicons-halflings-regular.woff
└── js/
    ├── bootstrap.min.js
    └── jquery.min.js
```

Ya podemos abrir la carpeta como un nuevo proyecto en [Atom](https://atom.io/). Lo primero que haremos en este editor será crear:

- un documento `index.html`
- un documento `style.css`
- una carpeta `images`

En el documento `index.html` tenemos que escribir: 

```
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Hola mundo!</title>
<link href="css/bootstrap.min.css" rel="stylesheet">
<link href="style.css" rel="stylesheet">
<!--[if lt IE 9]>
<script src="https://oss.maxcdn.com/html5shiv/3.7.2/html5shiv.min.js"></script>
<script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
<![endif]-->
</head>
<body>
<h1>Hola mundo!</h1>
<script src="js/jquery.min.js"></script>
<script src="js/bootstrap.min.js"></script>
</body>
</html>
```

El documento `style.css` y la carpeta `images` pueden quedar vacías por ahora. Esto es lo básico para comenzar a trabajar con Bootstrap:

```
bootstrap/
├── config.json
├── css/
|   └── bootstrap.min.css
├── fonts/
|   ├──  glyphicons-halflings-regular.eot
│   ├──  glyphicons-halflings-regular.svg
│   ├──  glyphicons-halflings-regular.ttf
│   └──  glyphicons-halflings-regular.woff
├── images/
├── index.html
└── js/
│   ├── bootstrap.min.js
│   └── jquery.min.js
└── style.css
```

#### Al trabajar con Bootstrap nos conviene recordar que: 

- puedes "tomar" hasta 12 columnas (`col-`) en una fila (`row`), las columnas que tomes hacen el ancho de cada bloque;
- las filas (`row`) van dentro de contenedores, que pueden ser fijos (`container`) o fluidos (`container-fluid`).

#### También podemos aprovechar estas referencias:

- [Bootstrap Classes Reference](https://www.w3schools.com/bootstrap/bootstrap_ref_all_classes.asp)
- [Bootstrap 3 Cheat Sheet](https://www.cheatography.com/masonjo/cheat-sheets/bootstrap/)
- [CSS · Boostrap](http://getbootstrap.com/css/)
- [Components · Boostrap](http://getbootstrap.com/components/)
- [Javascript · Boostrap](http://getbootstrap.com/javascript/)

#### Si necesitamos más ayuda, podemos consultar algunos manuales:

- [Bootstrap 3, el manual oficial](https://librosweb.es/libro/bootstrap_3/)
- [Bootstrap 3 Tutorial](https://www.w3schools.com/bootstrap/)

## Aplicación

En este repositorio encuentras el prototipo de un sitio web. Trabajaremos sobre este sitio hasta armar uno propio, mientras vamos poniendo a prueba la "declaración de principios" de este [Framework](https://es.wikipedia.org/wiki/Framework) de [HTML](https://developer.mozilla.org/es/docs/Glossary/HTML), [CSS](https://developer.mozilla.org/es/docs/Glossary/CSS) y [JS](https://developer.mozilla.org/es/docs/Glossary/JavaScript):

> Bootstrap makes front-end web development faster and easier. 
> It's made for folks of all skill levels, devices of all shapes, and projects of all sizes.
