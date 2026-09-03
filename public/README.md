# Catalina XV — Archivos pendientes

- **Fecha del evento**: pendiente confirmación. Al recibirla, reemplazar en `src/pages/index.astro`:
  - `cover-date` placeholder → fecha real
  - `event-card` → fecha real
  - Countdown: quitar clase `countdown--pending`, añadir `data-target="2026-XX-XXT19:00:00-05:00"` y descomentar tick()
- **Audio**: subir `once-upon-a-dream.mp3` a `/public/once-upon-a-dream.mp3` (referenciado como `/once-upon-a-dream.mp3`)
- **Fotos galería**: colocar 3–6 fotos en `/public/photos/1.jpg` etc. y reemplazar gallery placeholders
- **Mapa**: share.google link funciona como botón externo. Para embed, reemplazar venue-photo placeholder por iframe Google Maps cuando se tenga link maps.app.goo.gl o embed pb.

## RSVP personalizado

Para activar la identidad de invitados, configura `PUBLIC_SUPABASE_URL` y
`PUBLIC_SUPABASE_PUBLISHABLE_KEY` con los valores públicos de Novi. Cada enlace
de invitado debe usar `?invitacion=<token>`. Astro solo consulta el RPC
`get_guest_rsvp`; nunca expone la tabla `guests` ni una clave `service_role`.
