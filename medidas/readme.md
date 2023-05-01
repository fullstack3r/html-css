
# Unidades de medida en CSS

Las unidades de medida son una forma de establecer la longitud de un elemento o tipografía en una página web. Existen dos tipos de unidades de medida: absolutas y relativas.

## Unidades de medida absolutas

Las unidades de medida absolutas son valores fijos que no cambiarán en la pantalla. La unidad de medida absoluta más utilizada es el píxel (px), aunque existen otras unidades que también son poco comunes.

A continuación, se presentan algunas de las unidades de medida absolutas más utilizadas en CSS y su equivalencia en píxeles:

Unidad | Nombre | Equivalencia en píxeles
--- | --- | ---
px | Píxeles | 1 px = 1/96 in
cm | Centímetros | 1 cm = 96/2.54 px
mm | Milímetros | 1 mm = 1/10 cm
Q | Cuartos de milímetros | 1 Q = 1/4 mm
in | Pulgadas | 1 in = 2.54 cm = 96 px
pc | Picas | 1 pc = 1/6 in
pt | Puntos | 1 pt = 1/72 in

## Unidades de medida relativas

Las unidades de medida relativas son valores que dependen de otros factores externos, como el tamaño del elemento padre o las dimensiones de la pantalla del dispositivo. Estas unidades son útiles para crear diseños adaptables y responsivos.

A continuación, se presentan algunas de las unidades de medida relativas más utilizadas en CSS y su factor externo de referencia:

Unidad | Factor externo de referencia
--- | ---
em | Tamaño de la fuente del elemento que lo contiene
rem | Tamaño de la fuente del elemento raíz (la etiqueta html)
vw | Ancho de la pantalla en porcentaje (view width)
vh | Altura de la pantalla en porcentaje (view height)
vmin | El 1% de la dimensión más pequeña de la pantalla
vmax | El 1% de la dimensión más grande de la pantalla
ch | Anchura del carácter "0" del elemento que lo contiene
lh | Altura de línea del elemento que lo contiene

Es importante tener cuidado al utilizar unidades de medida relativas, ya que un pequeño cambio en su factor externo de referencia puede provocar cambios muy significativos en el tamaño del elemento.

### Diferencia entre rem y em

La unidad de medida "em" depende del tamaño de la fuente del elemento que lo contiene. Por ejemplo, si un elemento tiene un tamaño de fuente de 20px, el valor de 2em será igual a 40px.

Por otro lado, la unidad de medida "rem" depende del tamaño de la fuente del elemento raíz, que por defecto tiene un tamaño de 16px en la mayoría de los navegadores. Si cambiamos el tamaño de la fuente del elemento raíz a 10px (por ejemplo, para hacer más fácil el cálculo), entonces 2rem sería igual a 20px.

