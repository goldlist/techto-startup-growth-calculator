# Startup Growth Calculator

A modern, mobile-first reimagining of Trevor Blackwell's startup funding calculator — built for founders by [TechTO](https://techto.org).

**Live:** [growth.techto.org](https://growth.techto.org)

---

## What it does

Enter your monthly revenue, expenses, and growth rate. The calculator tells you whether you're **Default Alive** (you'll reach profitability on current trajectory) or **Default Dead** (you won't) — and shows exactly how long until profitability, how much capital you'll need, and how you compare to real Canadian and global company milestones (Wealthsimple, Shopify, Stripe, Apple).

Concept from Paul Graham's essay: [Default Alive or Default Dead?](https://www.paulgraham.com/aord.html)

---

## Features

- **Draggable SVG chart** (desktop) — drag the revenue, expense, and growth handles directly on the chart
- **Slider chart** (mobile) — touch-friendly sliders with a compact live chart
- **3-tier verdict** — Default Alive (green), Needs Runway (yellow), Danger Zone / Default Dead (red)
- **Company milestones** — see when you'd hit Wealthsimple, Shopify, Stripe, and Apple run rates
- **Shareable links** — state is encoded in the URL, no backend needed

---

## Inspiration & Attribution

Inspired by **[Trevor Blackwell's startuptools](https://gitlab.com/tlb/startuptools)** (MIT License). The core math — exponential revenue growth against expenses on a log scale — comes directly from his original calculator at [growth.tlb.org](https://growth.tlb.org). We built a new frontend from scratch but the underlying model is his.

---

## Stack

- React 18 (CDN, no build step)
- Tailwind CSS (CDN)
- Pure SVG chart
- URL-encoded state (shareable, no backend)
- TechTO brand fonts and nav (Webflow export)

## Running locally

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

---

*Built by [TechTO](https://techto.org) for founders.*
