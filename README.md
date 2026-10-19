# Moonfleet apps

Guest apps for Moonfleet, a holiday let in Bracklesham Bay, West Sussex, managed by Wellies & Windbreaks.

## Stay planner

`stay-planner/index.html`

A phone-friendly planner for guests. They enter their arrival and leaving dates and get:

- a grid of outdoor activities against each day of the stay, rated Go / Maybe / No with the best time window
- tick boxes to choose which activities appear (swimming, paddleboarding, bodyboarding, kitesurfing, fossil hunting, bike ride to West Wittering, kayaking and crabbing at Dell Quay, RSPB walks, West Wittering Beach)
- a day view with a beach scene, wind and conditions, a tide chart with sunrise and sunset, and a suggested timed plan
- their own morning / afternoon / evening plan, saved on their phone and shareable as text

Arrival day only plans from 16:00 and leaving day stops at 10:00.

### Data

The live forecast, waves, sea temperature and tides come from [Open-Meteo](https://open-meteo.com) (free, no API key). Tide times are modelled, so they are approximate on this coast. If the forecast can't be reached, the page falls back to a saved forecast for 18–24 October 2026.

Everything is in one self-contained HTML file with no build step.

## Hosting

Turn on GitHub Pages: **Settings → Pages → Deploy from a branch → `main` / root**. The planner is then at:

`https://andycooper-bot.github.io/Moonfleet-apps/`

The top-level `index.html` forwards to the stay planner, so that link is the one to put on a QR code in the house.

Nothing private (Wi-Fi password, key box codes) should go in this repo, as it is public.
