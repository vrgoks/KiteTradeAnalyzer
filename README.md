# Tradebook — Kite Analysis

A single-file browser tool that turns a Zerodha Kite tradebook export into a visual analysis of your trade history. No backend. No account. No data leaves your device.

---

## What it does

- Parses Zerodha tradebook exports (CSV and XLSX)
- Calculates realised P&L using FIFO cost basis
- Renders a portfolio curve charting cumulative P&L over time
- Shows monthly P&L across every calendar month in your history
- Breaks down win/loss ratio, best and worst trades, most traded stocks
- Trade log accordion — every stock expandable with full individual trade rows
- Download as HTML or PDF (PDF expands all trade rows automatically)

---

## Privacy

Your file never leaves your machine. Everything runs in the browser — no server, no uploads, no analytics, no account required. Close the tab and the data is gone.

---

## How to use

1. Export your tradebook from Zerodha Kite → Console → Reports → Tradebook
2. Open `tradebook-dashboard.html` in any modern browser
3. Drop your CSV or XLSX file onto the upload zone
4. Done

No installation. No dependencies to install. No internet connection required after the page loads.

---

## Tech

| Layer | What |
|---|---|
| Runtime | Vanilla HTML/CSS/JS — single file |
| XLSX parsing | [SheetJS (xlsx.js)](https://sheetjs.com/) via CDN |
| Charts | SVG drawn inline via JS |
| Fonts | Lora, Inter, JetBrains Mono via Google Fonts |
| Deployment | Any static host — Netlify, GitHub Pages, local file |

---

## Limitations

- Realised P&L only — open positions are not included
- FIFO cost basis calculation; does not support LIFO or average cost
- Zerodha Kite export format only
- No mobile optimisation yet

---
