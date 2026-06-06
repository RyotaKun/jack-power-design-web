# Deployment

This site deploys to **Vercel** as a fully static page (no build step).

## Canonical project

- **Vercel project name:** `ryo-power-design`
- **Production URL:** https://ryo-power-design.vercel.app
- **Account:** `sang-7322`
- The local `.vercel/` link (gitignored) already points at this project, so a plain
  `vercel deploy --prod` reuses it. If the link is missing (fresh clone), re-link with
  the `--name` flag below so the project name stays consistent.

## Deploy

```bash
vercel deploy --prod --yes --name ryo-power-design
```

⚠️ **Always use the name `ryo-power-design`** — do not let Vercel auto-generate a
different project name from the repo folder (`jack-power-design-web`).
