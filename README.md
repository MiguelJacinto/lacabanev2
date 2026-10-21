# La Cabane — website prototypes

Two looks, one static site. No build step, no dependencies.

- `index.html` — **Prototype A: Classic** (logo, off-white, brand-colour accents)
- `kitchen-table/index.html` — **Prototype B: Kitchen Table** (warm paper, tomato & lemon, ink sketches)
- `menu.pdf` — the menu, shared by both ("Open the full menu" opens it in a new tab)

Each page links to the other in its footer.

## Publish on GitHub Pages
1. Create a repository (e.g. `la-cabane-site`) and upload this whole folder, keeping the structure.
2. Settings → Pages → "Deploy from a branch", branch `main`, folder `/ (root)` → Save.
3. After a minute:
   - Prototype A: `https://<user>.github.io/la-cabane-site/`
   - Prototype B: `https://<user>.github.io/la-cabane-site/kitchen-table/`

## What works out of the box
- Every "Reserve" / phone button is a `tel:+351289313819` link (opens the dialer on phones).
- "Open the full menu (PDF)" opens `menu.pdf` in a new tab — keep it at the root with that name.
- EN / PT / FR switcher, review filters, dish slideshow, open/closed status: plain HTML/CSS/JS.
- Fonts come from Google Fonts; everything else is embedded in the files.

## Updating
- New menu: replace `menu.pdf` (same name).
- Photos: in each `index.html`, every `<div class="ph">` is an image slot — replace its contents with `<img src="photos/your-photo.jpg" alt="…">`. In Prototype B the slots hold the ink sketches and the photographer briefs.
