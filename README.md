# 🎬 MiraPelis — Visualizador de Catálogo de Películas

Aplicación web que carga un **sitemap de películas** y muestra un catálogo interactivo con buscador, filtros, reproductor embebido y servidores de streaming.

## 🚀 Características

- 📁 **Carga automática** de `sitemap-peliculas.php` (o cualquier sitemap en formato texto/XML)
- 🎨 Interfaz moderna tipo Netflix
- 🔍 Búsqueda instantánea en el catálogo local
- 🔻 Filtros por año, género y categorías (recientes, clásicos, mejor puntuados)
- ▶️ Reproductor de video con **múltiples servidores** (Latino, Castellano, Subtitulado)
- 📱 Diseño responsive (funciona en móviles)
- 🌐 Datos enriquecidos desde **The Movie Database (TMDB)**
- 📄 Carga lazy de imágenes con shimmer effect

## 📦 Cómo funciona

1. El HTML intenta cargar automáticamente un archivo `sitemap-peliculas.php` (puedes cambiar la ruta en el código)
2. El sitemap puede estar en:
   - **Formato texto**: `URL\tfecha\tprioridad` (una URL por línea)
   - **Formato XML**: `<url><loc>...</loc><lastmod>...</lastmod></url>`
3. Extrae el **slug** de la URL (ej: `/pelicula/avengers-endgame`), y genera el título y año
4. Consulta **TMDB** para obtener sinopsis, póster, calificaciones y géneros
5. Al hacer clic en una película, **scrapea dinámicamente** los servidores del streaming
<br></br>
![Home](PNG/Captura1.png)
![Movie](PNG/Captura2.png)
