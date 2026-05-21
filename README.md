<div align="center">

# Power Design · Web

### Beyond HTML, into the system.

**A long-scroll explainer for the modern website design stack — tokens, shadcn, Tailwind, Radix, OKLCH, motion, theming. The sister doc to [Power Design](https://github.com/ItsssssJack/power-design) (for slides).**

</div>

---

## What it covers

A self-contained HTML explainer (`index.html`) that walks through the canonical layers of a modern website design system, in plain English, with citations to first sources.

| § | Topic | Key sources |
|---:|---|---|
| 01 | **Design tokens** — the atoms | Salesforce / Jina Anne · 2016 · [W3C DTCG](https://www.w3.org/community/design-tokens/) |
| 02 | **shadcn/ui** — your library, not theirs | shadcn (Hunter Reaves) · March 2023 · [ui.shadcn.com](https://ui.shadcn.com) |
| 03 | **Tailwind v4** — utility-first, token-fluent | Adam Wathan · 2017 · v4 Jan 2025 · [tailwindcss.com](https://tailwindcss.com) |
| 04 | **Radix UI** — the accessibility backbone | WorkOS · [radix-ui.com](https://www.radix-ui.com) |
| 05 | **OKLCH color** — 12-step scale, perceptual uniform | Björn Ottosson / Lea Verou |
| 06 | **8-point grid + modular type** | Bryn Jackson · 2015 |
| 07 | **Canonical systems** — Geist · Primer · Carbon · Material · HIG · Atlassian | |
| 08 | **Motion + theming** | Matt Perry · Material 3 motion · next-themes |
| 09 | **The 2026 canonical stack** | Next · Tailwind · shadcn · Radix · Motion · lucide · next-themes |

---

## Open it

```bash
open index.html
```

Or serve locally:

```bash
python3 -m http.server 4174
# → http://localhost:4174
```

---

## Deploy to Vercel

```bash
npx vercel deploy --prod
```

The page is fully static — no build step.

---

## Companion repo

- [Power Design](https://github.com/ItsssssJack/power-design) — Claude skill for slides that don't look like AI made them. Brand DNA × 20 codified design principles.

---

## License

MIT
