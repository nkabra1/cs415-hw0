# Weather

A single-page mobile weather prototype. Shows current temperature, whether you need an
umbrella in the next few hours, air quality index + humidity, and wind speed/direction — all on
one screen, no scrolling.

Live data comes from [Open-Meteo](https://open-meteo.com/) (forecast, air quality, and
geocoding) plus [BigDataCloud](https://www.bigdatacloud.com/free-api/free-reverse-geocode-to-city-api)
for reverse-geocoding your device location to a city name. Both are free and require no API key,
so the whole thing is a single static `index.html` with no build step, no framework, and no
server.

## Run locally

Just open `index.html` in a browser, or serve the folder with any static file server, e.g.:

```bash
npx serve .
```

## Deploy to GitHub Pages

1. Push this repo to GitHub.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to "Deploy from a branch", branch `main`,
   folder `/ (root)`.
4. Save — the page will be live at `https://<username>.github.io/<repo>/` within a minute or two.
