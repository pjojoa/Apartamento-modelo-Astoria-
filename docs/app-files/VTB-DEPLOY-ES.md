# Tour virtual — despliegue en tu web

Este paquete ZIP contiene **tu tour virtual** listo para compartir y publicar: visor Marzipano, interfaz Virtual Tour Builder (menús, navegación, escenas, plantilla, etc.), datos del proyecto y recursos del export original de Marzipano Tool.

## Qué incluye

- **index.html** — Punto de entrada único (reemplaza el index del ZIP original). Incluye todas las funciones del builder exportadas en esta versión.
- **tiles/** — Imágenes del panorama (multiresolución).
- **app-config.json** y/o **data.js** — Datos del tour (según el proyecto original).
- **vtb-template.json** — Metadatos de plantilla (nombre del proyecto, color primario, URL del logo).
- **vendor/** u otros scripts — Si venían en el ZIP (p. ej. marzipano.js local).
- Resto de archivos del ZIP original **salvo** el index antiguo (sustituido por el generado).

## Cómo publicarlo

1. Descomprime el ZIP **manteniendo la estructura de carpetas** (no muevas solo el HTML).
2. Sube **todos** los archivos a tu hosting (FTP, panel, Netlify, Vercel, GitHub Pages, etc.).
3. Abre en el navegador la URL de **index.html** (o configura el sitio para que la raíz sirva ese archivo).

### Requisitos

- Hosting que sirva archivos estáticos (HTML, CSS, JS, imágenes). No hace falta Node.js en el servidor.

### Logo y branding

- Si en el builder indicaste **URL del logo** (ruta relativa, p. ej. `assets/logo.png`), sube también ese archivo en la misma ruta respecto a `index.html`.

### Importante

- Carpeta **vtb/** — Logo Marval (`vtb/marval-logo.png`), plano del minimapa (`vtb/floorplan.*`) e imágenes de la galería (`vtb/gallery-0.*`, etc.) generados al exportar. Sube el ZIP completo para que el tour funcione en tu web.

---

*Generado con Virtual Tour Builder.*
