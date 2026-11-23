# Selectores

CSS (*Cascading Style Sheets*) da **estilo** al HTML. Una regla tiene esta forma:

```css
selector {
    propiedad: valor;
}
```

El **selector** dice *a qué elementos* se aplica el estilo.

## Los tres selectores básicos

| Selector | Sintaxis | En el HTML | Ejemplo |
|----------|----------|------------|---------|
| Etiqueta | `li` | `<li>` | Todos los `<li>` en rojo |
| Clase | `.faltante` | `class="faltante"` | Se puede repetir en muchos elementos |
| Id | `#ingrediente-secreto` | `id="ingrediente-secreto"` | Único en toda la página |

## Especificidad: ¿quién gana?

En el ejemplo todos los `<li>` son rojos, pero:

- El que tiene `class="faltante"` sale **verde**.
- El que tiene `id="ingrediente-secreto"` sale **morado**.

Cuando varias reglas chocan, gana la más **específica**:

```
id (#)  >  clase (.)  >  etiqueta
```

Y el `<span>` dentro del primer `<li>` es **azul** porque tiene su propia regla, más cercana que la del `<li>` que lo contiene.

## Cómo enlazar el CSS

```html
<link rel="stylesheet" href="styles.css">
```

Va dentro del `<head>`.
