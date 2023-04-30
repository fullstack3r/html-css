## Qué es una declaración de CSS

Una declaración de CSS es un bloque que especifica el conjunto de estilos que se añadirán a un elemento HTML. Su estructura contiene lo siguiente:

- **Selector**: define el elemento o conjunto de elementos a los cuales se añadirán los estilos.
- **Propiedad**: es el nombre del estilo de CSS.
- **Valor**: es el valor que tomará la propiedad.

Ejemplo:

```css
h1 {
  color: red;
  font-size: 32px;
}
```
En este ejemplo, `h1` es el selector, `color` y `font-size` son las propiedades, y `red` y `32px` son los valores.

## Qué son comentarios de CSS

Los comentarios de CSS consisten en señalar algo que se ignorará. Para establecer un comentario CSS se lo envuelve entre `/*` y `*/`, independiente de la cantidad de líneas.

Ejemplo:

```css
/* Este es un comentario de una línea */
/*
Este es un comentario de varias líneas
*/
```

## Propiedades iniciales de CSS

Antes de empezar con CSS utilizaremos algunas propiedades de CSS.

- `color`: establece el color del texto de un elemento.
- `background-color`: establece un color de fondo al elemento.
- `font-size`: establece el tamaño de la fuente.
- `width`: establece la anchura de un elemento.
- `height`: establece la altura de un elemento.

Ejemplo:

```css
p {
  color: blue;
  background-color: yellow;
  font-size: 16px;
  width: 200px;
  height: 100px;
}
```

## Medidas iniciales

Estas son las medidas iniciales que debes conocer para establecer tamaños de elementos o de tipografía:

- `px`: establece una longitud de píxeles.
- `%`: establece un porcentaje con respecto a una medida base.

Ejemplo:

```css
p {
  font-size: 24px;
}

h1 {
  font-size: 200%;
}
```
----


## Cuáles son los selectores básicos

Un selector básico es la mínima expresión CSS para colocar estilos.

```
selector {
    /* Estilos */
}

```

### 1. Selector de tipo

Selecciona todos los elementos que coincidan con el **nombre de la etiqueta HTML**.

```
div {
    /* Todos los div en el documento */
}

```

### 2. Selector de clase

Selecciona todos los elementos que coincidan con las etiquetas HTML que **contengan el atributo `class`**.

```
<!--archivo HTML-->
<div class="card"> Soy una carta </div>
```

Para seleccionar estos elementos, se empieza por un punto `.` y seguido el **valor exacto** del atributo `class` de la etiqueta. Puede ser cualquier valor que desees colocar.

```
/* archivo CSS */
.card {
    /* Todas las etiquetas con la clase "card" */
}

```

Puede existir más de un valor dentro del atributo `class` separados por espacios.

```
<!--archivo HTML-->
<div class="card card1"> Soy una carta </div>
<div class="card card2"> Soy una carta </div>

```

```
.card {
    /* Todas las etiquetas con la clase "card" */
}

.card1 {
    /* Todas las etiquetas con la clase "card1" */
}

.card2 {
    /* Todas las etiquetas con la clase "card2" */
}

```

### 3. Selector de identificador único (id)

Selecciona el único elemento que coincida con la etiqueta HTML que **contenga el atributo `id`**. Solo puede existir un valor `id` para todo el documento.

```
<!--archivo HTML-->
<button id="eliminar"> Eliminar  </button>

```

Para seleccionar el elemento, se empieza por el símbolo de *hashtag* `#` y seguido el **valor exacto** del atributo `id` de la etiqueta. Puede ser cualquier valor que desees colocar.

```
/* archivo CSS */
#eliminar {
    /* La única etiqueta con el id "eliminar" */
}

```

### 4. Selector de atributo

Selecciona los elementos que coincidan con la etiqueta HTML que **contenga el atributo y valor** especificado.

```
<!--archivo HTML-->
<a href="https://disrup3.com"> Ir a disrup3</a>

```

Para seleccionar los elementos, se empieza por el nombre de la etiqueta, seguido de corchetes `[]` que contiene el atributo y valor especificado.

```
/* archivo CSS */
a[href=""https://disrup3.com"] {
    /* Todas las etiquetas <a> con una propiedad href con valor "https://disrup3.com" */
}

```

### 5. Selector universal

Selecciona todos los elementos del documento mediante un asterisco `*`.

```
* {
    /* Todos los elementos */
}

```
-----

## Selectores combinadores en CSS

Un selector combinador es la unión de dos o más selectores básicos.

```css
selector1 selector2 selector3 {
    /* Estilos */
}
```

### 1. Combinador de descendientes

Selecciona todos los elementos del selector de la derecha que son **hijos** del selector de la izquierda, **independientemente de la profundidad**. Estos selectores están separados por un espacio.

```css
padre hijos {
    /* Todos los hijos del padre */
}

div p {
    /* Todos los <p> hijos de <div> */
}

.container img {
    /* Todos los <img> hijos de la clase "container" */
}
```

### 2. Combinador de hijo directo

Selecciona todos los elementos del selector de la derecha que son **hijos directos** del selector de la izquierda. Estos selectores están separados por `>`.

```css
padre > hijos_directos {
    /* Todos los hijos directos del padre */
}

div > p {
    /* Todos los <p> hijos directos de <div> */
}

.container > img {
    /* Todos los <img> hijos directos de la clase "container" */
}
```

### 3. Combinador de elemento adyacente

Selecciona todos los elementos del selector de la derecha que están **adyacentes** al selector de la izquierda. Estos selectores están separados por `+`.

```css
elemento + adyacente {
    /* Elementos adyacentes */
}

div + p {
    /* Todos los <p> adyacentes a <div> */
}

.container + img {
    /* Todos los <img> adyacentes a la clase "container" */
}
```

**Adyacente significa que comparten el mismo padre y están situados inmediatamente hacia abajo de otro elemento**. Por ejemplo, en el siguiente código:

```html
<!--archivo HTML -->
<h1>Soy un título </h1>
<div>Soy un div</div>
<p>Soy un párrafo</p>
```

`<div>` está adyacente a `<h1>` y `<p>` está adyacente a `<div>`. Sin embargo, `<h1>` no está adyacente a `<div>` y `<div>` no está adyacente a `<p>`.

### 4. Combinador general de hermanos

Selecciona todos los elementos del selector de la derecha que son **hermanos** del selector de la izquierda. Estos selectores están separados por `~`.

```css
elemento ~ hermanos {
    /* Elementos hermanos */
}

div ~ p {
    /* Todos los <p> hermanos de <div> */
}

.container ~ img {
    /* Todos los <img> hermanos de la clase "container" */
}
```

**Hermanos significa que comparten el mismo padre y están situados hacia abajo de otro elemento**. Por ejemplo, en el siguiente código:

```html
<!--archivo HTML -->
<h1>Soy un título </h1>
<div>Soy un div</div>
<p>Soy un párrafo</p>
```

`<div>` y `<p>` son hermanos de `<h1>`, pero `<h1>` no es hermano de `<div>` y `<p>`.
