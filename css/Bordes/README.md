# Bordes

`border` es la línea entre el `padding` y el `margin` (ver [modelo de caja](../padding%20y%20margin)).

## Forma corta

```css
border: 1px solid black;
/*      grosor  estilo  color */
```

Estilos más usados: `solid`, `dashed` (rayas), `dotted` (puntos), `double`, `none`.

## Un lado por separado

```css
border-top: 1px solid greenyellow;
border-right: ...;
border-bottom: ...;
border-left: 1px solid green;
```

## El ejemplo

Formulario con fondo negro en el que los `<input>` no tienen borde completo, solo **arriba y a la izquierda**:

```css
input {
    border: none;                         /* 1. quita todos los bordes */
    border-top: 1px solid greenyellow;    /* 2. añade solo el de arriba */
    border-left: 1px solid green;         /*    y el de la izquierda */
    background: transparent;              /* deja ver el fondo negro */
    padding: 6px 9px;
}
```

Primero se quita todo y luego se añade lo que se quiere: es un patrón muy común.

## Bordes redondeados

```css
border-radius: 8px;    /* esquinas redondeadas */
border-radius: 50%;    /* círculo (si el elemento es cuadrado) */
```
