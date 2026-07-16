# Los Pares 84×88 · Sistemas (app instalable)

Esta carpeta es una PWA: una sola pantalla con acceso a tus 5 sistemas,
que se puede **instalar** en iPhone, Android o PC con el logo de Los Pares.

## Qué contiene
- `index.html` — la pantalla principal (el "menú" de sistemas)
- `manifest.webmanifest` — datos de la app (nombre, ícono, colores)
- `sw.js` — service worker (necesario para poder instalarla)
- `icon-192.png`, `icon-512.png` y versiones *maskable* — ícono de la app
- `apple-touch-icon.png` — ícono para iPhone/iPad
- `favicon-16.png`, `favicon-32.png` — ícono de pestaña

## Publicar en GitHub Pages (igual que tus otros sistemas)
1. Crea un repositorio nuevo, por ejemplo **`sistemas`** en tu cuenta `Arpaco07`.
2. Sube **todos** los archivos de esta carpeta a la raíz del repo (rama `main`).
3. Ve a **Settings → Pages**, en *Source* elige **Deploy from a branch**,
   rama `main`, carpeta `/ (root)` y guarda.
4. En 1–2 minutos quedará en:
   **https://arpaco07.github.io/sistemas/**

> Funciona con cualquier nombre de repo porque todas las rutas son relativas.

## Instalar la app
- **Android / PC (Chrome o Edge):** abre el link y toca el botón
  **“Instalar la app en este dispositivo”** (o el ícono de instalar en la barra).
- **iPhone / iPad (Safari):** abre el link, toca **Compartir** y luego
  **Añadir a inicio**. La página ya te muestra el aviso.

Al instalarla aparece un solo ícono (el logo P 84×88) que abre el menú
con los 5 sistemas. Cada sistema sigue pidiendo su propio PIN.

## Cambiar / agregar sistemas después
Edita `index.html` y busca la sección `<nav class="grid">`.
Cada sistema es un bloque `<a class="card" href="...">`. Copia uno,
cambia el `href` y el texto, y listo.
