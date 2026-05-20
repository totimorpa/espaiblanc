# espaiblanc

Minimal static landing page for Cloudflare.

## Local preview

From this directory:

```bash
python3 -m http.server 4173
```

Then open http://127.0.0.1:4173

## Deploy on Cloudflare

This repo is configured for Cloudflare's Git-connected static deployment flow using Wrangler static assets on the `espaiblanc` Worker.

When connecting the repository in Cloudflare:

- framework preset: none
- build command: leave the default Cloudflare command if it is auto-filled
- production branch: `main`

Cloudflare will serve the static files from `public/` via `wrangler.jsonc`.
