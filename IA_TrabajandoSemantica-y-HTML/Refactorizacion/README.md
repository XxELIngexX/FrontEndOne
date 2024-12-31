
[Aquí](https://github.com/alura-es-cursos/2090-IA-Generativa-en-el-Front.git) puedes descargar los archivos del proyecto que hemos avanzado hasta el aula anterior.

## 01: Refactorando el banner
[![Video 1](https://img.youtube.com/vi/LAc4G6TrYoU/0.jpg)](https://www.youtube.com/watch?v=LAc4G6TrYoU)

## 02: Etiquetas semánticas
[![Video 5](https://img.youtube.com/vi/se3Qq2xfRE0/0.jpg)](https://www.youtube.com/watch?v=se3Qq2xfRE0)

## 03: Desafio

Llegó tu turno de evolucionar un poquito más el sitio de la Jornada.

Mejora la semántica del banner y de las etiquetas principales. ¡Siéntete libre de usar tu IA Generativa favorita!

## 3.1: Opinión del instructor

¿Puedes darte cuenta de que los pequeños detalles marcan la diferencia?

Y hablando de pequeños detalles, [dejo el GitHub disponible](https://github.com/alura-es-cursos/2090-IA-Generativa-en-el-Front.git) para que puedas ver exactamente lo que hicimos en clase.

Observa que GitHub presenta con claridad todas las modificaciones realizadas, destacando lo que se eliminó y lo que se añadió, así como la línea correspondiente.

## 04. cuestionario: Encuentra la semántica correcta
Durante un café con tu colega desarrolladora, comenzaron a discutir sobre la refactorización del código HTML, agregando semántica y buenas prácticas. En la conversación, un tema que llamó la atención fue la forma adecuada de agregar semántica al HTML. Entonces, decidieron evaluar el siguiente código:
```
<div id="header">...</div>
<div id="main">...</div>
<div id="footer">...</div>
```

Considerando el contexto de buenas prácticas y semántica HTML, ¿cuál de las siguientes alternativas refactores correctamente este código en términos de semántica y es más fácil de ser interpretada tanto por personas como por mecanismos de búsqueda?

   - [ ] codigo:
  ```html
<div>...</div> 
<div>...</div> 
<div>...</div> 
```
   - [ ] codigo:
```html 
<top>...</top> 
<center>...</center> 
<bottom>...</bottom> 
```
   - [ ] codigo:
```html 
<head>...</head> 
<body>...</body> 
<base>...</base>
```
  - [x] codigo:
  ```html
  <header>...</header>
  <main>...</main>
  <footer>...</footer>
  ```


```
El código HTML fue enriquecido con elementos semánticos que representan la estructura de la página: `header`, `main` y `footer`. Estas son etiquetas semánticas HTML5 que ayudan a describir la forma del contenido de la página.
```

## 05: Lo que aprendimos

Lo que aprendimos en esta aula:

- Utilizar etiquetas semánticas, como `<header>`, `<section>` y `<main>`, para estructurar y dar significado al contenido;

- Describir las imágenes de manera adecuada, cambiando el atributo alt de la imagen para proporcionar una descripción más detallada ("Imagen de las Maldivas");

- Utilizar `<figure>` y `<figcaption>` para implementar la combinación de etiquetas `<figure>` y `<figcaption>`, asociando una imagen con su respectiva descripción y mejorando la semántica y accesibilidad;

- Realizar una estructuración consistente, ya que la conversión de divisiones genéricas (`<div>`) a elementos semánticos hace que la estructura sea más consistente, facilitando la interpretación por parte de lectores y navegadores.

