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
  captura directa del perfil: email de contacto (`gustavoguillaumet@yahoo.com.ar`)
  y zona de operación (Guatimozín, Córdoba, Argentina).
- **No hay dominio ni hosting conectado todavía.** Este repo solo contiene el
  código fuente del sitio.
- Sin backend, sin formularios con envío de datos, sin tracking. Los CTA
  activos son Instagram (`https://www.instagram.com/huella4.0/`) y el email
  directo (`mailto:gustavoguillaumet@yahoo.com.ar`).

## Estructura

```
index.html          Landing completa (hero, propuesta de valor, productos,
                     sobre la marca, contenido, contacto, footer)
assets/styles.css    Sistema de diseño (tokens de color/tipografía/espaciado
                     + estilos)
assets/logo-huella.jpg  Foto de perfil real de @huella4.0 (asset de marca)
```

## Cómo verlo local

No requiere instalación. Cualquier servidor estático sirve:

```bash
python3 -m http.server 8080
# abrir http://localhost:8080
```

## Pendiente / a confirmar con la marca

- **WhatsApp u otro canal de contacto directo**: no está confirmado
  públicamente, se dejó marcado como "pendiente" en la sección de contacto.
- **Detalle técnico de productos** (dosis, composición, cultivos recomendados
  por producto): la landing resume lo que la marca comunica en Instagram
  (p. ej. "NUTRIAAMIN + HUMICA HF", tensoactivos, Biótica N2 + micorrizas,
  guía de 5 productos), pero no reemplaza ficha técnica oficial.
- **Teléfono**: no se encontró publicado; no se inventó.
- **Dominio y hosting**: a definir. No se tocó DNS ni Cloudflare desde esta
  tarea (fuera de alcance).
- Revisión de copy final con el dueño de la marca antes de publicar.

Diseño y desarrollo: UmanoAI (agente Diseño Web).
