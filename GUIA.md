# Guía para completar el sitio de Star Conection

Este paquete tiene todo lo necesario para que vos mismo completes el sitio con tus datos y fotos.

## Contenido del paquete

- `index.html` → el sitio completo (abrilo con doble clic para verlo en el navegador).
- `images/` → carpeta con las fotos de placeholder. Cada una tiene el nombre exacto que usa el HTML y el tamaño recomendado escrito encima.
- `GUIA.md` → este archivo.

## Cómo reemplazar las fotos

Es lo más simple: **no hace falta tocar el código**. Solo tenés que poner tus fotos dentro de la carpeta `images/`, con el mismo nombre de archivo que la que querés reemplazar (y en formato `.jpg`). El sitio las va a levantar automáticamente.

| Archivo a reemplazar | Sección | Dónde aparece | Tamaño recomendado |
|---|---|---|---|
| `images/hero-bg.jpg` | Portada (Hero) | Foto de fondo grande arriba de todo | 1600×900 px (horizontal) |
| `images/nosotros-1.jpg` | Quiénes somos | 1ra foto de la columna (arriba) | 800×900 px (vertical) |
| `images/nosotros-2.jpg` | Quiénes somos | 2da foto de la columna (medio, corrida) | 800×900 px (vertical) |
| `images/nosotros-3.jpg` | Quiénes somos | 3ra foto de la columna (abajo) | 800×900 px (vertical) |
| `images/proyecto-1.jpg` | Proyectos | 1ra tarjeta ("Red FTTH – Zona urbana") | 800×1000 px (vertical) |
| `images/proyecto-2.jpg` | Proyectos | 2da tarjeta ("Corredor vial RN 8") | 800×1000 px (vertical) |
| `images/proyecto-3.jpg` | Proyectos | 3ra tarjeta ("Despliegue aéreo") | 800×1000 px (vertical) |
| `images/proyecto-4.jpg` | Proyectos | 4ta tarjeta ("Nexo de fibra óptica") | 800×1000 px (vertical) |
| `images/galeria-1.jpg` a `galeria-6.jpg` | Galería | Las 6 fotos en fila de abajo | 400×300 px (horizontal) |

Tip: si tus fotos no vienen exactamente en esas medidas no pasa nada, el diseño las recorta automáticamente para que llenen el espacio (`object-fit: cover`). Lo importante es que sean del mismo lado (vertical u horizontal) que la que reemplazan, para que no se vean recortadas raro.

Si en algún momento querés usar un nombre de archivo distinto, buscá ese nombre dentro de `index.html` (Ctrl+F / Cmd+F) y reemplazalo ahí también.

### Logo

Actualmente el logo es un círculo con una estrella (texto). Si tenés un logo propio en imagen:
1. Poné el archivo en `images/logo.png`.
2. En `index.html` buscá el comentario `ENCABEZADO / LOGO` (aparece 2 veces: en el header y en el footer) y seguí la instrucción que está ahí en el comentario para reemplazar el círculo por tu imagen.

## Cómo completar los textos

Abrí `index.html` con cualquier editor de texto (Notepad, TextEdit, VS Code, Sublime, etc. — no hace falta saber programar). Cada sección del sitio tiene un comentario que dice qué es y qué podés editar, por ejemplo:

```html
<!-- EDITAR: título principal -->
<h1>CONECTAMOS<span class="accent">LO QUE IMPORTA</span></h1>
```

Solo tenés que cambiar el texto que está entre las etiquetas (`<h1>...</h1>`, `<p>...</p>`, etc.) sin tocar las etiquetas en sí. Buscá `Ctrl+F` la palabra `EDITAR` para saltar de un campo a otro rápido.

### Resumen de todo lo que hay para completar

| Sección | Qué texto completar |
|---|---|
| Portada (Hero) | Título grande, bajada/descripción |
| Estadísticas | Los 4 números y sus etiquetas (años de experiencia, proyectos, km, equipo) |
| Quiénes somos | Título y los 2 párrafos de descripción |
| Servicios | Título de la sección + nombre y descripción de cada una de las 6 tarjetas (obras urbanas, obras viales, tendido de fibra, canalizaciones, mantenimiento, proyectos integrales) — podés cambiar los servicios por los que realmente ofrece tu empresa |
| Proyectos | Título de cada tarjeta y su ubicación (ciudad/zona) |
| Galería | Solo las imágenes, no lleva texto |
| CTA (franja roja) | Texto de invitación a contactar |
| Footer | Nombre de la empresa, teléfono, mail, dirección, horario de atención, links de redes sociales (Facebook, Instagram, LinkedIn) |
| Nombre de la empresa | Aparece en el logo (header y footer) y en el título de la pestaña del navegador (`<title>` al principio del archivo) |

## Cómo ver los cambios

Simplemente guardá el archivo `index.html` y volvé a abrirlo (o refrescá) en el navegador — no necesita ningún programa especial ni conexión a internet, salvo para cargar la tipografía (Google Fonts) que sí requiere internet la primera vez.

## Si te trabás

Contame qué sección estás editando y qué necesitás (agregar una tarjeta de servicio más, sacar una foto de la galería, cambiar el orden de las secciones, conectar el formulario de contacto a un mail real, etc.) y seguimos ajustando el archivo juntos.
