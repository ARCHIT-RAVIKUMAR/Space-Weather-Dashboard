# Space Weather Dashboard

A simple web dashboard that shows current solar and space-weather conditions using live NOAA data.

**Live link:** https://archit-ravikumar.github.io/Space-Weather-Dashboard/

## What it shows

- Planetary Kp index (geomagnetic activity)
- Solar wind speed, density and IMF Bz
- Solar X-ray flux and flare class
- Sunspot number and F10.7 radio flux
- Recent NOAA alerts and events
- A short note on how space weather affects Earth and space missions

## Data sources

All data comes from the NOAA Space Weather Prediction Center public JSON API (`services.swpc.noaa.gov`). No API key is needed. The page fetches it in the browser and refreshes every 5 minutes.

- Kp index: `/products/noaa-planetary-k-index.json`
- Solar wind speed and density: `/json/rtsw/rtsw_wind_1m.json`
- IMF Bz: `/json/rtsw/rtsw_mag_1m.json`
- X-ray flux and flare class: `/json/goes/primary/xrays-6-hour.json`
- Sunspot number and F10.7: `/json/solar-cycle/observed-solar-cycle-indices.json`
- Alerts: `/products/alerts.json`

## One possible impact of space weather

Satellite loss from atmospheric drag. In February 2022, a minor geomagnetic storm heated and expanded Earth's upper atmosphere, increasing drag on newly launched Starlink satellites. SpaceX lost about 38 of them before they could reach a safe orbit.

## Credit

Data from NOAA / NWS Space Weather Prediction Center.
