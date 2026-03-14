# Contuling — Roger Garcia Consulting Site

Personal consulting landing page for **Roger Garcia** — Operations, AI & Digital Strategy consultant based in Toronto, helping SMB/SME businesses untangle operations and build systems that scale.

**Live site → [rigarcia07.github.io/contuling](https://rigarcia07.github.io/contuling)**

---

## What this is

A single-file, self-contained HTML landing page with no build tools, no dependencies, and no frameworks. Everything — layout, styles, interactivity — lives in `index.html`. It can be opened directly in a browser or served from any static host.

---

## Files

| File | Description |
|---|---|
| `index.html` | Current production version |
| `index.v1.html` | Archived v1 (original gimmicky design, kept for reference) |
| `LI banner.html` | LinkedIn banner — separate asset |
| `README.md` | This file |

---

## Design decisions

- **No frameworks or build step** — portable, fast, zero maintenance overhead
- **Dark theme** — `#0c0c0e` base, single green accent (`#4ade80`) used sparingly
- **Three-tier text hierarchy** — t1 (16.8:1), t2 (5.8:1), t3 (3.9:1) contrast ratios against background
- **Typography-led** — system-ui + ui-monospace; structure through weight and tracking, not decoration
- **No animations** except subtle hover transitions (`120–130ms`)

### Colour tokens

| Token | Value | Role |
|---|---|---|
| `--bg` | `#0c0c0e` | Page background |
| `--s1` | `#141416` | Card surfaces |
| `--s2` | `#1c1c1f` | Nested elements |
| `--t1` | `#edeef0` | Primary text — headings, key values |
| `--t2` | `#8a8b96` | Secondary text — body, descriptions |
| `--t3` | `#6e6f79` | Tertiary text — labels, meta, hints |
| `--green` | `#4ade80` | Accent — CTA and one headline line only |

---

## Making changes

Open `index.html` in any editor. All CSS is in `<style>` in the `<head>`. All JS is in a `<script>` at the bottom of `<body>`.

Things most likely to need updating:
- **Headline / body copy** — `<!-- HERO -->` section
- **Services** — `<!-- SERVICES -->` section (`service-list`)
- **Proof points** — `<!-- Proof -->` card in the sidebar (`proof-list`)
- **Contact email** — two occurrences of `rgarcia@ikg-grp.com` (footer link + `openEmail()` JS function)
- **LinkedIn URL** — search for `linkedin.com/in/rogergarcia/`

---

## Hosting

Served via **GitHub Pages** from the `main` branch root.

To deploy a change: commit to `main` and push. Pages rebuilds automatically within ~60 seconds.

```bash
git add index.html
git commit -m "your message"
git push
```

---

## Versions

| Version | File | Notes |
|---|---|---|
| v2 (current) | `index.html` | Clean typographic redesign — no gradients, no glow |
| v1 | `index.v1.html` | Original — card-based with green glow effects |
