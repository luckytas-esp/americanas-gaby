# Americanas Gaby — PWA (instalable en móvil)

Esta carpeta contiene una versión PWA de tu app (todo local, sin API).
Puedes publicarla gratis en GitHub Pages y así instalarla en Android/iPhone.

## Estructura

- index.html
- manifest.json
- service-worker.js
- assets/
  - icons/
    - icon-192.png
    - icon-512.png
    - maskable-512.png
    - apple-touch-icon.png

## 1) Probar en local (sin instalar todavía)

> Importante: algunas funciones PWA (service worker) NO funcionan bien si abres el archivo con doble click (file://).
> Para probar correctamente, usa un servidor local.

Opción fácil con Python (si lo tienes instalado):

```bash
cd AmericanasGaby_PWA
python -m http.server 8000
```

Luego abre:
http://localhost:8000

## 2) Publicar en GitHub Pages (link público con HTTPS)

1. Crea una cuenta en GitHub (si no tienes).
2. Crea un repositorio nuevo llamado por ejemplo: `americanas-gaby`.
3. Sube TODOS los archivos de esta carpeta al repositorio.
4. En el repo: **Settings → Pages**
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/(root)**
5. Guarda. GitHub te dará una URL como:
   `https://TUUSUARIO.github.io/americanas-gaby/`

## 3) Instalar en el móvil

### Android (Chrome)
- Abre la URL
- Verás un botón **Instalar** (arriba, junto a Exportar/Importar)
- O menú ⋮ → **Instalar aplicación**

### iPhone (Safari)
- Abre la URL en Safari
- Botón **Compartir** (cuadrado con flecha) → **Añadir a pantalla de inicio**
- iOS no suele mostrar botón “Instalar” automáticamente.

## 4) Importar / Exportar datos

- **Exportar (JSON)**: descarga `padel-jornada-datos.json`
- **Importar (JSON)**: selecciona ese mismo archivo para restaurar datos en otro móvil

Nota: Importar reemplaza los datos actuales (te pedirá confirmación).
