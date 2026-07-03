# APAP — Mapa de cobertura y actividad comercial (Santo Domingo)

Mapa web interactivo que cruza la **actividad comercial** (mosaico basado en datos de Google Places) con la **red de puntos de acceso bancario** (Sucursales, Cajeros/ATM y Subagentes) en Santo Domingo.

## Contenido del repositorio

- `index.html` — la página completa y **auto-contenida** (todos los datos van embebidos; usa librerías Leaflet desde CDN). Es lo único necesario para publicar.

> No se incluyen API keys, scripts de generación ni archivos de datos crudos (Excel/CSV). La página es un **snapshot** de los datos ya procesados.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub y sube estos archivos (rama `main`).
2. En el repo: **Settings → Pages**.
3. En *Build and deployment* → *Source*: **Deploy from a branch**.
4. Branch: `main`, carpeta `/ (root)`. Guarda.
5. En 1–2 minutos la página queda publicada en:
   `https://<tu-usuario>.github.io/<nombre-del-repo>/`

## Notas

- Requiere conexión a internet para cargar los mapas base (OpenStreetMap) y las librerías (Leaflet / MarkerCluster / Leaflet.heat) desde CDN.
- Para **regenerar** el mapa con datos nuevos se usan scripts privados que **no** forman parte de este repositorio (contienen credenciales y no deben publicarse).
