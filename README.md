# Proyectos DJD - Sistema de Gestión Integral

Archivos para publicar en Netlify con actualización automática de versión y sincronización automática en Supabase.

## Archivos

- `index.html`: sistema principal.
- `config.js`: configuración predeterminada de Supabase.
- `version.json`: versión pública usada para avisar a los usuarios que hay una actualización.
- `_headers`: configuración para evitar caché en Netlify.

## Configuración de Supabase predeterminada

Edita `config.js` y completa:

```js
window.DJD_SUPABASE_CONFIG = {
  url: "https://xxxxxxxx.supabase.co",
  key: "sb_publishable_xxxxxxxxxxxxxxxxx",
  table: "djd_app_state"
};
```

Usa únicamente la **publishable key**. No pegues la **secret key**.

Con `config.js` configurado, los usuarios ya no necesitan entrar al módulo Nube ni presionar Guardar conexión. El sistema cargará y guardará automáticamente en Supabase.

## Actualización

Cada vez que cambies el sistema, actualiza también `version.json` y el valor `APP_VERSION` dentro de `index.html`.
