
![ejemplo](/images/display.png "pseudoclases y pseudoelementos")


La propiedad `display` establece el **tipo de visualización de los elementos HTML sin afectar el flujo normal de los elementos**.

Existen etiquetas que por defecto tienen su `display` ya determinado, como la etiqueta `<div>` que tiene `display: block`, `<span>` tiene `display: inline` y `<button>` tiene `display: inline-block`.

A continuación, abordaremos los tipos de `display` `block`, `inline` e `inline-block`.

## Visualización en bloque (`block`)

El `display: block` establece que un elemento ocupará todo el espacio disponible por defecto y el siguiente elemento a este se situará por debajo. Es posible **añadir medidas** de anchura `width` y altura `height` a estos elementos. También es posible **agregar todas las propiedades del modelo de caja** (no te preocupes por este concepto, ya lo abordaremos).

## Visualización en línea (`inline`)

El `display: inline` establece que un elemento ocupará el espacio del contenido del mismo y el siguiente elemento se situará a la derecha. **No es posible añadir medidas** de anchura `width` y altura `height` a estos elementos. Además, **no es posible agregar todas las propiedades del modelo de caja, únicamente funcionará la propiedad `margin` en el eje horizontal** (no te preocupes por este concepto, ya lo abordaremos).

## Visualización de bloque y línea (`inline-block`)

El `display: inline-block` combina las ventajas de `block` de colocar medidas al elemento y propiedades del modelo de caja correctamente, con las ventajas de `inline` de colocar un elemento seguido de otro en el mismo espacio. Si el elemento excede el contenido total, se coloca en la siguiente línea por debajo.


## Visualización nula (`none`)

El `display: none` desactiva la visualización de un elemento, como si el elemento no existiera.

- [Ejemplos](https://codi.link/PGgyPlZpc3VhbGl6YWNpw7NuIGRlIGVsZW1lbnRvcyBlbiBIVE1MIHkgQ1NTPC9oMj4NCg0KPGRpdiBjbGFzcz0iYmxvY2siPg0KICAgIDxwPkVzdGUgZXMgdW4gZWplbXBsbyBkZSBlbGVtZW50byBjb24gZGlzcGxheSBibG9jay48L3A+DQo8L2Rpdj4NCg0KPHNwYW4gY2xhc3M9ImlubGluZSI+RXN0ZSBlcyB1biBlamVtcGxvIGRlIGVsZW1lbnRvIGNvbiBkaXNwbGF5IGlubGluZS48L3NwYW4+DQo8c3BhbiBjbGFzcz0iaW5saW5lIj5Fc3RlIGVzIG90cm8gZWplbXBsbyBkZSBlbGVtZW50byBjb24gZGlzcGxheSBpbmxpbmUuPC9zcGFuPg0KDQo8ZGl2IGNsYXNzPSJpbmxpbmUtYmxvY2siPg0KICAgIDxwPkVzdGUgZXMgdW4gZWplbXBsbyBkZSBlbGVtZW50byBjb24gZGlzcGxheSBpbmxpbmUtYmxvY2suPC9wPg0KPC9kaXY+DQoNCjxkaXYgY2xhc3M9ImlubGluZS1ibG9jayI+DQogICAgPHA+RXN0ZSBlcyBvdHJvIGVqZW1wbG8gZGUgZWxlbWVudG8gY29uIGRpc3BsYXkgaW5saW5lLWJsb2NrLjwvcD4NCjwvZGl2Pg0KDQo8ZGl2IGNsYXNzPSJub25lIj4NCiAgICA8cD5Fc3RlIGVzIHVuIGVqZW1wbG8gZGUgZWxlbWVudG8gY29uIGRpc3BsYXkgbm9uZS48L3A+DQo8L2Rpdj4NCiANCiA8aW1nIHNyYz0iaHR0cHM6Ly9yYXcuZ2l0aHVidXNlcmNvbnRlbnQuY29tL2Z1bGxzdGFjazNyL2h0bWwtY3NzL21haW4vaW1hZ2VzL2Rpc3BsYXkucG5nP3Rva2VuPUdIU0FUMEFBQUFBQUJaSFJDNVhCVUhBR1dCMkZGREtNUUFTWkNPNUlRUSI+%7CLmltZ1N0eWxlIHsNCiAgICAgICAgZGlzcGxheTogYmxvY2s7DQogICAgICAgIHRleHQtYWxpZ246IGNlbnRlcjsNCiAgICB9DQogICAgLmltZ1N0eWxlIGltZyB7DQogICAgICAgIHdpZHRoOiAzMCU7DQogICAgfQ0KICAgIGJvZHkgew0KICAgICAgICBiYWNrZ3JvdW5kLWNvbG9yOiAjMTExOw0KICAgICAgICBjb2xvcjogI2ZmZjsNCiAgICB9DQoNCiAgICAvKiBFamVtcGxvIGRlIGRpc3BsYXkgZW4gSFRNTCB5IENTUyAqLw0KDQogICAgLyogRXN0aWxvcyBwYXJhIGxvcyBlbGVtZW50b3MgY29uIGRpc3BsYXkgYmxvY2sgKi8NCiAgICAuYmxvY2sgew0KICAgICAgICBkaXNwbGF5OiBibG9jazsNCiAgICAgICAgYmFja2dyb3VuZC1jb2xvcjogIzFmMTk3ZDsNCiAgICAgICAgd2lkdGg6IDIwMHB4Ow0KICAgICAgICBoZWlnaHQ6IDEwMHB4Ow0KICAgICAgICBtYXJnaW4tYm90dG9tOiAyMHB4Ow0KICAgIH0NCg0KICAgIC8qIEVzdGlsb3MgcGFyYSBsb3MgZWxlbWVudG9zIGNvbiBkaXNwbGF5IGlubGluZSAqLw0KICAgIC5pbmxpbmUgew0KICAgICAgICBkaXNwbGF5OiBpbmxpbmU7DQogICAgICAgIGJhY2tncm91bmQtY29sb3I6ICM0Zjc1MWI7DQogICAgICAgIG1hcmdpbi1yaWdodDogMjBweDsNCiAgICB9DQoNCiAgICAvKiBFc3RpbG9zIHBhcmEgbG9zIGVsZW1lbnRvcyBjb24gZGlzcGxheSBpbmxpbmUtYmxvY2sgKi8NCiAgICAuaW5saW5lLWJsb2NrIHsNCiAgICAgICAgZGlzcGxheTogaW5saW5lLWJsb2NrOw0KICAgICAgICBiYWNrZ3JvdW5kLWNvbG9yOiAjZDgxYzNkOw0KICAgICAgICB3aWR0aDogMTAwcHg7DQogICAgICAgIGhlaWdodDogMTAwJTsNCiAgICAgICAgbWFyZ2luLXJpZ2h0OiAyMHB4Ow0KICAgICAgICBtYXJnaW4tYm90dG9tOiAyMHB4Ow0KICAgIH0NCg0KICAgIC8qIEVzdGlsb3MgcGFyYSBsb3MgZWxlbWVudG9zIGNvbiBkaXNwbGF5IG5vbmUgKi8NCiAgICAubm9uZSB7DQogICAgICAgIGRpc3BsYXk6IG5vbmU7DQogICAgfQ0KDQoNCg==%7C)

----

¡Claro! Aquí te dejo una descripción en Markdown:

# Ejemplos de uso de Flexbox y Grid

El `display: flex` y `display: grid` son herramientas muy útiles en el desarrollo de interfaces web amigables y adaptables a diferentes dispositivos. A continuación se presentan algunos ejemplos de cómo utilizar estas propiedades en CSS:

## Ejemplo de Flexbox

El siguiente código HTML crea un contenedor padre con la propiedad `display: flex` y ordena sus elementos hijos en una sola línea horizontal:

```html
<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
</div>
```

```css
.container {
  display: flex;
}

.item {
  padding: 10px;
  margin: 5px;
  background-color: #eee;
}
```


## Ejemplo de Grid

El siguiente código HTML crea un contenedor padre con la propiedad `display: grid` y define dos columnas y tres filas para organizar sus elementos hijos:

```html
<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
  <div class="item">Item 4</div>
  <div class="item">Item 5</div>
  <div class="item">Item 6</div>
</div>
```

```css
.container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 50px 50px 50px;
  grid-gap: 10px;
}

.item {
  padding: 10px;
  background-color: #eee;
}
```

## Uso combinado de Flexbox y Grid

¡Claro! Aquí te proporciono un ejemplo de cómo combinar Flexbox y Grid para crear una interfaz de usuario responsive y atractiva:

```html
<div class="container">
  <div class="header">Header</div>
  <div class="sidebar">Sidebar</div>
  <div class="main">
    <div class="content">Content 1</div>
    <div class="content">Content 2</div>
    <div class="content">Content 3</div>
    <div class="content">Content 4</div>
    <div class="content">Content 5</div>
  </div>
  <div class="footer">Footer</div>
</div>
```

```css
.container {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: auto 1fr auto;
  grid-template-areas:
    "header header header header"
    "sidebar main main main"
    "footer footer footer footer";
}

.header {
  grid-area: header;
}

.sidebar {
  grid-area: sidebar;
}

.main {
  display: flex;
  flex-wrap: wrap;
  grid-area: main;
  gap: 10px;
  justify-content: space-between;
}

.content {
  flex: 0 0 calc(33.33% - 10px);
}

.footer {
  grid-area: footer;
}
```

Este ejemplo utiliza Flexbox para distribuir los elementos dentro del contenedor `main`, y Grid para posicionar los demás elementos en el layout. La propiedad `flex-wrap` en `.main` permite que los elementos se distribuyan en varias filas si no caben en una sola fila. 

Este es solo un ejemplo básico, pero la combinación de Flexbox y Grid ofrece muchas posibilidades para la creación de interfaces de usuario avanzadas y adaptativas.
 
