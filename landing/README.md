# El Llamado Divino — Landing Page

## Estructura
```
landing/
├── index.html        ← página principal
└── assets/
    ├── sky-bg.png    ← fondo del cielo
    └── book-only.png ← mockup del libro
```

## Cómo abrir en VS Code
1. Descomprime el zip.
2. En VS Code: **File → Open Folder…** y elige la carpeta `landing/`.
3. Recomendado: instala la extensión **Live Server** (Ritwick Dey) y haz click derecho sobre `index.html` → "Open with Live Server". Esto abre la página con recarga automática al guardar.

## Insertar el video VTURB
Abre `index.html` y busca el bloque marcado:
```html
<!-- ============================================================
     VIDEO · Pega aquí tu embed (VTURB, YouTube no listado, Vimeo, etc.)
============================================================ -->
```
Reemplaza el `<div class="video-placeholder">…</div>` por tu snippet de VTURB:
```html
<vturb-smartplayer id="vid-XXXXXXXXX"></vturb-smartplayer>
<script src="https://scripts.converteai.net/.../player.js" async></script>
```
El frame ya está dimensionado en 16:9 — el reproductor se expande al 100%.

## Publicar
Sube **toda la carpeta `landing/`** (no solo el HTML) a tu hosting:
- **Hostinger / cPanel:** sube al directorio `public_html` y descomprime.
- **Netlify / Vercel / Cloudflare Pages:** arrastra la carpeta y obtienes URL gratis con HTTPS.
- **GitHub Pages:** push del contenido de la carpeta a un repo y activa Pages.

Si tu plataforma solo acepta un archivo HTML, pide la versión "single-file" autocontenida.
