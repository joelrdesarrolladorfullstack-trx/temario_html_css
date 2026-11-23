# Ejercicio: tarjeta de presentación

Una tarjeta centrada con nombre, profesión y una descripción. Junta varios temas de CSS:

| Qué | Cómo | Tema |
|-----|------|------|
| Fondo negro y texto blanco | `background-color: black; color: white;` en el `body` | [Colores](../css/Colores) |
| Tarjeta de 400px centrada | `width: 400px; margin: auto;` | [Width](../css/width%20y%20height) / [Margin](../css/padding%20y%20margin) |
| Texto centrado | `text-align: center;` | [Texto](../css/propiedades%20de%20texto) |
| Subtítulo fino y espaciado | `font-weight: 100; letter-spacing: 2px;` | [Texto](../css/propiedades%20de%20texto) |
| Aire alrededor del párrafo | `padding: 20px;` | [Padding](../css/padding%20y%20margin) |

## Por qué `margin: auto` centra

Si un bloque tiene un `width` fijo, `margin: auto` reparte el espacio sobrante **a partes iguales** a izquierda y derecha → queda centrado.

## Ideas para mejorarla

- `border-radius: 12px;` en `.card` para redondear las esquinas.
- `padding` en `.card` para que el contenido no toque los bordes.
- Una foto con `<img>` y `border-radius: 50%` para hacerla redonda.
