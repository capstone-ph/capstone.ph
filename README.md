# capstone.ph — Production Build Repository

This repository hosts the compiled static production build of **Capstone Solutions Inc.** (`https://capstone.ph`), served via GitHub Pages.

> **Important:** Do not edit HTML, CSS, or `_astro/` files directly in this repository. All source code, content, and design tokens are maintained in the private Astro source repository and published here via `scripts/deploy.sh`.

---

## Included Deployment Files

- `CNAME` — Custom domain binding (`capstone.ph`)
- `.nojekyll` — Disables GitHub Pages Jekyll processing so Astro's `_astro/` bundled assets are served intact
- `index.html` & route folders (`/about/`, `/services/`, `/solutions/`, `/industries/`, `/clients/`, `/contact/`)
- `sitemap-index.xml`, `sitemap-0.xml`, `robots.txt`, `favicon.svg`
- `_astro/` — Compiled CSS, optimized WebP logo assets, and self-hosted fonts

---

## GitHub Pages & DNS Setup

### Repository Settings
1. Go to **Settings → Pages**.
2. Set **Source** to **Deploy from a branch** and choose the published branch (`gh-pages` or `main`), folder `/ (root)`.
3. Confirm **Custom domain** is `capstone.ph`.
4. Enable **Enforce HTTPS** once GitHub finishes issuing the TLS certificate.

### DNS Records (`capstone.ph`)
| Type | Host | Value |
| :--- | :--- | :--- |
| `A` | `@` | `185.199.108.153` |
| `A` | `@` | `185.199.109.153` |
| `A` | `@` | `185.199.110.153` |
| `A` | `@` | `185.199.111.153` |
| `AAAA` *(optional)* | `@` | `2606:50c0:8000::153` |
| `AAAA` *(optional)* | `@` | `2606:50c0:8001::153` |
| `AAAA` *(optional)* | `@` | `2606:50c0:8002::153` |
| `AAAA` *(optional)* | `@` | `2606:50c0:8003::153` |
| `CNAME` | `www` | `capstone-ph.github.io` |
