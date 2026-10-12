# Aurionpro — Market Intelligence Dashboard Portal

A single-page portal that indexes **70 Coherent Market Insights research dashboards**
across 4 market verticals, with tabs, instant search, and card/table views.

## The file

[`Aurionpro-Dashboard-Portal.html`](Aurionpro-Dashboard-Portal.html) is fully
self-contained — no build step, no dependencies, no server. Open it in any browser,
or host it anywhere static.

## Coverage

| Vertical | Dashboards |
|---|---|
| Banking & Fintech | 20 |
| AI & Digital CX | 16 |
| Mobility & GovTech | 16 |
| Data Center & Cloud | 18 |
| **Total** | **70** |

## Features

- **Tabs per vertical** plus an "All Markets" view that groups cards under colour-coded headings.
- **Instant search** across all 70 markets — press `/` to focus, `Esc` to clear.
- **Cards / Table toggle**; the table view doubles as the accessible fallback.
- **Hero panel** listing every vertical, each row jumping straight to that tab.
- **Credibility & Awards** sections and the full CMI footer, linking to the live site.
- Responsive down to mobile; respects `prefers-reduced-motion`.

Every dashboard link opens in a new tab.

## Source of truth

Dashboard names and URLs come from [`Aurionpro Dashboard Links.xlsx`](Aurionpro%20Dashboard%20Links.xlsx)
(one sheet per vertical). The HTML was generated from that workbook programmatically
rather than transcribed, and the build asserted 4 verticals, 70 rows, and a valid URL
on every row. To change the dashboard list, edit the workbook and regenerate.

## Design notes

The four vertical colours are a colourblind-safe categorical set, validated for
CVD separation and contrast. Colour is never the only cue — each vertical always
travels with its name and label, so the portal stays readable without it.
