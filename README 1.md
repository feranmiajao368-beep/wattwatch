# ⚡ WattWatch — Home Energy Monitor

A clean, browser-based energy usage tracker for homes, apartments, offices, farms, and more. No backend, no account — runs entirely in your browser.

**[🌐 Live Demo →](https://feranmiajao368-beep.github.io/wattwatch)**

---

## Features

- **Dashboard** — daily kWh, monthly cost, peak appliance, and CO₂ comparison
- **Appliance manager** — add appliances by wattage and daily usage hours; auto-calculates monthly cost
- **Visual charts** — weekly bar chart, category donut chart, 6-month trend line
- **Benchmark comparison** — compare your usage against eco, average, and high-consumer households
- **Energy-saving tips** — 8 practical tips with estimated savings
- **Settings** — set your electricity rate, currency (USD, NGN, EUR, GBP, INR, CAD, AUD), monthly budget, and environment type
- **Persistent storage** — all data saved to `localStorage`, survives page refresh
- **Mobile-friendly** — responsive layout works on phones and tablets

---

## Getting Started

### Option 1: GitHub Pages (recommended)

1. Fork or clone this repo
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)` folder
4. Visit `https://feranmiajao368-beep.github.io/wattwatch`

### Option 2: Run locally

Just open `index.html` in any browser — no build step, no dependencies to install.

```bash
git clone https://github.com/feranmiajao368-beep/wattwatch.git
cd wattwatch
open index.html   # macOS
# or
start index.html  # Windows
```

---

## Tech stack

| Layer | Tech |
|---|---|
| UI | Vanilla HTML/CSS/JS |
| Charts | [Chart.js 4.4](https://www.chartjs.org/) via CDN |
| Storage | Browser `localStorage` |
| Hosting | GitHub Pages |

No frameworks, no build tools, no backend — a single `index.html` file.

---

## Project structure

```
wattwatch/
└── index.html    # Everything in one file
└── README.md
```

---

## Customization

Open `index.html` and find the `BENCHMARKS` object to adjust baseline comparisons:

```js
const BENCHMARKS = {
  home: 900,        // kWh/month
  apartment: 600,
  office: 1500,
  shop: 2000,
  warehouse: 4000,
  farm: 800
};
```

Change `0.43` (kg CO₂ per kWh) in the dashboard section to match your country's grid emission factor.

---

## License

pay to use, fork, and modify.

---

*Built with ❤️ to help people understand and reduce their energy footprint.*
