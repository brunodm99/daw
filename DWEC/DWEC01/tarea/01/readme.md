# Unidad de Trabajo 1: Arquitecturas y Lenguajes de Programación en Clientes Web

 Ejemplo 1. Integración del código JavaScript en HTML.
```
<!DOCTYPE html>
<html>
<title>Myfpschool</title>
<head>

<script>
 function diAlgo()
 {
     alert("Hola");
 }
</script>

</head>
<body>

<script>
diAlgo();
</script>

</body>
</html>
```

### Práctica 1. a) Modifica el código para colocar el script en el body. b) Modifica el código para que el script se encuentre externamente en un archivo de extensión “.js”.
```
<!DOCTYPE html>
<html>
<body>

<h1>Modificando el código HTML</h1>

<p id="prueba">Modificando el contenido.</p>

<button type=”button”
onclick="document.getElementById('prueba').innerHTML = 'CAMBIANDO el contenido!'">
¡Dale!</button>

</body>
</html>
```

### Práctica 2. Añade otro botón que modifique de nuevo el contenido de la página.
```
<!DOCTYPE html>
<html>
<body>

<h1>Cambio de imágenes con JavaScript</h1>

<img id="myFPImage" onclick="cambiaPic()" src="http://myfpschool.com/wp-content/uploads/2016/06/myblack.jpeg" width="200" height="180">

<p>Haz click sobre la imagen para cambiarla.</p>

<script>
function cambiaPic() {
  var image = document.getElementById('myFPImage');
  if (image.src.match("green")) {
     image.src = "http://myfpschool.com/wp-content/uploads/2016/06/myblack.jpeg";
  } else {
     image.src = "http://myfpschool.com/wp-content/uploads/2016/06/mygreen.jpeg";
  }
}
</script>

</body>
</html>
```

### Práctica 3. Modifica ahora el código que alterne entre 3 imágenes diferentes a medida que el usuario haga click sobre las mismas. Puedes añadir una segunda condición empleando “else if(“condición”){“efecto”}”.
```
<!DOCTYPE html>
<html>
<body>
<p id="mytxt">Aprende JavaScript con MyFPSchool!</p>

<button type="button" onclick="myFunction()">¡Dale!</button>
<script>
function myFunction() {
  var x = document.getElementById("mytxt");
  x.style.fontSize = "25px";
  x.style.color = "red";
}
</script>
</body>
</html>
```

### Práctica 4. Elabora un cuestionario de 7 preguntas con dos botones cada una (verdadero/falso) de modo que el color del texto cambie a verde (acierto) o rojo (error). Para ello tendrás que escribir dos funciones (una para verdadero y otra para falso) y darle un valor de entrada function(x){“resultado”}.


### Práctica 5. Desarrolla una web sencilla con tres botones que permitan al usuario seleccionar entre tres idiomas (p.ej., español, francés e inglés). Modifica dichos botones para que al pulsarlos (onclick = “código javascript”) se genere una ventana de alerta con el texto “Bienvenido” en el idioma correspondiente y además, se imprima en la consola la selección del usuario (emplea el comando console.log(‘texto’)). Recuerda que puedes separar el código javascript mediante saltos de líneas pero también con ; en la misma línea.
