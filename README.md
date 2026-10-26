# Cluster — BattleTech damage resolver

Resolves BattleTech cluster weapon damage: cluster roll, modifiers, hit locations and a running tally. A single-page PWA (works offline via `sw.js`).

## Hosting and access

- **Live:** https://bt-cluster-resolver.torquemada.uk
- **Cloudflare Worker:** `drop-1a1795af-46f` — static assets only, no server code.
- **Access:** public, no Cloudflare Access. Karl, 26 Oct 2026: keep it.
- **Source:** `public/` was recovered on 26 Oct 2026 by downloading the live site, because the source previously existed only on Cloudflare. It is byte-for-byte what was being served.

## Deploy

```
npx wrangler deploy
```

`wrangler.jsonc` uses the existing Worker name and custom domain, so a deploy updates the live site in place.
