
![ejemplo](/images/pseudoclases.png "pseudoclases y pseudoelementos")

## Cuáles son las pseudoclases

Una pseudoclase define el estilo de **un estado** especial de un elemento.

- [Índice de pseudo-clases estándar](https://developer.mozilla.org/es/docs/Web/CSS/Pseudo-classes#indice_de_las_pseudo-clases_est%C3%A1ndar).

### Sintaxis

```css
selector:pseudoclase {
    propiedad: valor;
}
```

### :hover

Representa el estado en el cual **el cursor está encima del elemento**.

```css
a:hover {
    color: blue;
}
```

### :active

Representa el estado de un elemento que **está siendo activado** (es decir, cuando se hace clic en el elemento pero aún no se ha soltado el botón del mouse).

```css
button:active {
    background-color: green;
}
```

### :visited

Representa el estado de un enlace que **ya ha sido visitado**.

```css
a:visited {
    color: purple;
}
```

### :not()

Representa el estado en el cual **no coinciden los selectores que se indiquen**.

```css
input:not([type="submit"]) {
    border: 1px solid black;
}
```

### :nth-child()

Representa el estado en el cual **coinciden los hijos del elemento según el valor indicado**.

```css
ul li:nth-child(odd) {
    background-color: #f2f2f2;
}
```

## Cuáles son los pseudoselementos

Un pseudoelemento define el estilo de **una parte específica** de un elemento.

- [Lista de pseudo-elementos](https://developer.mozilla.org/es/docs/web/css/pseudo-elements#lista_de_pseudoelementos).

### Sintaxis

```css
selector::pseudo-elemento {
    propiedad: valor;
}
```

### ::before

Sirve para agregar un contenido **antes del elemento**. El contenido es agregado mediante la propiedad `content` de CSS.

```css
p::before {
    content: "Antes del texto: ";
    font-weight: bold;
}
```

### ::after

Sirve para agregar un contenido **después del elemento**. El contenido es agregado mediante la propiedad `content` de CSS.

```css
p::after {
    content: " Después del texto.";
    font-style: italic;
}
```

### ::first-letter

Sirve para añadir estilos a la **primera letra del texto** de cualquier elemento.

```css
p::first-letter {
    font-size: 200%;
    color: red;
}
```