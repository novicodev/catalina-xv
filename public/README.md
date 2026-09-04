# Catalina XV — Archivos pendientes

- **Fecha del evento**: sábado 3 de octubre de 2026, 7:00 pm (America/Bogota). La fecha pública y el countdown ya están configurados.
- **Audio**: subir `once-upon-a-dream.mp3` a `/public/once-upon-a-dream.mp3` (referenciado como `/once-upon-a-dream.mp3`)
- **Fotos galería**: colocar 3–6 fotos en `/public/photos/1.jpg` etc. y reemplazar gallery placeholders
- **Mapa**: share.google link funciona como botón externo. Para embed, reemplazar venue-photo placeholder por iframe Google Maps cuando se tenga link maps.app.goo.gl o embed pb.

## RSVP personalizado

Para activar la identidad de invitados, configura `PUBLIC_SUPABASE_URL` y
`PUBLIC_SUPABASE_PUBLISHABLE_KEY` con los valores públicos de Novi. Cada enlace
de invitado debe usar `?invitacion=<token>`. Astro solo consulta el RPC
`get_guest_rsvp`; nunca expone la tabla `guests` ni una clave `service_role`.
