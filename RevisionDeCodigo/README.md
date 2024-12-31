# FrontEndOne

# Proyecto FrontEnd

Este es un proyecto de FrontEnd donde incluyo un video explicativo:


Aquí están los dos videos que quiero compartir:

## 01: Empezando el proyecto
[![Video 1](https://img.youtube.com/vi/8YcTACliQn4/0.jpg)](https://www.youtube.com/watch?v=8YcTACliQn4)

## 02: empezando el proyecto
[![Video 2](https://img.youtube.com/vi/7o9b3gkCA0E/0.jpg)](https://www.youtube.com/watch?v=7o9b3gkCA0E)

## 04: Para saber mas (lectura recomendada)

[CSS y el Patrón BEM](./markdowns/CSS-y-PatronBEM.md).

## 05: Luri y la primera refactorización del código

[![Video 3](https://img.youtube.com/vi/lwOv1DydPGM/0.jpg)](https://www.youtube.com/watch?v=lwOv1DydPGM)

## 06. cuestionario: Semántica HTML en Accesibilidad

¿Cómo aplicarías la semántica del HTML para mejorar la accesibilidad de un sitio web?

1. ¿Te parece útil el patrón BEM?
   - [ ] Las etiquetas semánticas deben usarse con cuidado, ya que pueden dificultar la carga del sitio.
   - [ ] Usaría solo elementos `<div>` en todo mi código para garantizar flexibilidad en el diseño.
   - [ ] La utilización de elementos HTML semánticos ayuda en la accesibilidad y es una buena práctica que mejora los resultados de SEO.
   - [x] Los elementos `<div>` no agregan ninguna semántica al código. La accesibilidad y el SEO se mejoran cuando se usan elementos HTML semánticos.
         
```
Utilizaría etiquetas semánticas como `<header>`, `<nav>`, `<main>`, `<footer>` correctamente para describir significado y contenido, ayudando a lectores de pantalla y mejorando los resultados de SEO.
```

## 08. Desafío: principios de la semántica HTML - Navegación
La agencia de viajes "Jornada" está reformulando su sitio web para mejorar la experiencia de sus usuarios. El equipo de desarrollo web de Jornada ha estado trabajando arduamente para asegurar que la refactorización del código sea accesible y siga las mejores prácticas de HTML semántico. Sin embargo, se han encontrado con un problema: la navegación principal del sitio web no es clara y no sigue los estándares de semántica HTML y accesibilidad.

Tu desafío será ayudar al equipo a refactorizar su código HTML para hacerlo más accesible y semántico.
Código base HTML:

```
<a>
  <img class="encabezado__logo--icono" alt="" src="./img/logoproviblanca-1@2x.png" />
</a>
<div class="encabezado__navegacion">
  <a class="encabezado__navegacion--elemento" href="">Blog</a>
  <a class="encabezado__navegacion--elemento" href="">Paquete de viaje</a>
  <a class="encabezado__navegacion--elemento" href="">Contacto</a>
</div>
```

Espero que eso ayude al equipo de "Jornada" a mejorar la accesibilidad y semántica de su sitio web.

## 8.1 Opinión del instructor
El código debe ser refactorizado para incluir una etiqueta de navegador HTML que represente la navegación principal y una lista no ordenada para los elementos de navegación. Además, la imagen del encabezado debe tener un texto alternativo apropiado para la accesibilidad.

```
<img class="encabezado__logo--icono" alt="Logo de la Jornada" src="./img/logoproviblanca-1@2x.png" />
</a>
<nav class="encabezado__navegacion" role="navigation" aria-label="Navegación principal">
  <ul class="encabezado__navegacion--lista">
    <li class="encabezado__navegacion--elemento">
      <a href="">Blog</a>
    </li>
    <li class="encabezado__navegacion--elemento">
      <a href="">Paquetes de viaje</a>
    </li>
    <li class="encabezado__navegacion--elemento">
      <a href="">Contacto</a>
    </li>
  </ul>
</nav>
```

Y el CSS:

```
.encabezado__navegacion--lista {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
}

.encabezado__navegacion--elemento a {
    /** demás estilos omitidos, solo ajustamos el selector */
}
```

Otra forma interesante de seguir el estilo que yo utilicé es echando un vistazo [aquí en Github](https://github.com/alura-es-cursos/2090-IA-Generativa-en-el-Front.git).

## 09: Lo que aprendimos

Lo que aprendimos en esta aula:

- Utilizar atributos alt significativos para imágenes, proporcionando una descripción precisa para lectores de pantalla;
- Aplicar la etiqueta `<nav>` para destacar la navegación principal del sitio;
- Implementar listas (`<ul>` y `<li>`) para representar estructuralmente elementos de navegación, que es estándar para menús;
- Aplicar atributos ARIA (`role` y `aria-label`) para mejorar la accesibilidad y proporcionar contextos adicionales para lectores de pantalla.
