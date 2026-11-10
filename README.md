# Mirandel interactive maps

| File | What it is |
|---|---|
| `index.html` | World map (home page). Click rings for lore; click the outlined area to open the regional map. |
| `regional.html` | Amox / Ferry Falls / Everwoods regional map. |
| `amox.html` | City of Amox map. |
| `markets.html` | Amox Market (shops, price finder, party ledger). |

## Editing
Each map page has a settings block at the top of its `<script>`: `MAP_WIDTH_MILES`, `DAY_HOURS`, `MODES` (travel speeds), `LINKS` (buttons on location cards), and `WORLD_URL` / `REGION_URL` (links between pages). Location text lives in the `PLACES` list in the same file.
