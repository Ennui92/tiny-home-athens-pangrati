# Mikró — Pangrati Studio website

A self-contained, single-page website for the Airbnb listing
[*Mikró — a tiny studio in Pangrati, Athens*](https://www.airbnb.co.uk/rooms/1148249899225863736),
built from the listing's own photos and description. No framework, no build
step — plain static files, hosted free on **GitHub Pages**.

Live URL (once Pages is enabled): **https://ennui92.github.io/tiny-home-athens-pangrati/**

```
.
├── index.html      ← the whole site (HTML + CSS + JS inline)
├── og-image.png    ← 1200×630 social-share card
├── robots.txt      ├─ SEO
├── sitemap.xml     ┘
├── .nojekyll       ← serve files as-is (no Jekyll processing)
├── images/         ← 9 optimised photos (.webp, ~744 KB total)
└── .github/workflows/deploy-pages.yml   ← auto-deploys to GitHub Pages on push
```

## Going live on GitHub Pages

1. Push this folder to the repo's `main` branch (the site files live at the repo root).
2. In the repo: **Settings → Pages → Build and deployment → Source → GitHub Actions**.
3. The included workflow deploys automatically on every push to `main`.
   Your site goes live at `https://ennui92.github.io/tiny-home-athens-pangrati/`.

> If you name the repo something other than `mikro-athens`, update the URL in
> `index.html` (canonical, Open Graph, JSON-LD), `robots.txt` and `sitemap.xml`
> to match — they're all currently set to `ennui92.github.io/tiny-home-athens-pangrati`.

## Make it findable by name on Google (the SEO)

Already built in: keyword-rich title + description, canonical, geo tags,
Open Graph + Twitter cards, a custom social image, `robots.txt` + `sitemap.xml`,
and schema.org structured data — a **`LodgingBusiness`** with your 4.65★ rating
and reviews (⭐ rich results), plus a **`FAQPage`** and **`WebSite`** entity.

Two steps only you can do:

1. **Match the name.** The site is branded **“Mikró”**. Set your **Airbnb
   listing title** to start with *Mikró* so a guest who sees the name and
   searches it lands here. (Prefer a different name? Tell me and I'll rebrand
   the whole site to match.)
2. **Get it indexed.** Add the live URL to
   [Google Search Console](https://search.google.com/search-console),
   submit `sitemap.xml`, and click **Request indexing**. Because
   “Mikró · Pangrati” is a near-unique phrase, it should rank #1 for that exact
   search within days.

Validate the structured data at <https://search.google.com/test/rich-results>.
