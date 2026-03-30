# woolworths-z

A single-page Leaflet webapp that finds the shortest road route from any NZ address to the nearest Woolworths supermarket.

## Features

- **Address search** — type any NZ address and hit *Find Nearest Store* (or press Enter)
- **Live store data** — fetches all Woolworths / Countdown locations in NZ from the [Overpass API](https://overpass-api.de/); falls back to a built-in list of 25 major stores if the API is unavailable
- **Road routing** — uses the public [OSRM](https://project-osrm.org/) demo server to calculate and draw the actual road route on the map
- **Transport modes** — Walk 🚶 · Bike 🚲 · Drive 🚗 (switching mode re-routes automatically)
- **Distance units** — m · km · miles · furlongs · **furlongs per fortnight** 🐎 (fun unit: shows your speed in fur/fortnight alongside the travel time)
- **Icon toggle** — switch all store markers between the Woolworths green-W hexagon and a Dragon Ball Z orange-Z hexagon 🐉

## Usage

Open `index.html` in any modern browser (internet connection required for map tiles, geocoding, routing, and store data).

## Data sources

| Service | Purpose |
|---------|---------|
| [OpenStreetMap](https://www.openstreetmap.org/) | Map tiles |
| [Nominatim](https://nominatim.openstreetmap.org/) | Address geocoding |
| [OSRM demo](https://router.project-osrm.org/) | Road routing |
| [Overpass API](https://overpass-api.de/) | Woolworths store locations |
