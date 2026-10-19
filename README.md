# Báktara Arceo · 360 Consulting

Tarjeta digital: https://360consulting-tarjetas.github.io/

HTML, CSS y JavaScript estáticos. WhatsApp, llamada, correo, web, contacto vCard con foto, QR de la tarjeta, compartir, giro, inclinación, flotación y fondo 3D.

Esta carpeta se sirve desde GitHub Pages, mediante la rama principal del repositorio `360consulting-tarjetas/360consulting-tarjetas.github.io`.

## Edición

- `index.html`: contenido y enlaces.
- `assets/styles.css`: diseño.
- `assets/card.js`: QR, compartir y efectos. La URL se adapta al alojamiento; `fallbackUrl` se usa al abrir archivos locales.
- `assets/360-Consulting-Baktara-Arceo.vcf`: contacto con foto. Actualiza este archivo si cambian los datos.
- `assets/baktara-arceo.jpg`: foto extraída de la referencia proporcionada.
- `assets/360-logo.svg`: logo vectorizado a partir de la referencia; mantiene la forma original y escala sin pixelarse. `assets/360-logo.jpg` conserva el recorte original.

## Comprobaciones locales

Referencias a archivos, enlaces, vCard UTF-8 con foto y 15 escenarios para QR, compartir, giro y estados de error. No se realizó una prueba visual en navegador.
