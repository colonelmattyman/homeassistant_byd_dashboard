# BYD Sealion 7 — Home Assistant Dashboard

A visual Home Assistant dashboard for the BYD Sealion 7, featuring an interactive car graphic with live tyre pressure indicators, battery level display, door lock and window status overlays, climate control, live location map, and seat automation helpers.

![Dashboard Preview](preview.png)

---

## Features

- Layered car graphic with conditional overlays for tyre pressure warnings, door locks, and open windows
- Two battery display styles (Type 1: full-width graphic, Type 2: small icon)
- Animated charging bolt indicator
- Live tyre pressure readouts for all four corners with high/low alerts
- Seat heating and ventilation automation toggles
- Climate control thermostat card
- Live GPS map
- Garage camera feed via Frigate (optional)
- Auto-poll on dashboard load via Browser Mod
- Auto-poll on Android Auto connection (optional)

---

## Prerequisites

Install the following before proceeding. All HACS items require [HACS](https://hacs.xyz/) to be installed first.

| Requirement | Type | Notes |
|---|---|---|
| [BYD Vehicle Integration](https://github.com/danieldotnl/ha-byd-ev) | HACS Integration | Provides all `sensor.byd_sealion_7_*` entities |
| [Frigate Card](https://github.com/dermotduffy/frigate-hass-card) | HACS Frontend | Optional — only needed if you have a Frigate camera |
| [Browser Mod](https://github.com/thomasloven/hass-browser_mod) | HACS Integration | Required for auto-poll on dashboard page load |
| Local Media | Built-in HA integration | Must be enabled — check Settings → Integrations |

---

## Installation

### Step 1 — Copy Images

Copy the contents of the `images/` folder from this repo into your Home Assistant media folder:
