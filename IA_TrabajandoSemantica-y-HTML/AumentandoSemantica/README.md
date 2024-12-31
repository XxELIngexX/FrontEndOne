
[Aquí](https://github.com/alura-es-cursos/2090-IA-Generativa-en-el-Front.git) puedes descargar los archivos del proyecto que hemos avanzado hasta el aula anterior.

## 01: Aplicando semantica en las ofertas
[![Video 1](https://img.youtube.com/vi/MvXxyOb-cwo/0.jpg)](https://www.youtube.com/watch?v=MvXxyOb-cwo)

## 02: Para saber más: ¡la accesibilidad es importante!

Sabe, cuando hablamos de HTML semántico, estamos yendo mucho más allá de simplemente organizar un código. Estamos haciendo que la web sea un espacio más inclusivo, accesible y amigable para todos.

¿Por qué esto es tan importante? Bueno, piensa en las IAs generativas, por ejemplo. Ellas pueden ayudar en esto, ya que, cuando tenemos un código limpio y estructurado semánticamente, estas IAs pueden interpretar mejor el contenido, lo que puede ayudar a hacer que la web sea más inclusiva y accesible para todos.

Si deseas profundizar y obtener una comprensión más amplia sobre semántica y accesibilidad, no hay lugar mejor para comenzar que explorar los recursos ofrecidos por la WAI ARIA. La sigla ARIA (Accessible Rich Internet Applications) representa un enfoque notable para aumentar la accesibilidad del contenido web para personas con discapacidades, mediante la implementación de tecnologías asistivas.

Algunas fuentes y bibliografía que recomiendo:

- **W3C's WAI-ARIA Overview:** Es el punto de partida. Aquí, tendrás una visión general completa y directa de la fuente.

- **MDN Web Docs on HTML5 Semantics:** Mozilla siempre brilla con sus recursos, y esta sección sobre semántica HTML5 no es una excepción. Explicaciones claras, ejemplos y una visión general sólida de lo que es importante.

- **WebAIM:** Un recurso fantástico para accesibilidad en la web. Aquí encontrarás artículos, herramientas y entrenamientos.

- **"HTML5 - Designing Rich Internet Applications" por Matthew David:** Un buen libro que cubre el poder del HTML5, con un enfoque especial en semántica y diseño.

- **"Inclusive Design Patterns - Coding Accessibility Into Web Design" por Heydon Pickering:** Una lectura esencial si quieres entender cómo el diseño inclusivo y la accesibilidad se cruzan.

Recuerden: la web fue hecha para todos. Cuanto más aprendamos y apliquemos estos conceptos, más podremos contribuir a hacer de Internet un lugar mejor y más inclusivo.

```
Y solo para recordar, estoy aquí para ayudar y charlar. ¡Así que no dejen de profundizar y echar un vistazo a estas referencias!
```

## 03. cuestionario: HTML semántico para la accesibilidad

Estás refactorizando una página web para mejorar el acceso y la experiencia de usuarios con discapacidades visuales. La semántica HTML es esencial para satisfacer estas necesidades, ya que las etiquetas correctas proporcionan información sobre la estructura de la página.

Basado en este contexto, evalúa el código abajo y selecciona qué etiqueta sugieres para reemplazar las `divs` de modo a mejorar la semántica HTML y la accesibilidad en la web?

   - [ ] codigo:
  ```html
<header>...
    <div class="nav">...</div>
</header>
<main>...</main>
<div class="footer">...</div>
```
   - [ ] codigo:
```html 
<div class="header">
       <nav>...</nav>
   </div>
   <article>...</article>
   <div class="footer">...</div> 
```
   - [x] codigo:
```html 
<header class="header">
    <nav>...</nav>
</header>
<main>...</main>
<footer>...</footer>
```

```
Esta mejora la semántica HTML, ya que cambia las `divs` por etiquetas que especifican el papel de estas secciones en la estructura de la página.
```

  - [ ] codigo:
  ```html
<div class="header">
    <nav>...</nav>
</div>
<div class="main-content">...</div>
<div class="footer">...</div>
  ```





## 04. Haga lo que hicimos

En el diseño actual, todo el contenido está contenido en `divs` sin mucho significado semántico. Tu tarea es ayudar a Jornada a reformular el código de su página de ofertas para hacerlo más comprensible para los motores de búsqueda y las tecnologías de asistencia.


## 4.1: Opinión del instructor

La estructura semántica de un documento HTML permite una mejor accesibilidad en la web y optimización para motores de búsqueda. La semántica también proporciona un medio para que los navegadores y otras tecnologías web entiendan el significado de las etiquetas y su contenido.

En esta tarea, necesitas reemplazar las etiquetas `div` por etiquetas más semánticas.

Por ejemplo, el elemento principal `<main>`, donde se contiene el contenido principal del cuerpo de un documento o aplicación, debe usarse una vez por página.

Además, el contenido de la tarjeta de oferta podría estar encapsulado dentro de una `<section>`, representando un bloque de contenido relacionado; la `<header>` para representar una introducción al contenido de la tarjeta; y el nombre del destino podría mostrarse con un título `<h2>`.

Por último, la acción de ver detalles, que antes se colocaba en un `<span>`, puede expresarse mejor como una <a>, indicando una acción del usuario para ir a otra página con detalles de la oferta.

```
<main class="container">
    <div class="ofertas">
        <!-- ... -->
        <div class="ofertas__cards">
            <div class="ofertas__cards--grupo">
                <div class="ofertas__cards--elemento ofertas__cards--japon">
                    <div class="ofertas__card">
                        <!-- ... -->
                        <div class="ofertas__card--destino">
                            <div class="ofertas__card--destino-tipo">HOTEL+AÉREO</div>
                            <b class="ofertas__card--destino-nombre">Japón</b>
                        </div>
                        <!-- ... -->
                    </div>
                </div>
                <!-- ... -->
            </div>
            <!-- ... -->
        </div>
    </div>
</main>
```
Dejo el [Github](https://github.com/alura-es-cursos/2090-IA-Generativa-en-el-Front.git) para que puedas echar un vistazo a cómo lo hicimos.

## 05: Lo que aprendimos
Lo que aprendimos en esta aula:

- **Convertir divs genéricas a secciones:** Se cambió la etiqueta `<div>` con la clase "ofertas" a la etiqueta semántica `<section>`. Este cambio indica claramente que el contenido interno representa una sección cohesiva del contenido, haciendo que el código sea más accesible y semánticamente correcto;

- **Usar títulos semánticos:** El nombre del destino, anteriormente marcado como un elemento `<b>`, fue convertido a un elemento de título `<h2>`. Esto no solo proporciona mayor énfasis visual y semántico, sino que también ayuda a las tecnologías de asistencia (como lectores de pantalla) a identificar y navegar el contenido;

- **Convertir divs a enlaces:** La acción "Ver detalles" fue convertida de un `<span>` a un `<a>`, convirtiéndola así en un enlace navegable. Este es un cambio crucial en términos de accesibilidad, ya que permite a los usuarios hacer clic en el enlace y potencialmente navegar a una página de detalles;

- **Refuerzo de la estructura semántica:** La estructura semántica fue reforzada al reemplazar divs genéricas por elementos semánticos en varias áreas del código. Por ejemplo, la etiqueta `<section>` se utilizó para agrupar cada elemento de oferta, indicando que cada elemento representa una sección distinta del contenido.

