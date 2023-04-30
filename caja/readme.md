![ejemplo](/images/padding.png "pseudoclases y pseudoelementos")
# Modelo de caja en HTML y CSS

El modelo de caja en HTML y CSS es una estructura rectangular que comprende cuatro elementos principales: margen, borde, relleno y contenido. A continuación se explica cada uno de estos elementos:

## Contenido

El contenido se refiere a todo lo que está dentro del elemento HTML y su tamaño se establece con las propiedades `width` y `height`.

## Borde

El borde es el perfil o borde del elemento HTML. Su apariencia puede ser personalizada utilizando las propiedades `border-color`, `border-style` y `border-width`.

## Relleno

El relleno es el espacio entre el borde y el contenido del elemento HTML. Este espacio se puede establecer utilizando la propiedad `padding`.

## Margen

El margen es el espacio entre el borde y otro elemento HTML. Este espacio se puede personalizar utilizando la propiedad `margin`.

Es posible establecer estos valores de manera individual o en cada posición del elemento utilizando las propiedades `margin-top`, `margin-right`, `margin-bottom`, `margin-left`, `padding-top`, `padding-right`, `padding-bottom`, `padding-left`, `border-top`, `border-right`, `border-bottom` y `border-left`.

Es importante tener en cuenta que el navegador establece valores por defecto a algunas propiedades CSS. Por lo tanto, se recomienda restablecer estos valores a `0` utilizando el selector universal `*`.

A continuación se presenta un ejemplo de cómo se puede calcular el tamaño total de un elemento a partir de la suma de los valores de las propiedades `border`, `padding` y `width` o `height`:

### Ejemplo

Si queremos establecer un elemento `div` con un borde rojo de 5 píxeles de ancho, un relleno de 10 píxeles, un margen de 15 píxeles y un ancho y alto de 100 píxeles, el código CSS se vería así:

```css
div {
    width: 100px;
    height: 100px;
    border: 5px solid red;
    padding: 10px;
    margin: 15px;
}
```

Esto resultaría en una caja de 150 píxeles de ancho y alto (100 píxeles de ancho y alto + 5 píxeles de borde a cada lado + 10 píxeles de relleno a cada lado + 15 píxeles de margen a cada lado).