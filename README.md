# Madrid Gratis

Web estática (HTML/CSS) sobre planes gratis en Madrid. Pensada para publicarse en GitHub Pages sin coste de hosting.

## Estructura

```
madrid-gratis/
├── index.html              → página de inicio
├── articulos.html          → índice de todos los artículos, por categoría
├── css/style.css           → estilos de todo el sitio
└── articulos/
    ├── 20-cosas-gratis-que-hacer-en-madrid.html
    └── museos-gratis-en-madrid.html
```

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo `madrid-gratis`).
2. Sube todo el contenido de esta carpeta a la raíz del repositorio.
3. En el repositorio, ve a **Settings → Pages**.
4. En "Source", elige la rama `main` y la carpeta `/root`.
5. Guarda. En un par de minutos tu web estará en `https://tu-usuario.github.io/madrid-gratis/`.

Cuando compres el dominio, solo tienes que añadirlo como dominio personalizado en esa misma pantalla de Settings → Pages.

## Cómo añadir un artículo nuevo

1. Duplica un archivo de `articulos/` (por ejemplo `museos-gratis-en-madrid.html`) y ponle el nombre del nuevo artículo en formato `mi-titulo-en-minusculas.html`.
2. Cambia el `<title>`, la `<meta name="description">`, el `<h1>` y el texto del `dek` (subtítulo).
3. Escribe el contenido dentro de `.article-body`, usando:
   - `<h2>` para secciones grandes.
   - `<div class="place">` para cada lugar/plan concreto, con `<div class="meta">` para la dirección o el metro.
   - `<div class="note">` para avisos importantes (horarios que cambian, etc.).
4. Añade el enlace al nuevo artículo en `articulos.html`, en la categoría que corresponda, y opcionalmente en `index.html` si quieres destacarlo en portada.

## robots.txt y sitemap.xml

Ya están incluidos en la raíz del proyecto, listos para que Google pueda rastrear e indexar el sitio. **Importante:** abre ambos archivos y sustituye `TU-USUARIO` por tu nombre de usuario real de GitHub antes de subirlos (o por tu dominio propio, si ya lo tienes).

Cuando publiques artículos nuevos, añade su URL dentro de `sitemap.xml` siguiendo el mismo formato.

## Siguientes pasos sugeridos

- Completar los 8 artículos restantes de la primera lista (parques, niños, pareja, lluvia, miradores, fotos, noche, fin de semana).
- Añadir imágenes propias o libres de derechos en `img/` (evitar fotos con copyright de bancos de imágenes de pago).
- Cuando haya artículos publicados, crear cuentas de TikTok/Instagram y enlazar cada vídeo al artículo correspondiente.
- Dar de alta el sitio en Google Search Console para monitorizar qué búsquedas empiezan a traer visitas.
- Valorar AdSense solo cuando haya tráfico orgánico estable.
