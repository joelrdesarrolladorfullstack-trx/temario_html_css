# Box sizing

¿El `width` incluye el padding y el borde o no? Eso lo decide `box-sizing`.

## El ejemplo

Las dos primeras cajas tienen **el mismo CSS** salvo una línea:

```css
.box { width: 100px; height: 100px; }

.box:nth-child(1) {
    padding: 30px;
    border: 10px solid black;
}

.box:nth-child(2) {
    padding: 30px;
    border: 10px solid black;
    box-sizing: border-box;   /* ← la diferencia */
}
```

| | `content-box` (por defecto) | `border-box` |
|---|---|---|
| `width: 100px` mide… | solo el contenido | contenido + padding + borde |
| Tamaño real en pantalla | 100 + 30·2 + 10·2 = **180px** | **100px** |

La caja 1 se ve mucho más grande que la 2 aunque las dos digan `width: 100px`.

## Lo que se usa en la práctica

Casi todos los proyectos empiezan con:

```css
* {
    box-sizing: border-box;
}
```

Así el tamaño que escribes es el tamaño que ves.

## Extra: `:nth-child()`

`.box:nth-child(1)` selecciona la caja que es el **primer hijo** de su padre. `nth-child(2)` la segunda, etc. Es una *pseudo-clase*.
