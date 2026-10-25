# SKYNETRED · Interstellar Open Source Intelligence

A live open-source intelligence console on a 3D globe. It runs on your own computer, opens in your web browser and
reads public, passive data only. Free for personal, non-commercial use.

![SkynetRED over Europe: ships, aircraft, pipelines, refineries, the Ukraine front line, disaster alerts](docs/globe.jpg)

![Lower Manhattan in 3D with street names](docs/city.jpg)

## What it shows

- **Air, sea, orbit:** live ships (AIS) and aircraft (ADS-B), tankers, military and private jets, satellites, GPS
  interference worked out from aircraft reports, vessels switching their transponder off (with a free key)
- **Hazards:** earthquakes with shaking maps, disaster alerts (cyclones, floods, droughts, volcanoes), active fires
  (with a free key), fireballs, space weather and aurora
- **Airspace and sea:** SIGMETs, US flight restrictions, navigational warnings
- **Energy:** refineries, LNG and petroleum terminals, offshore platforms, gas flaring, pipelines, the European power
  grid
- **Conflict:** conflict events, the Ukraine front line; incidents from the news; submarine cables; internet outages
  (with a free key)
- **Places:** country, city, town and street names, worldwide street and address search, 3D buildings with photos
  of the building you click, traffic cameras, your own location
- **Space:** the solar system live, the Deep Space Network, spacecraft, near-Earth asteroids, the Moon and Mars

## Download

Get the zip for your computer from the [latest release](../../releases/latest), unzip it, and keep the `SkynetRED`
executable and its `app` folder together.

| Computer | File |
| --- | --- |
| Mac with Apple Silicon (M1–M4) | `SkynetRED-<version>-macos-apple-silicon.zip` |
| Mac with Intel | `SkynetRED-<version>-macos-intel.zip` |
| Windows 10/11 (64-bit) | `SkynetRED-<version>-windows-x64.zip` |
| Linux (64-bit) | `SkynetRED-<version>-linux-x64.zip` |

`SHA256SUMS.txt` in the release lists each zip's checksum.

## Start

- **macOS:** double-click `SkynetRED`. The app is not signed with an Apple Developer ID, so the first time macOS says
  it cannot verify the developer: right-click (or Control-click) `SkynetRED` → **Open** → **Open**. If macOS only
  offers *Done*, open **System Settings → Privacy & Security** and click **Open Anyway** next to SkynetRED.
- **Windows:** double-click `SkynetRED.exe`. If SmartScreen warns, click **More info → Run anyway**.
- **Linux:** run `./SkynetRED`.

The console opens at <http://localhost:8787/geo/> in your default browser. Keep the window that opened running; close
it to stop SkynetRED.

## Optional keys

Most layers need nothing. A few free keys switch on more: copy `app/.env.example` to `app/.env` and fill in what you
want — NASA FIRMS (fires), Cloudflare Radar (internet outages), Global Fishing Watch (vessels going dark), Mapillary
(more building photos), aisstream.io (worldwide ships), and ArcGIS, Cesium ion or Google keys for sharper imagery and
photorealistic 3D cities. Keys stay on your computer.

## Privacy

Nothing is sent to the makers of SkynetRED. Your browser and SkynetRED's local server fetch public data directly from
the providers credited in the **Sources** panel. Text you search for goes to Photon (komoot); a building you click is
looked up on OpenStreetMap, Wikidata and Wikimedia Commons. Your location, if you ask for it, stays in your browser.

## Data and licences

Every source is credited in the app's **Sources** panel with its licence; several allow non-commercial use only. The
bundled energy data come from OGIM v3.0 (EDF / MethaneSAT, CC BY 4.0) and the European grid from OpenStreetMap
(© OpenStreetMap contributors, ODbL). Third-party software and data: [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt).

SkynetRED itself: [LICENSE.txt](LICENSE.txt) — free for personal, non-commercial use; the source code is not public.

Information shown comes from third-party public sources and may be incomplete, delayed or wrong. Do not rely on it for
navigation, safety, or decisions with legal or financial consequences. Not affiliated with any of the data providers.
