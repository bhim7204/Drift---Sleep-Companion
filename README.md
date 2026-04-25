# Drift — Sleep Companion

A lightweight static sleep analytics dashboard built with HTML, CSS, and JavaScript.

The app visualizes 28 days of wearable sleep and activity data using interactive charts and metrics, helping users review trends, sleep stages, correlations, and nightly recovery performance.

## Features

- Dark/light theme toggle
- Mobile-friendly sidebar navigation
- Dashboard view with sleep score, duration, efficiency, HRV, and recovery insights
- Trends view showing bedtime consistency, HRV, resting heart rate, and sleep efficiency
- Sleep stages analysis with nightly stage distribution and average breakdown
- Daily sleep log and correlation analysis between sleep metrics and activity
- Built on static files with Chart.js for visualization

## Files

- `index.html` — main app shell and page layout
- `style.css` — primary component styling and layout
- `base.css` — foundational resets and shared design tokens
- `app.js` — app logic, page routing, chart rendering, and UI behavior
- `data.js` — sample sleep and activity dataset used by the dashboard

## Getting Started

### Prerequisites

No build tools are required. The app runs in any modern browser.

### Run locally

1. Open `index.html` in your web browser.
2. Or serve the folder using a simple local server:

```bash
# Python 3
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Usage

- Use the sidebar to navigate between Dashboard, Trends, Sleep Stages, Correlations, and Sleep Log.
- Click the theme toggle button to switch between dark and light modes.
- The charts are rendered using Chart.js, and the app updates metrics based on the sample `SLEEP_DATA` and `ACTIVITY_DATA` arrays.

## Data

The repository ships with sample wearable data in `data.js`:

- `SLEEP_DATA` — nightly sleep metrics such as score, efficiency, deep/REM/light sleep, HRV, heart rate, latency, wake-ups, and more
- `ACTIVITY_DATA` — daily activity metrics including steps, distance, calories, activity score, and recovery score

## Customize

- Add or modify records in `data.js` to change the displayed sleep dataset.
- Update `app.js` to change chart behavior, calculations, or page content.
- Adjust styling in `style.css` and `base.css` for branding or layout changes.

## Dependencies

- `Chart.js` is loaded via CDN in `index.html`.

## Notes

This repository is a static frontend prototype for sleep data visualization and does not include any backend or data persistence.
