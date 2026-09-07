# votebrianparker.com

Campaign website for **Brian Parker**, Director, Moulton Niguel Water District.
General election: Tuesday, November 3, 2026.

## Structure

Single-page static site. No build step, no dependencies.

```
index.html      # entire site — markup + inline CSS + 12 lines of JS
img/            # lockup, candidate portrait, sign art
```

Fonts load from Google Fonts. Everything else is local.

## Local preview

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Before launch

- [ ] **FPPC I.D.** — the footer disclaimer reads `FPPC I.D. pending`. Legally required; search `class="todo"` in `index.html`.
- [ ] **Years in Laguna Niguel** — `[NUMBER]` placeholder in the last About paragraph. Same `todo` class.
- [ ] **Social share card** — 1200×630 as `img/og-card.jpg`, then uncomment the `og:image` meta tag in `<head>`. Without it the URL previews as a bare link in text messages.

## Optional

A second photo slot in the About column is commented out in the markup — uncomment one line and add `img/parker-about.jpg`.

## Deployment

GitHub Pages, `main` branch, root.

---

Paid for by Parker for Moulton Niguel 2026.
