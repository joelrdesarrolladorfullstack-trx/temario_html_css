# Width y height

- `width`: ancho del elemento.
- `height`: alto del elemento.

```css
div {
    background-color: red;
    width: 300px;
    height: 500px;
}

input {
    width: 300px;
    height: 50px;
}
```

## Elementos de bloque vs. en línea

| Tipo | Ejemplos | Comportamiento por defecto |
|------|----------|----------------------------|
| **Bloque** | `div`, `p`, `h1`, `ul` | Ocupa todo el ancho y empieza en una línea nueva |
| **En línea** | `span`, `a`, `strong` | Ocupa solo lo que mide su contenido; **ignora** `width` y `height` |
| **En línea-bloque** | `input`, `button`, `img` | Van uno al lado del otro pero **sí** aceptan `width` y `height` |

Por eso los `<input>` del ejemplo quedan en fila y el `<div>` ocupa su propia línea.

## Propiedades relacionadas

- `min-width` / `max-width`: tamaño mínimo / máximo.
- `min-height` / `max-height`: lo mismo para el alto.

`max-width` es muy útil para que algo no se haga gigante en pantallas grandes.
