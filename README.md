# ReWeather

A small weather dashboard built with React, TypeScript and Shadcn. ReWeather fetches weather, geocoding and air-pollution data from OpenWeather and displays it on an interactive Leaflet map (MapTiler for basemaps). The app is intended as a compact demo / starter for building weather/map-based UIs.

## Features
- Location search (geocoding)
- Current weather + hourly/daily forecasts
- Air pollution (AQI) lookup
- Interactive map with markers and click-to-locate
- Multiple weather overlay tiles (OpenWeather map tiles)
- Responsive UI with light/dark theme support
- Type-checked schemas for API responses

## Tech stack
- Framework: React
- Language: TypeScript
- Bundler / Dev server: Vite
- Data fetching / caching: @tanstack/react-query
- Map rendering: Leaflet + @maptiler/leaflet-maptilersdk
- Weather & geocode APIs: OpenWeather (OneCall, Geocoding, Air Pollution)
- Validation: Zod
- Styling: TailwindCSS

## Quickstart

1. Install dependencies
   - npm
     - `npm install`
   - or pnpm
     - `pnpm install`
   - or yarn
     - `yarn`

2. Add environment variables
   - Create a `.env` file at project root or set env vars in your host.
   - Required:
     - `VITE_API_KEY` — OpenWeather API key
   - Optional (if you want to use your own MapTiler key):
     - `VITE_MAPTILER_KEY` — MapTiler API key (if you replace the hardcoded key)

3. Run locally
   - `npm run dev` (or `pnpm dev` / `yarn dev`)
   - Open http://localhost:5173 (or the URL printed by Vite)
