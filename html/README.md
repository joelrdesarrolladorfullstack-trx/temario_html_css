# HTML

HTML (*HyperText Markup Language*) es el lenguaje que define la **estructura** y el **contenido** de una página web. Se escribe con **etiquetas**: `<etiqueta>contenido</etiqueta>`.

Todas las páginas parten del mismo esqueleto:

```html
<!DOCTYPE html>          <!-- le dice al navegador que es HTML5 -->
<html>
    <head>               <!-- información de la página (no se ve) -->
        <title>Título de la pestaña</title>
    </head>
    <body>               <!-- todo lo que se ve en pantalla -->
    </body>
</html>
```

---

## 1. Párrafos y encabezados — [parrafos_y_encabezados.html](parrafos_y_encabezados.html)

- `<h1>` a `<h6>`: títulos, de más importante (`h1`) a menos (`h6`). Lo normal es **un solo `<h1>`** por página.
- `<p>`: un párrafo de texto.

Los encabezados no son "texto grande": indican **jerarquía**. Google y los lectores de pantalla los usan para entender la página. El tamaño se cambia luego con CSS.

## 2. Listas — [Listas.html](Listas.html)

```html
<ol>  <li>Primero</li>  <li>Segundo</li>  </ol>   <!-- ordenada: 1, 2, 3 -->
<ul>  <li>Uno</li>      <li>Otro</li>     </ul>   <!-- desordenada: viñetas -->
```

- `<ol>` (*ordered list*) cuando el orden importa (pasos de una receta).
- `<ul>` (*unordered list*) cuando no (lista de la compra, menú de navegación).
- Cada elemento siempre va dentro de un `<li>` (*list item*).

## 3. Rutas — [rutas.html](rutas.html)

Un enlace `<a href="...">` puede apuntar a:

| Tipo | Ejemplo | Cuándo |
|------|---------|--------|
| **Ruta absoluta** | `https://www.w3schools.com` | Otra web. Lleva el protocolo `https://` |
| **Ruta relativa** | `Listas.html` | Un archivo de tu propio proyecto, contado desde donde está el HTML actual |

## 4. Enlaces — [Enlaces/](Enlaces)

Tres páginas que se enlazan entre sí (`enlaces.html`, `enlaces_2.html`, `enlaces_3.html`).

- `href`: a dónde lleva el enlace.
- `title`: texto que aparece al pasar el ratón por encima (también sirve en otras etiquetas, como el `<h1>`).
- `target="_blank"`: abre el enlace en una **pestaña nueva**.

```html
<a href="enlaces_2.html" target="_blank" title="segunda página">Ir a la 2</a>
```

## 5. Imágenes — [imagenes/img.html](imagenes/img.html)

```html
<img src="foto.png" alt="Descripción" width="500" height="333">
```

- `<img>` **no tiene etiqueta de cierre**.
- `src`: ruta de la imagen. En el ejemplo se ven tres casos:
  - Una URL de internet (ruta absoluta).
  - `ejemplo.svg` → archivo en la **misma carpeta**.
  - `../Enlaces/test_de_rutas.png` → `..` significa **subir una carpeta** y luego entrar en `Enlaces`.
- `alt`: texto alternativo. Se muestra si la imagen no carga y lo leen los lectores de pantalla. Siempre hay que ponerlo.
- `width` / `height`: tamaño en píxeles.

## 6. Formularios — [imagenes/forms.html](imagenes/forms.html)

```html
<form method="post">
    <input type="text" placeholder="Nombre" required>
    <input type="submit">
</form>
```

- `<form>` agrupa los campos que se envían juntos. `method="post"` envía los datos "ocultos" (no en la URL).
- `<input>` cambia según su `type`:

| `type` | Qué muestra |
|--------|-------------|
| `text` | Caja de texto |
| `email` | Texto que el navegador valida como correo |
| `password` | Texto oculto con puntos |
| `checkbox` | Casilla para marcar (sí/no) |
| `radio` | Opción única dentro de un grupo con el mismo `name` |
| `date` | Selector de fecha |
| `submit` | Botón de enviar |

- `name`: nombre con el que se envía el dato.
- `placeholder`: texto de ayuda dentro del campo.
- `required`: el formulario no se envía si ese campo está vacío.
