# NOTAS FRANK · Coaching.html

Cada número coincide con el comentario `NOTA FRANK #N` dentro de la página. Original guardado en `Institute-antes\Coaching.html`.

**#1 Título principal.** Antes: "Deja de darle vueltas a las decisiones importantes…". Ahora: "Sal de la duda y toma la decisión importante de tu negocio", con el resultado (prioridades y pasos por escrito), los 45 minutos, el precio desde $375 y el botón ELEGIR MI PROGRAMA. Por qué: la gente compra el resultado que sueña, rápido y con claridad de cuánto cuesta (Hormozi, $100M Offers, Ecuación de Valor, p. 62 y 65).

**#2 Orden de programas.** Antes: Clarity, Momentum, Transformation. Ahora: Transformation ($3,500), Momentum ($1,750), Clarity ($375). Por qué: ver primero el precio alto hace que los otros parezcan razonables (Pricing Playbook, Play #9, ancla de precio alto). No se cambió ningún precio.

**#3 Botones.** Antes: "CONSULTAR … POR WHATSAPP". Ahora: "RESERVAR CLARITY · $375", etc., con el mismo WhatsApp. Cada clic se registra como Lead en Meta. Pendiente: si quieren cobrar en línea, hay que crear enlaces de Stripe (marcadores sugeridos STRIPE_LINK_CLARITY, STRIPE_LINK_MOMENTUM, STRIPE_LINK_TRANSFORMATION); mientras tanto sigue el WhatsApp.

**#4 Garantía (PROPUESTA, requiere aprobación antes de publicar).** Antes: ninguna. Ahora: "Si al terminar tu primera sesión no tienes por escrito tus prioridades y tus próximos pasos, repetimos esa sesión sin costo." Por qué: quita el miedo a comprar (Hormozi, $100M Offers, Garantías, p. 117 y 119). Las jefas deben decidir si la ofrecen y con qué condiciones; si no, se borra el recuadro.

**#5 Un solo aviso legal.** Antes: el mismo aviso repetido en nota, preguntas frecuentes y pie. Ahora: un recuadro claro junto a los programas (antes de contratar) que dice que es educativo, sin asesoría legal/fiscal/financiera y sin garantía de resultados de negocio.

**#6 Letra y botones más grandes.** Textos de los programas, preguntas y botones subidos de tamaño, para personas mayores de 60 años.

**#7 Pie de página.** Nuevos enlaces a Privacidad, Términos y Cookies, "Configurar cookies" y "No vender ni compartir mi información personal" (obligatorio en California al usar el píxel de Meta).

**#8 Medición.** Aviso de cookies y píxel de Meta (solo cargan si la persona acepta); ViewContent al llegar a los programas. Falta poner el número real del PIXEL_ID.

## No se hizo (a propósito)
- Testimonios: la página no tiene ninguno y no se inventan. Si hay clientes reales que acepten, se añaden con su permiso.
- Escasez/urgencia: la página no da datos reales de cupos; no se puso nada.
- "Value stack" con valores en dólares: no se inventaron cifras; solo se usan los precios que ya estaban.
- Bonos y continuidad: ideas para decidir más adelante (por ejemplo un bono de plantilla de prioridades), sin publicarlas.

## SEO, imágenes, pago de Clarity y WhatsApp (NOTA FRANK #9 a #16)

| # | Qué cambió | Por qué, en simple |
|---|------------|--------------------|
| 9 | El idioma ya era `es`; se dejó igual | Google sabe que está en español |
| 10 | Título (57 letras): "Coaching para dueños de negocio latinos \| Éxito Institute". Descripción (148 letras). Canonical, Open Graph y Twitter | Son las palabras que busca el dueño de negocio latino |
| 11 | Fichas para Google (JSON-LD): el servicio con sus precios de la página (Clarity $375, Momentum $1,750, Transformation $3,500) y las 8 preguntas frecuentes tal cual | Google puede mostrar precios y preguntas. No se inventó nada |
| 12 | Las 2 imágenes en base64 (favicon y logo) pasaron a archivos en `img/`. Alt en español | La página pasó de 191,532 a 68,491 bytes. Mismos bytes |
| 13 | En el pie, enlaces a Inicio, "Living trust en español en California" y "Contabilidad y taxes para tu negocio" | Une las páginas entre sí |
| 14 | El botón de Clarity ahora es "PAGAR CLARITY · $375" y lleva a pago en línea (marcador `STRIPE_LINK_CLARITY`). Registra InitiateCheckout con valor 375 USD. Momentum y Transformation siguen por WhatsApp | La oferta de entrada se compra sin esperar respuesta |
| 15 | **Propuesta** (falta aprobación): bajo Clarity se lee "Si después eliges Momentum o Transformation en los siguientes 30 días, te abonamos lo que pagaste por Clarity." | Quita el miedo a "pagar dos veces" y empuja al programa más grande (Hormozi: Rollover Upsell). Si las jefas no lo aprueban, se borra ese párrafo |
| 16 | Botón verde fijo de WhatsApp abajo a la derecha (60 px) | Contacto a un toque; sube cuando sale el aviso de cookies |

**Importante:** la carpeta `img/` tiene que subirse junto con los HTML.

**Lo que falta (antes de publicar):**
- Cambiar `DOMINIO` por el dominio real en esta página (canonical, Open Graph, JSON-LD) y en `robots.txt` y `sitemap.xml`. Es un buscar y reemplazar de `https://DOMINIO`.
- La imagen para compartir en redes (og:image) hoy es el logo. Lo ideal es una imagen de 1200 x 630 px; cuando exista, se cambia en la etiqueta og:image y twitter:image.
- Cuando el sitio esté publicado: dar de alta el dominio en Google Search Console y enviar el `sitemap.xml`.
- Crear en Stripe el enlace de pago de Clarity ($375) y ponerlo en lugar de `STRIPE_LINK_CLARITY`. Que al pagar lleve a `gracias.html`. Hasta entonces ese botón no funciona.
- Aprobar o quitar el abono de Clarity (NOTA FRANK #15).
