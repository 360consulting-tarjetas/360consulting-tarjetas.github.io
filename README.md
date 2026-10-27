# Báktara · 360 Consulting

Tarjeta digital: https://360consulting-tarjetas.github.io/

HTML, CSS y JavaScript estáticos. WhatsApp, llamada, correo, web, LinkedIn, contacto vCard con foto, QR de la tarjeta, compartir, giro breve y fondo 3D estático. No hay flotación, inclinación con el cursor ni animaciones continuas.

Esta carpeta se sirve desde GitHub Pages, mediante la rama principal del repositorio `360consulting-tarjetas/360consulting-tarjetas.github.io`.

## Edición

- `index.html`: contenido y enlaces.
- `assets/styles.css`: diseño.
- `assets/card.js`: QR, compartir y efectos. La URL se adapta al alojamiento; `fallbackUrl` se usa al abrir archivos locales.
- `assets/360-Consulting-Baktara.vcf`: contacto con el nombre Báktara, LinkedIn y foto de 320 × 320 píxeles. La ruta anterior `assets/360-Consulting-Baktara-Arceo.vcf` sirve los mismos datos para mantener los enlaces existentes.
- `assets/baktara.jpg`: foto de 640 × 640 píxeles obtenida de la imagen original de 2289 × 2400 píxeles incluida en `TarjetaDigital_360.ai`. El recorte respeta el encuadre del diseñador y no incluye un aro; el único borde blanco se dibuja con CSS.
- `assets/360-logo.svg`: trazados vectoriales originales extraídos de `TarjetaDigital_360.ai`, sin vectorización aproximada ni imágenes incrustadas. Las imágenes iniciales se conservan para compatibilidad.
- `assets/360-wallet-logo.png`: exportación de 480 × 480 píxeles del logo vectorial para el pase de Wallet.
- `assets/360-Consulting-Baktara-Arceo.pkpass`: pase firmado por WalletWallet y proporcionado para esta tarjeta. El botón «Guardar en Apple Wallet» enlaza directamente con este archivo.

## Apple Wallet

El pase contiene el logo de 360, el nombre, el teléfono y un QR que abre esta tarjeta. Se publica sin modificar los bytes del archivo firmado. El pase suministrado todavía muestra «Báktara Arceo»; para cambiar ese nombre o actualizar su logo hay que generar un nuevo pase firmado. Los cambios de la web y la vCard no modifican los pases ya guardados.

Se comprobaron los hashes del manifiesto, la firma CMS, la cadena hasta Apple Root CA y la coincidencia del identificador y del equipo con el certificado. El pase no tiene fecha de caducidad configurada; el certificado de firma actual vence el 20 de enero de 2027.

Para comprobar la instalación en un iPhone, abre la tarjeta en Safari, pulsa «Guardar en Apple Wallet» y confirma «Agregar». Esta instalación requiere una prueba en el dispositivo. Para Google Wallet hace falta su propio enlace de guardado; el archivo `.pkpass` corresponde a Apple Wallet.

## Comprobaciones locales

Referencias a archivos, enlaces, vCard UTF-8 con foto y 15 escenarios para QR, compartir, giro, ausencia de inclinación y estados de error. La revisión de octubre de 2026 incorpora el LinkedIn proporcionado: https://www.linkedin.com/in/nadia-arceo-flores/.
