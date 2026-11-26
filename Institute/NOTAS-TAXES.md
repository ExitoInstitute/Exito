# NOTAS TAXES (para las jefas) - Taxes.html

Respaldo del original: Institute-antes\Taxes.html. Las notas dentro del código se llaman NOTA FRANK #N.
Precios: solo los que ya estaban en la página ($7,000 pago anual; 6 pagos de $2,000 = $12,000). No se inventó ninguna cifra, testimonio ni escasez.

**#1 Título.** Antes: "Deja de coordinar por separado tu contabilidad, nómina e impuestos" (hablaba de lo que dejas de hacer). Ahora: "Tu contabilidad, nómina e impuestos en orden, con un solo equipo" y una frase corta. Por qué: se vende el resultado que el dueño quiere (Hormozi, $100M Offers, Dream Outcome, p. 64).

**#2 Botón principal.** Antes: "Consultar si mi negocio encaja". Ahora: "ELEGIR MI PAQUETE" lleva a los precios; "¿Dudas? Habla con el equipo" queda como segunda opción. Por qué: una sola acción clara, menos esfuerzo (Value Equation, p. 67).

**#3 Lista "Lo que recibes".** Antes: los servicios estaban repartidos en la página. Ahora: una lista junta justo antes de los precios. Sin valor en dólares por pieza, porque la lista interna de la página dice que no se publican hasta aprobarlos. Si ustedes dan esos valores, se suman aquí (Hormozi, presentar el stack, p. 112).

**#4 Compra y ahorro.** Antes: botones "Consultar pago". Ahora: "COMPRAR" con enlace de Stripe en cada opción, y la etiqueta "Ahorras $5,000 frente a las cuotas" ($12,000 - $7,000). Por qué: pagar es un clic y el pago único se ve mejor (Money Models, Payment Plan Downsells, p. 113-116).

**#5 Garantía (PROPUESTA, pendiente de aprobación).** Antes: ninguna. Ahora: "Confirmación sin riesgo": si al comenzar confirmamos que los servicios no aplican a tu negocio, se devuelve el 100 %. Por qué: quita el miedo a pagar (Offers, Guarantees, p. 118). Ustedes deciden si se publica y con qué plazo. Un solo aviso claro (#5b): servicio de preparación, no asesoría legal ni fiscal, sin garantía de resultados ante el IRS.

**#6 y #7 Menú y cierre.** Antes: "Consultar paquete". Ahora: "ELEGIR MI PAQUETE" a los precios. Por qué: misma acción en toda la página.

**#8 Pie de página.** Privacidad, términos, cookies, "Configurar cookies" y "No vender ni compartir mi información personal" (California, por el píxel de Meta), más aviso corto.

**#9 Píxel de Meta.** Aviso de cookies (el píxel solo carga si aceptan). ViewContent al ver precios, InitiateCheckout al pulsar comprar, Lead al pulsar "Habla con el equipo" (la página no tiene formulario).

## Pendiente por decidir / completar
- Enlaces de Stripe: STRIPE_LINK_TAXES_ANUAL y STRIPE_LINK_TAXES_CUOTAS (cuotas = suscripción de 6 pagos de $2,000 que se detenga sola). Redirigir a gracias.html?plan=taxes&v=7000 (o 12000).
- PIXEL_ID del píxel de Meta.
- Contacto oficial (CONTACT_URL en el script): sigue visible el aviso "Enlace de contacto pendiente".
- Antes se confirmaba el alcance ANTES de contratar; ahora se paga y luego se confirma. Las jefas deben aprobar eso (por eso la garantía #5).
- Aprobar o quitar la garantía; valores por servicio; sección "El equipo" sigue oculta (faltan testimonios y datos verificables).
- No se creó escasez: la página no da datos reales.

## SEO, imágenes y WhatsApp (NOTA FRANK #10 a #16)

| # | Qué cambió | Por qué, en simple |
|---|------------|--------------------|
| 10 | Idioma de la página `es` (antes `es-US`) | Google sabe que está en español |
| 11 | Título (59 letras): "Contabilidad y taxes para negocios \| Bookkeeping en español". Descripción (153 letras) con esas búsquedas. Canonical, Open Graph y Twitter | Son las palabras que busca el dueño de negocio latino |
| 12 | Fichas para Google (JSON-LD): el servicio con sus precios de la página (pago anual $7,000; seis pagos de $2,000, total $12,000) y las 8 preguntas frecuentes tal cual | Google puede mostrar precio y preguntas. No se inventó nada |
| 13 | Las 3 imágenes en base64 (favicon y logo) pasaron a archivos en `img/`. Alt en español; "lazy" en el logo del pie | La página pasó de 310,161 a 70,949 bytes. Mismos bytes |
| 14 | En el pie, enlaces a Inicio, "Living trust en español en California" y "Coaching para dueños de negocio latinos" | Une las páginas entre sí |
| 15 | "¿Dudas? Habla con el equipo" ahora abre el WhatsApp oficial (+1 510 909 8823, el mismo de las otras páginas). El aviso visible "Enlace de contacto pendiente de confirmación" ya no se muestra | Antes el botón llevaba a un aviso interno; ahora lleva a una persona |
| 16 | Botón verde fijo de WhatsApp abajo a la derecha (60 px) | Contacto a un toque; sube cuando sale el aviso de cookies |

**Importante:** la carpeta `img/` tiene que subirse junto con los HTML.

**Lo que falta (antes de publicar):**
- Cambiar `DOMINIO` por el dominio real en esta página (canonical, Open Graph, JSON-LD) y en `robots.txt` y `sitemap.xml`. Es un buscar y reemplazar de `https://DOMINIO`.
- La imagen para compartir en redes (og:image) hoy es el logo. Lo ideal es una imagen de 1200 x 630 px; cuando exista, se cambia en la etiqueta og:image y twitter:image.
- Cuando el sitio esté publicado: dar de alta el dominio en Google Search Console y enviar el `sitemap.xml`.
- Confirmar que el WhatsApp +1 (510) 909-8823 es el canal correcto para las dudas de Taxes (si es otro, se cambia en `CONTACT_URL`).
