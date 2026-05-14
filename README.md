# Findy CSS 2026 — Demos

Live, editable CSS demos for the **Findy CSS 2026** talk (2026-05-14).

Every demo is a standalone static HTML/CSS page. Click an **Open in StackBlitz**
badge to run and edit it in the browser — no install, no sign-in required.

## Demos

### 1. Gradient text & color interpolation

| Demo | What it shows | Playground |
|------|---------------|------------|
| [`1_gradient-text/1_basic`](./1_gradient-text/1_basic/) | `background-clip: text` × `linear-gradient(in oklch …)` | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/1_gradient-text/1_basic) |
| [`1_gradient-text/2_oklch-vs-srgb`](./1_gradient-text/2_oklch-vs-srgb/) | `linear-gradient` interpolation compared: sRGB / OkLab / OkLCH | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/1_gradient-text/2_oklch-vs-srgb) |
| [`1_gradient-text/3_color-vs-named`](./1_gradient-text/3_color-vs-named/) | `color(srgb …)` vs named/hex — the notation alone switches the interpolation space | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/1_gradient-text/3_color-vs-named) |

### 2. CSS Anchor Positioning

| Demo | What it shows | Playground |
|------|---------------|------------|
| [`2_anchor-position`](./2_anchor-position/) | `anchor-name` / `position-anchor` + Popover API — a theme-switch menu with zero JS | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/2_anchor-position) |

### 3. Invoker Commands API

| Demo | What it shows | Playground |
|------|---------------|------------|
| [`3_command-commandfor/1_dialog`](./3_command-commandfor/1_dialog/) | `command` / `commandfor` attributes open and close a `<dialog>` with zero JS | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/3_command-commandfor/1_dialog) |

### 4. CSS Subgrid

| Demo | What it shows | Playground |
|------|---------------|------------|
| [`4_subgrid/1_two-cards`](./4_subgrid/1_two-cards/) | `grid-template-rows: subgrid` aligns the 4 rows of every card (2 cards) | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/4_subgrid/1_two-cards) |
| [`4_subgrid/2_three-cards`](./4_subgrid/2_three-cards/) | Same, with 3 cards | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/4_subgrid/2_three-cards) |
| [`4_subgrid/3_form_columns`](./4_subgrid/3_form_columns/) | `grid-template-columns: subgrid` aligns label / input columns across form rows | [![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/tonkotsuboy/findy-css-2026-demos/tree/main/4_subgrid/3_form_columns) |

## Structure

Each demo folder contains an `index.html` and `style.css` (plus any images it
references). StackBlitz auto-detects the folder as a static project and serves
it directly — there is no build step.

In every `style.css`, the **feature being demonstrated** is placed at the top of
the file under a `★ 技術解説` header; resets, design tokens and decorative
styles follow below. Read the first few lines to see what each demo is about.

## Running locally

```sh
# from the repo root
python3 -m http.server 8000
# then open http://localhost:8000/1_gradient-text/1_basic/
```
