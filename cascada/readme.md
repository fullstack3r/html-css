![ejemplo](/images/cascada.png "pseudoclases y pseudoelementos")

# Entendiendo la cascada y la especificidad en CSS

Cuando estás creando una página web, es común encontrarte con problemas relacionados a los estilos, tales como:

- ¿Por qué no se aplica el color que le estoy poniendo?
- ¿Por qué este elemento se comporta de manera diferente?

En la mayoría de los casos, se trata de un problema de **cascada o especificidad** en CSS.

## ¿Qué es la cascada en CSS?

La cascada es el concepto que determina **qué estilos se colocan sobre otros**, priorizando a aquellos que se encuentren más abajo en el código. De hecho, la palabra "cascade" proviene del nombre completo de CSS, que es "Cascading Style Sheets" (hojas de estilo en cascada).

Por ejemplo, si tenemos el siguiente código:

```css
h1 {
  color: red;
}

h1 {
  color: blue;
}
```

El elemento `<h1>` tendrá un color de letra azul, porque es el último estilo aplicado y se encuentra más abajo en el código. Esto ocurre con cada propiedad CSS que se repita en algún punto más arriba del código.

Puedes ver un ejemplo de cascada [aquí](https://codi.link/PGgxPkNhc2NhZGE8L2gxPg==%7CaDEgew0KICBjb2xvcjogcmVkOw0KfQ0KDQpoMSB7DQogIGNvbG9yOiBibHVlOw0KfQ==%7C).

## ¿Qué es la especificidad en CSS?

La especificidad en CSS consiste en dar un valor a una regla CSS sobre **qué tan específico es el estilo**. De esta forma, los navegadores pueden saber qué estilos aplicar sobre otros, independientemente de dónde se encuentren en el código. **El estilo se aplicará donde la especificidad sea mayor**.

### Tipos de especificidad en CSS

Existen 6 tipos de especificidad, donde `X` es la cantidad de estilos que lo contienen. Estos son:

| Selector           | Especificidad       |
| ------------------ | ------------------- |
| Estilo en línea     | `1000`              |
| Selector de ID     | `100`               |
| Selector de clase, atributo o pseudoclase | `10` |
| Selector de elemento o pseudoelemento | `1`   |
| Selector universal | `0`                 |

Cabe destacar que los selectores combinados suman la especificidad de cada selector básico para obtener la especificidad total de la regla CSS.

La palabra reservada `!important` es **un valor de toda propiedad CSS que provee una especificidad de `10000`**, por lo que se aplicará ante otros estilos. Sin embargo, esta es una mala práctica y no deberías utilizarla.

Si utilizas Visual Studio Code y mantienes el *mouse* sobre el selector, te mostrará la especificidad total. Además, puedes usar herramientas en línea como [Specificity Calculator](https://specificity.keegan.st/) para calcular la especificidad.

En resumen, es recomendable evitar los estilos en línea y el uso de `!important`, y en su lugar trabajar únicamente con la especificidad de los selectores. De esta forma, podrás crear estilos más limpios y mantenibles en tu sitio web.