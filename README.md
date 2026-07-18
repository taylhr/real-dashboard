# real-dashboard

A single-file, zero-dependency dashboard of editable, pseudo-live-updating graphs
and tickers. Everything lives in `index.html`.

## Features

- **Line graphs** with a title, custom X/Y axis names, and custom value ranges.
- **X-axis label formats**: plain numbers, clock times (`18:00` — anchored to the
  real clock), or dates (`07/18/26`).
- **Draggable points** — hover a chart to reveal handles, then drag to reshape the
  line. "Drag falloff" in the config controls how many neighboring points follow.
- **Tickers** — a labeled, live-updating number with prefix/suffix (e.g. `$ … /s`),
  decimals, and an up/down delta indicator.
- **Live simulation** per element: configurable trend (increase/decrease per tick),
  jitter (randomness), and tick interval. Toggle "Live" to freeze an element.
- **Hidden chrome** — per-card controls (reorder grip, config gear, remove) appear
  on hover; the add/export/import dock appears when you hover the bottom-right
  corner. Config panels auto-hide when the mouse leaves the card.
- **Auto-fill layout** — cards resize to fill the window and reflow as elements are
  added or removed. Drag the `⠿` grip to reorder.
- **Import/export** the whole dashboard (including current data) as a `.json` file.
- The layout also autosaves to `localStorage`, and the dashboard title (top left)
  is click-to-edit.
- Light and dark theme follow the OS setting.