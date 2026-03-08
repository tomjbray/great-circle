# Great Circle Route App

Plot the shortest flight path between any two airports on an interactive map.

## Files

```
great-circle.html   ← The app (open this in a browser)
airports.json       ← Airport database (~907 airports, must be in same folder)
README.md           ← This file
```

## How to run it locally (VS Code Live Server)

The app fetches `airports.json` at startup. Because of browser security rules,
this **only works via a web server** — double-clicking the HTML file won't work.

The easiest way is VS Code's Live Server extension:

1. Open the folder in VS Code (`File → Open Folder`)
2. Right-click `great-circle.html` in the Explorer panel
3. Click **"Open with Live Server"**
4. The app opens at `http://127.0.0.1:5500/great-circle.html`

## How to deploy on GitHub Pages (free, works from anywhere)

1. Create a free account at [github.com](https://github.com)
2. Click **New repository**, give it a name (e.g. `great-circle`), set it to **Public**
3. Upload all three files (`great-circle.html`, `airports.json`, `README.md`)
4. Go to **Settings → Pages**
5. Under "Branch", select `main` and click **Save**
6. After ~60 seconds your app is live at:
   `https://YOUR-USERNAME.github.io/great-circle/great-circle.html`

That's it — no server, no cost, accessible from any device.

## Adding more airports

`airports.json` is a plain JSON file. Each entry looks like:

```json
"LHR": ["Heathrow", "GB", "London", 51.4775, -0.4614]
```

The fields are: `[name, country_code, city, latitude, longitude]`

To add a missing airport, just add a new line in the same format and save the file.
You can find coordinates at [airportdb.io](https://airportdb.io) or 
[ourairports.com](https://ourairports.com).

## Current coverage (~907 airports)

- 🇬🇧 UK & Ireland (30+ airports including regional)
- 🇪🇺 Europe (200+ airports across all countries)  
- 🌍 Africa (80+ airports)
- 🌏 Asia & Middle East (200+ airports)
- 🌎 Americas (250+ airports)
- 🌊 Oceania & Pacific (60+ airports)
