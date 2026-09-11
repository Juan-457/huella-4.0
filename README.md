# Huella 4.0 — Landing page

Sitio estático (HTML + CSS, sin build ni dependencias) para **Huella 4.0**, marca de
bioinsumos para el agro argentino y representante oficial de **Biótica Life Sciences**.

## Estado

- Landing generada a partir del contenido público de
  [@huella4.0 en Instagram](https://www.instagram.com/huella4.0/) (116
  seguidores al momento de la investigación) y de investigación pública sobre
  Biótica Life Sciences.
- Se agregó una sección "Resultados a campo" con un caso real que la marca
  publicó (trigo en espigazón, tratamiento de semilla con Humica HF + Biótica
  N2 + micorrizas, medición de °Brix vs. testigo), y se confirmaron por
  captura directa del perfil: email de contacto (`gustavoguillaumet@yahoo.com.ar`).
- **Datos confirmados directamente por el dueño de la marca (Gustavo Martín
  Guillaumet, WhatsApp 2026-09-08):** razón social/marca registrada a su
  nombre, rubro = proveedor de insumos biológicos y asesoramiento en su uso,
  representante de Biótica Life Sciences, base en **Colón, provincia de
  Buenos Aires** (reemplaza la zona de Guatimozín, Córdoba que se había
  inferido de Instagram — dato incorrecto, ya corregido en el sitio).
- **Logo oficial subido** por el dueño (`huella40.jpeg`, 1280×1280). Se
  generaron dos derivados en `assets/`: `logo-huella.jpg` (ícono recortado en
  alta resolución, reemplaza el crop borroso de 100×100 que se usaba antes en
  header/footer/favicon) y `logo-huella-full.jpg` (lockup completo ícono +
  wordmark, usado como `og:image`/`twitter:image` para previews al compartir
  el link).
- **No hay dominio ni hosting conectado todavía.** El CNAME apunta a
  `huella40.com.ar` pero falta conectar DNS/hosting. Este repo solo contiene
  el código fuente del sitio.
- **WhatsApp confirmado** (Gustavo, 2026-09-08): `+54 9 2477 33-1767`. Ya está
  como canal activo en la sección de contacto (`wa.me/5492477331767`) y en el
  footer.
- Sin backend, sin formularios con envío de datos, sin tracking. Los CTA
  activos son Instagram (`https://www.instagram.com/huella4.0/`), WhatsApp
  y el email directo (`mailto:gustavoguillaumet@yahoo.com.ar`).

## Estructura

```
index.html          Landing completa (hero, propuesta de valor, productos,
                     sobre la marca, contenido, contacto, footer)
assets/styles.css    Sistema de diseño (tokens de color/tipografía/espaciado
                     + estilos)
assets/logo-huella.jpg       Ícono de marca (recorte cuadrado en alta res
                              del logo oficial), usado en header/footer/favicon
assets/logo-huella-full.jpg  Logo oficial completo (ícono + wordmark),
                              usado como og:image/twitter:image
huella40.jpeg        Logo oficial original tal como lo subió el dueño
                     (1280×1280, fuente de los derivados de arriba)
```

## Cómo verlo local

No requiere instalación. Cualquier servidor estático sirve:

```bash
python3 -m http.server 8080
# abrir http://localhost:8080
```

- **Línea de productos real** (2026-09-11): el dueño subió `Productos/`
  (fotos + `Descripcion de productos.docx`) con los 5 productos oficiales de
  la guía — Trichontrol, Biótica N2, Nutraamin, Humica y Algae — categoría y
  descripción de cada uno. Se reemplazaron las tarjetas genéricas de la
  sección "Línea de productos" por estas 5 (foto propia para las primeras 4,
  Algae sin foto en el material recibido) y se sumó el link a los ensayos de
  Biótica en Fauno (`https://fauno.ai/en/ensayos/?company=Biotica`) en la
  tarjeta de alianza estratégica.

## Pendiente / a confirmar con la marca

- **Dosis, presentaciones y cultivos recomendados por producto**: las
  descripciones son las oficiales provistas por la marca, pero no incluyen
  ficha técnica de dosis/cultivo — confirmar si se quiere sumar.
- **Teléfono**: no se encontró publicado; no se inventó.
- **Dominio y hosting**: a definir. No se tocó DNS ni Cloudflare desde esta
  tarea (fuera de alcance).
- Revisión de copy final con el dueño de la marca antes de publicar.

Diseño y desarrollo: UmanoAI (agente Diseño Web).
