# Curso de HTML y CSS — Apuntes y ejemplos

Repositorio con los ejemplos que fui haciendo mientras aprendía **HTML** y **CSS** desde cero.
Cada tema tiene su carpeta con el código y un `README.md` que explica qué se practica.

> Para ver un ejemplo: abre el archivo `.html` en el navegador (doble clic o con la extensión *Live Server* de VS Code).

---

## 📄 HTML

| Tema | Archivo | Qué se aprende |
|------|---------|----------------|
| Párrafos y encabezados | [parrafos_y_encabezados.html](html/parrafos_y_encabezados.html) | `<h1>`…`<h6>` y `<p>` |
| Listas | [Listas.html](html/Listas.html) | Listas ordenadas `<ol>` y desordenadas `<ul>` |
| Rutas | [rutas.html](html/rutas.html) | Enlaces absolutos y relativos |
| Enlaces | [Enlaces/](html/Enlaces) | Navegar entre páginas, `title`, `target="_blank"` |
| Imágenes | [imagenes/img.html](html/imagenes/img.html) | `<img>`, `src`, `alt`, rutas a otras carpetas |
| Formularios | [imagenes/forms.html](html/imagenes/forms.html) | `<form>` y tipos de `<input>` |

👉 Explicación completa en [html/README.md](html/README.md)

## 🎨 CSS

| # | Tema | Qué se aprende |
|---|------|----------------|
| 1 | [Selectores](css/selectores) | Etiqueta, clase (`.`), id (`#`) y especificidad |
| 2 | [Colores](css/Colores) | Nombres, hexadecimal, `rgb()`, `hsl()` |
| 3 | [Unidades de medida](css/unidades%20de%20medida) | `px`, `em`, `rem`, `%`, `vw`, `vh` |
| 4 | [Width y height](css/width%20y%20height) | Ancho y alto de los elementos |
| 5 | [Padding y margin](css/padding%20y%20margin) | Espacio interior y exterior (modelo de caja) |
| 6 | [Bordes](css/Bordes) | `border` y sus lados por separado |
| 7 | [Box sizing](css/box%20sizing) | `content-box` vs `border-box` |
| 8 | [Propiedades de texto](css/propiedades%20de%20texto) | Fuentes propias con `@font-face` y estilos de texto |

La carpeta [css/Fonts](css/Fonts) contiene la fuente **Montserrat** (licencia libre OFL, ver `OFL.txt`) que se usa en *Propiedades de texto*.

## 🧪 Ejercicios

| Ejercicio | Qué combina |
|-----------|-------------|
| [Tarjeta de presentación](ejercicios) | Colores, texto, padding, centrado con `margin: auto` |

---

## Estructura

```
├── html/          → temas de HTML
├── css/           → un tema de CSS por carpeta (index.html + styles.css)
└── ejercicios/    → ejercicios que mezclan varios temas
```
