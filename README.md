# Skintec — Rediseño del sitio web

Rediseño de una sola página (`index.html`, HTML + CSS + JS, sin dependencias de build) basado en el contenido real de [skintec.cl](https://skintec.cl): las 3 líneas de producto, la información de la empresa, industrias atendidas y datos de contacto.

## Cómo subirlo a `github.com/skintec/web`

**Opción A — desde la web de GitHub (sin terminal):**
1. Entra a tu repo → botón **Add file → Upload files**.
2. Arrastra `index.html` (y este `README.md` si quieres).
3. Confirma el commit en la rama `main`.

**Opción B — desde tu computador:**
```bash
git clone https://github.com/skintec/web.git
cd web
# copia index.html aquí
git add index.html
git commit -m "Rediseño del sitio"
git push origin main
```

## Publicarlo con GitHub Pages
1. En el repo: **Settings → Pages**.
2. En "Source" elige la rama `main` y la carpeta `/ (root)`.
3. Guarda. En 1–2 minutos quedará publicado en `https://skintec.github.io/web/`.
4. Si quieres usar `skintec.cl` como dominio, agrega un archivo `CNAME` con el dominio dentro y configura el DNS del dominio apuntando a GitHub Pages.

## Notas de diseño
- Paleta grafito + naranja señal (protección contra incendios) + azul acero (térmico/acústico) — ambos acentos corresponden a las dos líneas de negocio reales, no son colores decorativos.
- Tipografía: Barlow Condensed (titulares) + IBM Plex Sans (cuerpo) + IBM Plex Mono (códigos de ficha técnica).
- El diagrama del hero es un corte técnico real de un muro cortafuego (yeso RF, lana mineral, cámara de aire, fibrosilicato, terminación metálica), no una imagen de stock.
- El formulario de contacto usa `mailto:` para que funcione sin backend; si más adelante quieres que llegue a un CRM o guarde leads, se puede conectar a un servicio como Formspree o a un backend propio.
