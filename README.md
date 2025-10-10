# Grid Maker — CSCI‑39548 Assignment 2

An interactive grid builder that lets you add/remove rows and columns, pick a color, click cells to paint them, and use bulk actions to fill or clear the grid.

### Live Demo
https://shanglichen.github.io/CSCI-39548-Assignment-2/

### Features
- Add/remove rows and columns dynamically.
- Select a color from the dropdown (Red, Blue, Green, Yellow).
- Click any cell to color it with the selected color.
- Fill Uncolored: color only cells that are currently white.
- Fill All: color every cell to the selected color.
- Clear: reset all cells to white.

### How It Works
- `Add Row` creates a new row; if it’s the first row, it also creates the first column.
- `Add Col` adds a new column to all existing rows; if the grid is empty, it creates the first cell.
- `Remove Row` deletes the last row; when the last row is removed, the column count resets.
- `Remove Col` deletes the last column; removing the last column clears the grid entirely.
- `SELECT` a color, then click cells to paint them; bulk actions respect the selected color.

### Local Setup
- Open `CSCI-39548-Assignment-2/index.html` in any modern browser.
- Files:
  - `index.html` — layout and controls.
  - `styles.css` — styling for buttons, grid, and responsive tweaks.
  - `script.js` — core grid logic and color actions.

### Tech Stack
- HTML, CSS, JavaScript (no frameworks)

### Notes
- Cells are considered “uncolored” when their background is empty or white; `Fill All Uncolored` only affects those cells.
- Console logs the currently selected color for debugging when changed.
