# NOTA FRANK: cambios en Home.html (para las jefas)

Original guardado en `..\Institute-antes\Home.html`. Cada cambio lleva un comentario `NOTA FRANK #N` en el código.

| # | Antes | Ahora | Por qué |
|---|-------|-------|---------|
| 1 | Letra pequeña (11 a 14 px) | Letra y botones más grandes | Muchos clientes tienen más de 60 años; menos esfuerzo para leer (Hormozi, $100M Offers, p. 62) |
| 2 | "Dale dirección a lo que estás construyendo." | "Pon en orden tu familia, tu negocio y tus números." | Se vende el resultado que el cliente sueña (p. 64) |
| 3 | Texto general sin precios | Desde $399 (LT, borrador en 2 semanas), desde $7,000 (Taxes), desde $375 (Coaching) | Precio y plazo a la vista; son cifras ya publicadas en cada página |
| 4 | "Explorar nuestros servicios" | "Ver servicios y precios" | CTA claro (Hormozi, $100M Leads, p. 66) |
| 5 | Living Trust: descripción genérica | Resultado + precio + plazo + "Plan Éxito: solo 4 familias al mes" + enlace a LT.html | Escasez real (p. 95); el enlace antes apuntaba a otro archivo |
| 6 | Taxes: enlace "pendiente" | Resultado + desde $7,000 o 6 pagos de $2,000 + enlace a Taxes.html | Resultado claro y página conectada |
| 7 | Coaching: enlace "pendiente" | Resultado + desde $375 + enlace a Coaching.html | Igual |
| 8 | Cierre sin precios | Tres filas con resultado y precio, enlazadas | CTA claros |
| 9 | Pie sin enlaces legales | Privacidad, Términos, Cookies, Configurar cookies, No vender mi información + aviso de cookies y píxel de Meta | Obligatorio en California por usar el píxel |
| 10 | Avisos dispersos | Un solo aviso visible: servicio administrativo y educativo, no asesoría legal ni fiscal | Transparencia, sin prometer resultados legales |

## Pendiente / propuestas (no publicadas)
- Garantía de servicio para Home: no se muestra. Propuesta: reutilizar la "Triple Garantía Familia en Orden" de LT cuando las jefas la aprueben.
- Los "4 familias al mes" y el plazo de 2 semanas vienen de las decisiones de LT; confirmar que son reales.
- Colocar el PIXEL_ID real (hoy es el marcador `PIXEL_ID`, el píxel no carga hasta cambiarlo).
- Foto auténtica de Esmeralda (sigue el marcador de posición).
- Taxes: no hay precio por pago único distinto de los ya publicados; no se inventó ninguno.

## SEO, imágenes y selector (NOTA FRANK #11 a #16)

| # | Qué cambió | Por qué, en simple |
|---|------------|--------------------|
| 11 | El idioma de la página ahora es `es` (antes `es-US`) | Así Google sabe que la página está en español |
| 12 | Título nuevo (58 letras): "Éxito Institute: Living Trust, Taxes y Coaching en español". Descripción nueva (155 letras) con la marca y los tres servicios. Se añadieron canonical, Open Graph y Twitter | Es lo que sale en Google y cuando alguien comparte el enlace por WhatsApp o Facebook |
| 13 | Ficha de la empresa para Google (JSON-LD tipo Organization): Éxito Institute, fundadora Esmeralda Espinoza, teléfono +1-510-909-8823 (el de WhatsApp), correo y California | Ayuda a que Google muestre bien el nombre, la fundadora y el contacto. Home no tiene preguntas frecuentes, así que no lleva ficha de preguntas (no se inventó ninguna) |
| 14 | Las imágenes estaban metidas dentro del HTML en código (base64). Ahora son archivos en la carpeta `img/` y el HTML las llama por su nombre. Todas tienen texto alternativo (alt) en español; todas menos el logo de arriba cargan con "lazy" (solo cuando se ven) | La página pasó de 294,885 a 53,714 bytes: carga mucho más rápido en el celular. Los archivos son exactamente los mismos bytes que antes |
| 15 | Arriba, junto al titular: "¿Qué necesitas hoy?" con 3 botones grandes: "Proteger a mi familia" (LT), "Ordenar mis números e impuestos" (Taxes) y "Hacer crecer mi negocio" (Coaching). Cada clic se registra como ViewContent en el píxel | La persona llega en un clic a lo que busca, sin leer toda la página |
| 16 | Botón verde fijo de WhatsApp abajo a la derecha (60 px) | Contacto a un toque. Cuando sale el aviso de cookies, el botón sube para no taparlo |

**Importante:** la carpeta `img/` tiene que subirse junto con los HTML; sin ella no se ven los logos.

**Lo que falta (antes de publicar):**
- Cambiar `DOMINIO` por el dominio real en esta página (canonical, Open Graph, JSON-LD) y en `robots.txt` y `sitemap.xml`. Es un buscar y reemplazar de `https://DOMINIO`.
- La imagen para compartir en redes (og:image) hoy es el logo. Lo ideal es una imagen de 1200 x 630 px; cuando exista, se cambia en la etiqueta og:image y twitter:image.
- Cuando el sitio esté publicado: dar de alta el dominio en Google Search Console y enviar el `sitemap.xml`.
- Si al publicar Home pasa a llamarse `index.html` (la portada del dominio), hay que cambiar `Home.html` por `/` en el canonical, og:url, el JSON-LD y el sitemap, y los enlaces "Home.html" de las otras páginas.
