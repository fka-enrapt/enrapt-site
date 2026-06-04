# enrapt.io

Marketing/personal website for Fabian Alsultany — Strategic Advisor, Fractional COO, Business Development Executive — under the ENRAPT brand. Hosted on **GitHub Pages** at **https://enrapt.io**.

## Per-page URLs (important)
The site has **clean per-page URLs**, one real file per route, so each page has its own crawlable title/description/Open-Graph card:

| URL | File |
|---|---|
| https://enrapt.io/ | `index.html` |
| https://enrapt.io/about/ | `about/index.html` |
| https://enrapt.io/services/ | `services/index.html` |
| https://enrapt.io/work/ | `work/index.html` |
| https://enrapt.io/expertise/ | `expertise/index.html` |
| https://enrapt.io/industries/ | `industries/index.html` |
| https://enrapt.io/why/ | `why/index.html` |
| https://enrapt.io/contact/ | `contact/index.html` |

Each file is self-contained (fonts, images, logo, styles embedded) and boots the app to its page from the URL path. In-app clicks use the History API for instant navigation; direct visits / shared links / crawlers load the correct file directly.

## Other files
| File | Purpose |
|---|---|
| `404.html` | Fallback for unknown paths (noindex); renders the home shell. |
| `CNAME` | `enrapt.io` — binds the custom domain. Do not delete. |
| `favicon.svg`, `apple-touch-icon.png` | Icons (referenced at site root). |
| `enrapt-og.png` | Open Graph / social share image (1200×630). |
| `robots.txt`, `sitemap.xml` | SEO. Sitemap lists all 8 URLs. |

## Deploying an update
Upload the changed files to the repo (keeping the folder structure) and **Commit**. GitHub Pages publishes in ~1 minute. To update everything, upload the whole folder, overwriting. No build step.

## ⚠️ When you ADD or RENAME a page
You must keep four things in sync: (1) the React route in `App.jsx`/`Primitives.jsx`, (2) the generated folder/`index.html`, (3) `sitemap.xml`, (4) the nav links. The design project regenerates all of these — make page changes there, not by hand-editing these built files.

## Contact form
Wired to Formspree (`https://formspree.io/f/xaqznyrj`) → emails fka@enrapt.io. The first live submission triggers a one-time Formspree confirmation email; click it once to activate.
