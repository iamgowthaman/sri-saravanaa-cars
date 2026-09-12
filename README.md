# Sri Saravanaa Cars — Website

A static website (single self-contained HTML file, no build step, no server required) for Sri Saravanaa Cars, a used-car dealership in Rasipuram, Namakkal district, Tamil Nadu.

## Structure

```
index.html          Everything — markup, styles, and logic for all pages
assets/img/logo.jpg  Your logo (used as the browser tab icon and site brand mark)
```

The site is a single page with client-side navigation (Home / Sell Your Car / About / Contact) — the URL changes (`#/`, `#/sell`, `#/about`) but nothing reloads. This makes it trivially portable: drop the two files above onto *any* static host and it works, no server configuration needed.

## What's already set up

- **Contact info**: WhatsApp `+91 94427 49039`, Call `+91 94436 02022`, email `srisaravanaacars@gmail.com`
- **Address**: Tiruchengode Main Road, Near PSK Complex, Koonavelampatti, Andagalur Gate Flyover, Kurukkapuram, Tamil Nadu – 637401
- **Map pin**: confirmed from your Google Maps listing (11.4436236, 78.1494674) — the "Get Directions" button links straight to it
- **Logo**: used as the header/footer brand mark and the browser tab icon
- **Light / dark theme toggle** (top right, remembers the visitor's choice)
- **Tamil / English language toggle** (EN / தமிழ் — switches all text including the WhatsApp message it pre-fills)
- **Sell Your Car form** — opens WhatsApp with the visitor's car details pre-filled, no backend needed

## Still placeholder / to confirm

- **Business hours** — currently shows Mon–Sat 9:30 AM–8:00 PM, Sun 10:00 AM–6:00 PM. Update if different.
- **About page story paragraph** — currently generic dealership copy, marked with an "Owner note" tag. Replace with your real story whenever you're ready.

## To edit anything

Everything lives in `index.html`. Near the top of the `<script>` section:

- `SITE_CONFIG` — phone, WhatsApp, email, map link
- `ADDRESS` — address text (English and Tamil versions)
- `HOURS` — business hours (English and Tamil versions)
- `I18N` — every piece of visible text on the site, in both languages (search for the English text you want to change, then update its Tamil pair alongside it)

## Running it locally

No install needed — just open `index.html` in a browser by double-clicking it, or:

```
open index.html
```

## Deploying for real

Drag-and-drop the whole `sri-saravanaa-cars` folder onto any of these free hosts and you're live:

- **Netlify Drop** — app.netlify.com/drop (no signup needed for a first deploy)
- **Vercel** — vercel.com
- **GitHub Pages** — push to a repo, enable Pages in settings

No database, no backend, no monthly server cost. Add a custom domain (e.g. `srisaravanaacars.in`) from any registrar afterward and point it at whichever host you choose.

## Coming later

A color theme pass to match the red/black/white of your logo more closely (currently uses a green/steel-grey palette). This is intentionally deferred — ask whenever you're ready.
