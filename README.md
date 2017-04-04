# Bootstrap 3

Bootstrap es un Framework de HTML, CSS y JS para el desarrollo de proyectos web responsive. Es uno opción entre varias.

Sin más preámbulo, vamos a visitar [http://getbootstrap.com](http://getbootstrap.com). En el menú del sitio visitado busquen la página **customize** (quien esté usando Safari podrían tener problemas, recomiendo el uso de cualquier otro navegador –menos Safari– para realizar este paso). 

En customize de Bootstrap encontrarán muchas opciones que revisaremos más adelante. Por ahora avancen hasta el final de la página y presionen el botón: **Compile and Download**. Con esa descarga obtendrán la siguiente carpeta:

```bootstrap/
	├── config.json
	├── css/
	│   ├── bootstrap.css
	│   ├── bootstrap.min.css
	│   ├── bootstrap-theme.css
	│   └── bootstrap-theme.min.css
	├── fonts/
	│	  ├──  glyphicons-halflings-regular.eot
	│		├──  glyphicons-halflings-regular.svg
	│		├──  glyphicons-halflings-regular.ttf
	│		└──  glyphicons-halflings-regular.woff
	└── js/
			├── bootstrap.js
			└── bootstrap.min.js
```

Pero, de todo eso, sólo necesitamos: 

```bootstrap/
	├── config.json
	├── css/
	│   └── bootstrap.min.css
	├── fonts/
	│	  ├──  glyphicons-halflings-regular.eot
	│		├──  glyphicons-halflings-regular.svg
	│		├──  glyphicons-halflings-regular.ttf
	│		└──  glyphicons-halflings-regular.woff
	└── js/
			└── bootstrap.min.js
```

Visiten otro sitio web: [http://jquery.com](http://jquery.com) para descargar **the compressed, production jQuery 3.2.0**. El código que descarguen, debe:

- renombrarse “jquery.min.js” 
- incluirse en la carpeta “js”, dentro de la carpeta “bootstrap”. 

Con eso queda:

```bootstrap/
	├── config.json
	├── css/
	│   └── bootstrap.min.css
	├── fonts/
	│	  ├── glyphicons-halflings-regular.eot
	│		├── glyphicons-halflings-regular.svg
	│		├── glyphicons-halflings-regular.ttf
	│		└── glyphicons-halflings-regular.woff
	└── js/
			├── bootstrap.min.js
			└── jquery.min.js
```

Ahora corresponde pueden abrir la carpeta como un nuevo proyecto en Atom. En este editor crearemos: 

- un documento `index.html`
- un documento `style.css`
- una carpeta `images`

Con lo que acabos de crear, la carpeta debe verse así:

```
nombre_propio/
├── config.json
├── css/
|    └── bootstrap.min.css
├── fonts/
|    ├──  glyphicons-halflings-regular.eot
│    ├──  glyphicons-halflings-regular.svg
│    ├──  glyphicons-halflings-regular.ttf
│    └──  glyphicons-halflings-regular.woff
├── images/
├── index.html
└── js/
│    ├── bootstrap.min.js
│    ├── jquery.min.js
│    └── masonry.pkgd.min.js
└── style.css
```

Ahora vamos a fijarnos en el documento `index.html`, allí vamos a escribir: 

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
### Recursos:

…
