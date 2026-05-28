# Proyectos DJD - Sistema de Gestión Integral

Archivos para publicar en Netlify con actualización automática de versión.

## Archivos
- `index.html`: sistema web principal.
- `version.json`: número de versión publicado.
- `_headers`: configuración para evitar caché fuerte en Netlify.

## Cómo actualizar
1. Edita `index.html`.
2. Cambia el número de versión en:
   - `index.html`: constante `APP_VERSION`.
   - `version.json`: campo `version`.
3. Sube los cambios a GitHub.
4. Netlify publicará automáticamente el mismo enlace.
