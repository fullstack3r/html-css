# HTML Semántico

El HTML semántico consiste en etiquetar cada elemento de la página con una etiqueta que lo defina correctamente y tenga un significado semántico claro. 

## El problema con la etiqueta `div`

La etiqueta `div` define un bloque genérico de contenido que no tiene ningún valor semántico. Se utiliza principalmente para elementos de diseño como contenedores. Sin embargo, su uso excesivo no es recomendado, ya que no proporciona información útil sobre el contenido de la página.

```html
<div class="container">
  <h1>Título</h1>
  <p>Este es un párrafo de texto.</p>
</div>
```

## Etiquetas semánticas

A continuación se muestran algunas etiquetas semánticas comúnmente utilizadas en la definición de una interfaz web:

- `<header>`: define el encabezado de la página (no confundir con `<head>`).
```html
<header>
  <h1>Título del encabezado</h1>
</header>
```
- `<nav>`: define una barra de navegación que incluye enlaces.
```html
<nav>
  <ul>
    <li><a href="#">Inicio</a></li>
    <li><a href="#">Sobre nosotros</a></li>
    <li><a href="#">Contacto</a></li>
  </ul>
</nav>
```
- `<section>`: define una sección de la página.
```html
<section>
  <h2>Sección principal</h2>
  <p>Este es un párrafo de texto en la sección principal.</p>
</section>
```
- `<footer>`: define un pie de página o de sección.
```html
<footer>
  <p>Derechos de autor © 2023. Todos los derechos reservados.</p>
</footer>
```
- `<article>`: define un artículo, el cual puede tener su propio encabezado, navegación, sección o pie de página.
```html
<article>
  <header>
    <h2>Título del artículo</h2>
    <p>Publicado por John Doe</p>
  </header>
  <section>
    <p>Este es el contenido del artículo.</p>
  </section>
  <footer>
    <p>Comentarios (3)</p>
  </footer>
</article>
```

## Ventajas de utilizar HTML semántico

Las ventajas de utilizar HTML semántico son:

- Ayuda a tu sitio a ser accesible
- Mejora tu posicionamiento (SEO)
- Código más claro, legible y mantenible
- Ayuda a buscadores (como Google) a encontrar tu página

## Conclusión

El uso de etiquetas semánticas en HTML puede mejorar significativamente la calidad del código y la accesibilidad de la página web. Es importante evitar el uso excesivo de la etiqueta `div` y utilizar etiquetas semánticas adecuadas para cada elemento de la página.