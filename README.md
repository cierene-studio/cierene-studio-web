# Cierene Studio — company site

One-page static company website for **Cierene Studio LLC**, used (among other
things) for Apple Developer **organization** enrollment verification.

- Single self-contained file: `index.html` (inline CSS, no build step, no deps).
- Canonical domain: `https://cierenestudio.com`.
- Contact shown: `hello@cierenestudio.com` (change in `index.html` if that
  mailbox is not set up — e.g. to `support@cierenestudio.com`).

## Deploy

Any static host works (it's just one HTML file). Recommended: **Vercel**
(matches the `cierene-studio` GitHub org).

1. Push this repo to GitHub (`gh repo create cierene-studio/cierene-studio-web --public --source=. --push`).
2. In Vercel → New Project → import the repo. Framework preset: **Other**.
   No build command, output directory = repo root.
3. Project → Settings → Domains → add `cierenestudio.com` (+ `www` 301 → apex),
   then point your DNS as Vercel instructs.
4. Confirm `https://cierenestudio.com` loads before submitting it to Apple.

GitHub Pages / Netlify / Cloudflare Pages work equally well — drop the file in,
attach the custom domain.

## Note

- Do not publish a street address.
- **At GiftPebbly launch day:** add the product back to the page — a card with the
  app icon and an "Available on the App Store" link (a shipped product with a real
  store link is far stronger than a lingering "coming soon", which was intentionally
  omitted pre-launch).
