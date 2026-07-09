# Public House Laureles — landing de cervecería de barrio (siembra)

`estado: 🟢 terminada y desplegada` · `en vivo: https://public-house-demo.vercel.app` · `repo: github.com/Kelvmdev/public-house-demo`

**Stack:** Astro 6 (estático) · Tailwind v4 (`@tailwindcss/vite`) · `@astrojs/sitemap` · npm
**Dev:** `npm run dev` → :4321 · **Build:** `npm run build`

## Concepto
Cervecería/gastropub de barrio en Laureles-Estadio, Medellín. Estética cálida noche. Demo de siembra con datos de un negocio real (IG @publichousemedellin). Contenido en `src/data/site.json` (CMS Nivel 1, sin panel: se edita el JSON y se rebuildea).

## Hecho
- Nav sticky + hamburguesa a11y · Hero · **Menú con pestañas** (`role=tab/tabpanel`, datos del JSON) · Ambiente (galería lightbox `<dialog>` nativo) · Sobre · Futbol · Ubicacion + mapa Google anti-hijack (lat/lon) · CTA · Footer · **404 con marca**.
- SEO: title/desc, OG (`public/og.jpg`), canonical, JSON-LD `BarOrPub` con `geo`/`openingHours`/rating, robots.txt, sitemap, apple-touch-icon.
- GEO: `public/llms.txt` (spec oficial) + Faq con schema `FAQPage`.
- Imágenes WebP optimizadas en `public/img/`.
- Conversión: WhatsApp. Desplegado en Vercel (200 OK).

## Pendiente
- nada bloqueante · ajustar pin exacto del mapa si pasa a cliente real (hoy coords aproximadas de barrio).

## Gotchas
- Sin CMS/`/admin`: el contenido vive en `src/data/site.json`, se edita ahí y se rebuildea.
- Es demo de siembra (datos de un local real) — si se contacta al negocio, verificar tel/WhatsApp antes de publicar como suyo.

<sub>actualizado 2026-07-09 · re-clonado desde el repo (la carpeta local previa estaba desfasada).</sub>
