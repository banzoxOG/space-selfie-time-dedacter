# 🛰️ Satellite Pass Tracker

A real-time satellite pass predictor. Enter any NORAD ID, click the map to set your location, and get exact pass times with a live countdown.

## Features

- **Click-to-set location** on a world map
- **Any satellite** — just enter a NORAD ID (e.g. `25544` for ISS, `62713` for SATGUS)
- **Live countdown** to the next pass
- **Max elevation**, duration, and peak time for each pass
- **48-hour window** of upcoming passes
- Fully self-contained — no backend, no API key needed

## Deploy to GitHub Pages

1. Fork or clone this repo
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)` folder
4. Your tracker is live at `https://banzoxog.github.io/space-selfie-time-dedacter/`

## How it works

- TLE orbital data is fetched live from [CelesTrak](https://celestrak.org) via a CORS proxy
- Orbital mechanics computed client-side using [satellite.js](https://github.com/shashwatak/satellite-js)
- No server, no API key, runs entirely in the browser

## Popular NORAD IDs

| Satellite | NORAD ID |
|---|---|
| ISS (Space Station) | 25544 |
| Hubble Space Telescope | 20580 |
| SATGUS | 62713 |
| NOAA 19 | 33591 |
| Tiangong (CSS) | 48274 |
