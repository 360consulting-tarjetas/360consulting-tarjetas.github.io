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
- `assets/360-wallet-logo.png`: exportación de 480 × 480 píxeles del logo vectorial para el pase de Wallet.
- `assets/360-Consulting-Baktara-Arceo.pkpass`: pase firmado por WalletWallet y proporcionado para esta tarjeta. El botón «Guardar en Apple Wallet» enlaza directamente con este archivo.

## Apple Wallet

El pase contiene el logo de 360, el nombre, el teléfono y un QR que abre esta tarjeta. Se publica sin modificar los bytes del archivo firmado. Cualquier cambio del contenido requiere generar un nuevo pase firmado.

Se comprobaron los hashes del manifiesto, la firma CMS, la cadena hasta Apple Root CA y la coincidencia del identificador y del equipo con el certificado. El pase no tiene fecha de caducidad configurada; el certificado de firma actual vence el 20 de enero de 2027.

Para comprobar la instalación en un iPhone, abre la tarjeta en Safari, pulsa «Guardar en Apple Wallet» y confirma «Agregar». Esta instalación requiere una prueba en el dispositivo. Para Google Wallet hace falta su propio enlace de guardado; el archivo `.pkpass` corresponde a Apple Wallet.

## Comprobaciones locales

Referencias a archivos, enlaces, vCard UTF-8 con foto y 15 escenarios para QR, compartir, giro y estados de error. No se realizó una prueba visual en navegador.
