# Findy CSS 2026 — Demos

Live, editable CSS demos for the **Findy CSS 2026** talk (2026-05-14).

Every demo is a standalone static HTML/CSS page.

- **View** → opens the rendered demo on GitHub Pages (instant, no build).
- **Edit** → opens the demo in StackBlitz to run and tweak it in the browser.

**Landing page:** <https://tonkotsuboy.github.io/findy-css-2026-demos/>

## Demos

### 1. Gradient text & color interpolation

| Demo | What it shows | View | Edit |
|------|---------------|------|------|
| `1_gradient-text/1_basic` | `background-clip: text` × `linear-gradient(in oklch …)` | [▶ Live](https://tonkotsuboy.github.io/findy-css-2026-demos/1_gradient-text/1_basic/) | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/1_gradient-text/1_basic) |
| `1_gradient-text/2_oklch-vs-srgb` | `linear-gradient` interpolation compared: sRGB / OkLab / OkLCH | [▶ Live](https://tonkotsuboy.github.io/findy-css-2026-demos/1_gradient-text/2_oklch-vs-srgb/) | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/1_gradient-text/2_oklch-vs-srgb) |
| `1_gradient-text/3_color-vs-named` | `color(srgb …)` vs named/hex — the notation alone switches the interpolation space | [▶ Live](https://tonkotsuboy.github.io/findy-css-2026-demos/1_gradient-text/3_color-vs-named/) | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/1_gradient-text/3_color-vs-named) |

### 2. CSS Anchor Positioning

| Demo | What it shows | View | Edit |
|------|---------------|------|------|
| `2_anchor-position` | `anchor-name` / `position-anchor` + Popover API — a theme-switch menu with zero JS | [▶ Live](https://tonkotsuboy.github.io/findy-css-2026-demos/2_anchor-position/) | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/2_anchor-position) |

### 3. Invoker Commands API

| Demo | What it shows | View | Edit |
|------|---------------|------|------|
| `3_command-commandfor/1_dialog` | `command` / `commandfor` attributes open and close a `<dialog>` with zero JS | [▶ Live](https://tonkotsuboy.github.io/findy-css-2026-demos/3_command-commandfor/1_dialog/) | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/3_command-commandfor/1_dialog) |

### 4. CSS Subgrid

| Demo | What it shows | View | Edit |
|------|---------------|------|------|
| `4_subgrid/1_two-cards` | `grid-template-rows: subgrid` aligns the 4 rows of every card (2 cards) | [▶ Live](https://tonkotsuboy.github.io/findy-css-2026-demos/4_subgrid/1_two-cards/) | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/4_subgrid/1_two-cards) |
| `4_subgrid/2_three-cards` | Same, with 3 cards | [▶ Live](https://tonkotsuboy.github.io/findy-css-2026-demos/4_subgrid/2_three-cards/) | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/4_subgrid/2_three-cards) |
| `4_subgrid/3_form_columns` | `grid-template-columns: subgrid` aligns label / input columns across form rows | [▶ Live](https://tonkotsuboy.github.io/findy-css-2026-demos/4_subgrid/3_form_columns/) | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/4_subgrid/3_form_columns) |

## Structure

Each demo folder contains an `index.html` and `style.css` (plus any images it
references). There is no build step — the folders are served as-is by GitHub
Pages, and StackBlitz auto-detects each one as a static project.

In every `style.css`, the **feature being demonstrated** is placed at the top of
the file under a `★ 技術解説` header; resets, design tokens and decorative
styles follow below. Read the first few lines to see what each demo is about.

## Running locally

```sh
# from the repo root
python3 -m http.server 8000
# then open http://localhost:8000/1_gradient-text/1_basic/
```
