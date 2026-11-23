# Propiedades de texto

## Usar una fuente propia: `@font-face`

En [fonts.css](fonts.css) se registra la fuente Montserrat (guardada en [../Fonts](../Fonts)) con un nombre inventado, `"MiFuente"`. Cada grosor es un archivo distinto:

```css
@font-face {
    font-family: "MiFuente";                                   /* nombre que usaremos */
    src: url("../Fonts/static/Montserrat-Regular.ttf") format("truetype");
    font-weight: 400;                                          /* este archivo = grosor 400 */
}
```

Luego se usa como cualquier otra fuente:

```css
p { font-family: "MiFuente"; }
```

> Para que funcione, el HTML tiene que cargar `fonts.css` **antes** que `styles.css`:
>
> ```html
> <link rel="stylesheet" href="fonts.css">
> <link rel="stylesheet" href="styles.css">
> ```
>
> Ojo también con las mayúsculas en los nombres de archivo: en Mac `montserrat-bold.ttf` y `Montserrat-Bold.ttf` son el mismo archivo, pero en un servidor Linux (como GitHub Pages) no, y la fuente no carga.

Alternativa más rápida: [Google Fonts](https://fonts.google.com), que te da el `<link>` listo para pegar.

## Propiedades de la fuente

| Propiedad | Qué hace | Ejemplo |
|-----------|----------|---------|
| `font-family` | Tipo de letra | `"MiFuente", sans-serif` |
| `font-size` | Tamaño | `20px` |
| `font-weight` | Grosor (100 fino → 900 muy grueso) | `700` o `bold` |
| `font-style` | Cursiva | `italic` |

## Propiedades del texto

| Propiedad | Qué hace | Valores |
|-----------|----------|---------|
| `color` | Color de la letra | cualquier color |
| `text-align` | Alineación | `left`, `center`, `right`, `justify` |
| `text-decoration` | Líneas sobre el texto | `underline`, `overline`, `line-through`, y estilo `wavy` (ondulado) |
| `line-height` | Alto de cada línea | `2` = el doble del tamaño de letra |
| `letter-spacing` | Espacio entre letras | `2px` |
| `text-transform` | Mayúsculas/minúsculas | `uppercase`, `lowercase`, `capitalize` (primera letra de cada palabra) |

## Fuente de respaldo

Conviene terminar siempre con una familia genérica por si la fuente no carga:

```css
font-family: "MiFuente", sans-serif;
```
