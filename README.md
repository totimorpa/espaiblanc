# espaiblanc

Minimal static landing page for Cloudflare.

## Local preview

From this directory:

```bash
python3 -m http.server 4173
```

Then open http://127.0.0.1:4173

## Deploy on Cloudflare

This repo is configured for Cloudflare Workers with static assets.

It serves the site from `public/` and uses a small Worker to:

- redirect `http` to `https`
- redirect `www.espaiblanc.com` to `espaiblanc.com`

The active Worker name is `espaiblanc`.
