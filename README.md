# Mirandel interactive maps

| File | What it is |
|---|---|
| `index.html` | World map (home page). Click rings for lore; click the outlined area to open the regional map. |
| `regional.html` | Amox / Ferry Falls / Everwoods regional map. |
| `amox.html` | City of Amox map. |
| `markets.html` | Amox Market (shops, price finder, party ledger). |

## Publish with GitHub Pages
1. Put all four `.html` files in the root of the repo (keep the names; `index.html` must stay `index.html`).
2. Repo **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main`, folder = `/ (root)`.
3. Your site: `https://USERNAME.github.io/REPO/` (other pages: `.../amox.html`, `.../regional.html`, `.../markets.html`).

## Editing
Each map page has a settings block at the top of its `<script>`: `MAP_WIDTH_MILES`, `DAY_HOURS`, `MODES` (travel speeds), `LINKS` (buttons on location cards), and `WORLD_URL` / `REGION_URL` (links between pages). Location text lives in the `PLACES` list in the same file.
