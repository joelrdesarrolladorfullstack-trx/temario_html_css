# Colores

Un color en CSS se puede escribir de varias formas. Todas estas son el mismo rojo:

| Formato | Ejemplo | Notas |
|---------|---------|-------|
| Nombre | `red` | Fácil, pero hay pocos nombres |
| Hexadecimal | `#ff0000` | `#RRGGBB`, cada par va de `00` a `ff` |
| RGB | `rgb(255, 0, 0)` | Rojo, verde, azul de 0 a 255 |
| RGBA | `rgba(255, 0, 0, 0.5)` | El cuarto valor es la transparencia (0 a 1) |
| HSL | `hsl(0, 100%, 50%)` | Tono (0–360°), saturación, luminosidad |

## El ejemplo

```css
.box {
    width: 200px;
    height: 200px;
    background-color: #feeeff;   /* rosa muy claro en hexadecimal */
    margin: 20px;
}
```

- `color` → color del **texto**.
- `background-color` → color del **fondo**.

💡 Truco: en VS Code, al pasar el ratón por un color aparece un selector para elegirlo visualmente.
