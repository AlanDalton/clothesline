# clothesline

**Should you hang out your washing today?**  
Simple, accessible advice on the best times to dry clothes outside using hourly weather data.

---

## Features
- **One‑sentence weekly summary** — quick view of the best drying windows this week.  
- **Daily verdicts** — each day labelled *Good*, *Fair*, or *Bad* for outdoor drying.  
- **Scannable bullet breakdowns** — precipitation, wind, humidity, and best drying window.  
- **Hourly details** — expand any day to see hour‑by‑hour rain, wind, and humidity.  
- **Location search + “Use my location”** — search by town, postcode, or coordinates, or let the browser detect your location.  
- **Responsive and accessible** — semantic HTML, keyboard‑accessible controls, and high‑contrast colours.

---

## How it works
Clothesline uses the free **Open‑Meteo** API to fetch hourly forecasts for the next 7 days.

A drying hour is considered **good** when:
- total precipitation is **< 0.2 mm**
- wind is **< 6 m/s**
- relative humidity is **< 70%**

Daily verdicts and the weekly summary are derived from these hourly conditions.

---

## Usage
1. Clone or download this repository.
2. Put `index.html` at the repository root (or in `docs/` if you prefer to publish from `docs/`).
3. Open `index.html` in a browser to run locally, or enable GitHub Pages for the repository to publish the site.

---

## Accessibility notes
- Semantic headings and landmarks are used for screen readers.  
- Colour contrast meets WCAG AA for body and heading text.  
- The page shows a clear message when JavaScript is disabled and links to a short explanation of JavaScript.  
- Keyboard focus styles and ARIA live regions are used for dynamic updates.

---

## Development
- Static site: plain HTML, CSS, and JavaScript — no build tools required.  
- To test different locations, use the search box, paste coordinates, or click **Use my location**.

---

## Credits
- Weather data: **Open‑Meteo**  
- Icons: Unicode emoji (screen‑reader friendly)  
- I used Microsoft Copilot to create this code.

---

## License
MIT
