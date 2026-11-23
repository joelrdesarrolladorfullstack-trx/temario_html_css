# Unidades de medida

## Absolutas

| Unidad | Qué es |
|--------|--------|
| `px` | Píxel. Siempre mide lo mismo |

## Relativas

| Unidad | Relativa a… | Ejemplo |
|--------|-------------|---------|
| `%` | El tamaño del elemento padre | `width: 50%` → mitad del padre |
| `em` | El `font-size` del **padre** | Si el padre tiene `20px`, `1em = 20px` |
| `rem` | El `font-size` del **`<html>`** (raíz) | Normalmente `1rem = 16px` |
| `vw` | 1% del **ancho** de la ventana | `50vw` → media pantalla de ancho |
| `vh` | 1% del **alto** de la ventana | `100vh` → toda la altura visible |

## El ejemplo

```css
div  { font-size: 20px; }
h1   { height: 50vh; width: 50vw; }   /* mitad de la pantalla, cambia al redimensionar */
span { font-size: 1em; }             /* igual que su padre */
```

- Cambia el tamaño de la ventana del navegador y verás cómo el `<h1>` crece y se encoge (por `vw` / `vh`).
- `em` se **acumula**: un `2em` dentro de otro `2em` es 4 veces el tamaño original. Por eso para tamaños de letra se suele preferir `rem`.

⚠️ Si escribes mal la unidad (por ejemplo `24xp` en vez de `24px`), el navegador **ignora** esa línea entera.
