# z-index

![ejemplo](/images/z-index.svg "pseudoclases y pseudoelementos")

Supongamos que tenemos un elemento de texto y una imagen superpuestos en la página HTML. Queremos que la imagen aparezca encima del texto, para que sea más visible. Para ello, podemos utilizar la propiedad z-index.

El código HTML para estos elementos podría ser el siguiente:

```html
<div class="contenedor">
  <p>Este es un texto de ejemplo.</p>
  <img src="ejemplo.jpg" alt="Ejemplo">
</div>
```

Para aplicar la propiedad z-index, primero necesitamos darle una posición a los elementos. Por ejemplo, podemos utilizar la posición "relative" para el contenedor y "absolute" para la imagen:

```css
.contenedor {
  position: relative;
}

.contenedor img {
  position: absolute;
  top: 0;
  left: 0;
}
```

Ahora podemos utilizar la propiedad z-index para cambiar el orden de apilamiento de los elementos. Si le asignamos un valor mayor a la imagen que al texto, la imagen se colocará encima del texto. Por ejemplo:

```css
.contenedor img {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 1;
}

.contenedor p {
  z-index: 0;
}
```

En este caso, la imagen tiene un z-index de 1 y el texto tiene un z-index de 0. Esto significa que la imagen se colocará encima del texto. Si quisiéramos que el texto se colocara encima de la imagen, podríamos intercambiar los valores de z-index.