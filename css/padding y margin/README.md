# Padding y margin — el modelo de caja

En CSS **todo elemento es una caja** formada por capas, de dentro hacia fuera:

```
┌──────────── margin ────────────┐   espacio FUERA (separa de otros)
│  ┌───────── border ─────────┐  │   el borde
│  │  ┌────── padding ─────┐  │  │   espacio DENTRO (entre borde y contenido)
│  │  │      contenido      │  │  │
│  │  └─────────────────────┘  │  │
│  └───────────────────────────┘  │
└─────────────────────────────────┘
```

- **padding**: relleno interior. Toma el color de fondo del elemento.
- **margin**: separación exterior. Siempre es transparente.

## Formas de escribirlo

```css
margin: 10px;                 /* los 4 lados */
margin: 10px 20px;            /* arriba-abajo | izquierda-derecha */
margin: 10px 20px 5px;        /* arriba | lados | abajo */
margin: 10px 20px 5px 0;      /* arriba | derecha | abajo | izquierda (sentido del reloj) */
margin-top: 10px;             /* un solo lado */
```

Lo mismo vale para `padding`.

## El ejemplo

Cuatro cajas de colores con `margin: 10px` cada una, centradas en pantalla con:

```css
body {
    display: flex;            /* pone los hijos en fila */
    justify-content: center;  /* centra en horizontal */
    align-items: center;      /* centra en vertical */
    height: 100vh;            /* el body ocupa toda la pantalla */
    margin: 0;                /* quita el margen que el navegador pone por defecto */
}
```

(`flex` es un tema propio; aquí solo se usa para centrar).

💡 Truco: `margin: 0 auto;` centra horizontalmente un bloque que tenga `width`.
