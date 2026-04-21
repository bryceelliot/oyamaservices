# Oyama Services — Website

Multi-page static website for Oyama Services, a neighborhood vehicle mechanic and inspection shop in Lake Country, BC.

**Business:** Oyama Services
**Address:** 5325 Todd Rd, Lake Country, BC
**Phone:** (250) 862-6369

## Stack

- Plain HTML + CSS (no build step)
- Archivo via Google Fonts
- Vercel for hosting

## Pages

- `index.html` — Home
- `services.html` — Full service list + FAQ
- `about.html` — Shop story + owner
- `service-area.html` — Central Okanagan areas served
- `contact.html` — Phone, map, form

## Design

Ferrari-inspired editorial: chiaroscuro black/white sections, Ferrari Red `#DA291C` reserved for primary CTAs, 2px radii, compact sans typography with uppercase label treatments.

## Before launch — TODO

1. **Replace stock photos** with real shop/owner photography. Current Unsplash placeholders are flagged in the alt text.
2. **Swap domain** — canonical URLs, JSON-LD `@id`, OG URLs, and `sitemap.xml` all reference `https://oyamaservices.ca/`. Search and replace once the real domain is chosen.
3. **Wire the contact form** — in `contact.html`, replace `YOUR_FORM_ID` with the real Formspree form ID from https://formspree.io.
4. **Verify hours** — currently showing `Mon–Fri 8am–5pm · By appointment`.
5. **Owner portrait + name** — placeholder on `about.html`.
6. **Submit sitemap** to Google Search Console after deploy.

## Development

Just open `index.html` in a browser, or:

```bash
npx serve .
```

## Deploy

Configured for Vercel. The `vercel.json` enables clean URLs and adds security headers.

```bash
vercel --prod
```

## SEO

- JSON-LD `AutoRepair` + `LocalBusiness` schema on home and contact
- `BreadcrumbList` on interior pages
- `FAQPage` on services
- `geo.*` and `ICBM` meta tags on every page
- Open Graph and Twitter Card meta
- `sitemap.xml` and `robots.txt`

© Oyama Services
