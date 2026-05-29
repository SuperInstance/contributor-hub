# contributor-hub

Public contributor directory for the Cocapn Fleet — a Cloudflare Worker that renders contributor profiles and stats.

## What This Gives You

- **Contributor profiles** — name, role, bio, and repo count for each contributor
- **Beautiful landing page** — dark-themed, responsive HTML with gradient accents
- **Health endpoint** — `/health` returns contributor count and status
- **Zero external APIs** — all data rendered server-side from embedded state

## Quick Start

```bash
wrangler deploy

# View the contributor page
open https://contributor-hub.<your-subdomain>.workers.dev/

# Health check
curl https://contributor-hub.<your-subdomain>.workers.dev/health
```

### API

| Method | Path | Description |
|---|---|---|
| `GET` | `/` | Rendered contributor page |
| `GET` | `/health` | JSON status with contributor count |

## How It Fits

A Cocapn Fleet vessel serving the public-facing contributor directory. Part of the SuperInstance ecosystem.

Related repos:
- [cocapn-com](https://github.com/SuperInstance/cocapn-com) — main Cocapn website
- [cocapn-landing](https://github.com/SuperInstance/cocapn-landing) — landing page
- [cocapn-press](https://github.com/SuperInstance/cocapn-press) — press and media

## License

Apache 2.0
