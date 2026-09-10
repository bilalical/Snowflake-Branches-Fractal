# Recursive Fractal Generator: Tree-in-Snowflake

A Python visualization project that generates recursive fractal art by combining a **Koch snowflake** boundary with a **recursive branching tree** structure radiating from its center, rendered with a warm-to-cool gradient color palette on a black background.

## Fractal Type(s) Implemented

- **Koch Snowflake** — a classic recursive fractal built by subdividing each side of an equilateral triangle into four smaller segments and repeating the process, forming the outer boundary of the image.
- **Recursive Branching Tree (Fractal Tree)** — a binary recursive tree where each branch spawns two smaller child branches at an angular offset, forming the inner structure. Multiple layered "tree-stars" (arms radiating from a shared center point at different lengths, angles, and recursion depths) are combined to densely fill the interior.
- **Decorative Core** — a supplementary radial "glow" effect (stacked translucent circles), a 12-pointed star polygon, and scattered sparkle points layered at the center for visual detail.

## Tools, Languages, and Libraries Used

- **Language:** Python 3
- **Libraries:**
  - [`matplotlib`](https://matplotlib.org/) — plotting and rendering (`pyplot`, `patches`)
  - [`numpy`](https://numpy.org/) — trigonometric calculations and coordinate generation
- **Environment:** Jupyter Notebook (also runs as a standalone `.py` script)

## Setup and Run Instructions

### 1. Install dependencies
```bash
pip install matplotlib numpy
```

### 2. Run the script
**Option A — Jupyter Notebook**
1. Open Jupyter Notebook / JupyterLab.
2. Paste the full contents of `fractal.py` into a single cell.
3. Run the cell (`Shift + Enter`).
4. If nothing renders, run `%matplotlib inline` in its own cell first, then re-run.

**Option B — Command line**
```bash
python fractal.py
```
This opens a matplotlib window displaying the fractal.

### 3. Adjust the design (optional)
Key parameters you can tune at the bottom of the script:
- `snow_depth` — recursion depth of the Koch snowflake boundary (higher = more detailed edges, slower).
- `depth` / `n_arms` / `spread` / `shrink` in each `draw_tree_star(...)` call — controls how many branches, how wide they splay, and how quickly they shrink.
- `r_outer` in `draw_core(...)` — size of the glowing center.

## Student Information

- **Name:** Muhammad Bilal
- **Registration Number:** 542332
