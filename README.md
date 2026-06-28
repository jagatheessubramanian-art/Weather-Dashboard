# 🌤️ WeatherNow — Premium Real-Time Weather Intelligence

![WeatherNow Premium Dashboard](https://img.shields.io/badge/UI-Glassmorphism-6366f1?style=for-the-badge) ![Vanilla JS](https://img.shields.io/badge/Vanilla-JavaScript-f7df1e?style=for-the-badge&logo=javascript&logoColor=black) ![Open-Meteo API](https://img.shields.io/badge/Powered%20By-Open--Meteo-0284c7?style=for-the-badge) ![Leaflet Maps](https://img.shields.io/badge/Interactive-Leaflet%20Maps-10b981?style=for-the-badge)

**WeatherNow** is a high-end, premium weather dashboard designed with rich glassmorphism aesthetics, dynamic background animations, and real-time interactive widgets. It provides lightning-fast access to accurate current conditions, 7-day forecasts, air quality indices (AQI), astronomical sun/moon cycles, and interactive weather maps—all in one beautifully crafted single-page web application.

---

## ✨ Features & Capabilities

### 🎨 Next-Generation Design & Ergonomics
- **Glassmorphism Aesthetics**: Elegant semi-transparent frosted glass cards with subtle border lighting, depth-enhancing blurs, and vibrant, harmonious HSL color palettes.
- **Flawless Dual Themes**: Seamlessly toggle between **Light Mode** (airy, bright celestial gradients) and **Dark Mode** (deep cosmic night skies) at the click of a button, persisting beautifully across sessions.
- **Dynamic Bottom Dock / Tab Bar**: 
  - On desktop viewports, navigation links and tool actions reside in a sleek floating island pill centered at the bottom of the screen.
  - On mobile viewports, the dock adapts intelligently into an ultra-slim single-row bottom tab bar with stacked icons and text, mirroring premium native iOS/Android applications.
- **Staggered Entrance Animations**: Weather widgets slide and fade into view using custom CSS keyframe choreography for a premium tactile feel.
- **3D Interactive Tilt**: Mouse tracking tilt effects on prominent weather cards bring the interface to life.

### 🌩️ Deep Weather & Environmental Intelligence
- **Live Current Conditions**: Real-time temperature, apparent "feels like" temperature, humidity, wind speed, surface pressure, visibility, and UV index.
- **Interactive Data Charts (Chart.js)**: Visualize 24-hour temperature curves and precipitation probability trends instantly.
- **Air Quality Index (AQI)**: Breakdown of US AQI values and granular pollutant levels (PM2.5, PM10, Carbon Monoxide, Nitrogen Dioxide, Sulphur Dioxide, Ozone).
- **Interactive Weather Maps (Leaflet.js)**: Pan and zoom across real-time maps with switchable layers (Standard Map, Satellite View, Temperature Heatmap, Wind Velocity, Precipitation Radar).
- **Sun & Moon Astronomy**: Precise sunrise/sunset timestamps paired with real-time calculated Moon Phases (e.g., *Waxing Gibbous*, *Waning Crescent*).
- **Live Weather Alerts**: Automated warnings for extreme weather events like Heat Waves, Heavy Storms, Freezing Fog, and High Winds.

### 🎙️ Advanced Search & Geolocation
- **Dual Geolocation Engines**: Leverages high-accuracy GPS reverse-geocoding via `api.bigdatacloud.net` with an automatic, instantaneous IP-based fallback (`get.geojs.io`) when browser location permissions are restricted.
- **Native Voice Search**: Tap the microphone icon in the hero search box to speak a city name using the Web Speech API, fully equipped with a fallback prompt dialog for restricted environments.
- **Intelligent Search History & Favorites**: Automatically bookmarks recent searches in a compact, scrollable chip container, and lets you star favorite cities for instant one-click access.
- **Native Share & Print**: Instantly copy weather summaries to your clipboard, invoke native mobile share sheets, or print clean weather reports directly from the dashboard.

---

## 🛠️ Technology Stack & Architecture

- **Core**: Vanilla HTML5, CSS3, and ES6 JavaScript (Zero heavy bundling required).
- **Weather Data Engine**: [Open-Meteo API](https://open-meteo.com) (Free, open-source weather & air quality APIs).
- **Mapping Engine**: [Leaflet.js](https://leafletjs.com) (Mobile-friendly interactive maps).
- **Charting Engine**: [Chart.js](https://www.chartjs.org) (Fast, responsive HTML5 canvas charting).
- **Iconography**: FontAwesome 6 Free.
- **Fonts**: Google Fonts (*Plus Jakarta Sans*).

---

## 🚀 Getting Started

Because **WeatherNow** is built using clean, highly optimized Vanilla web standards, running it is incredibly simple and requires no backend server or package installations.

### 1. Direct Browser Launch
Simply double-click the `index.html` file to open it in any modern web browser (Chrome, Edge, Firefox, Safari).

### 2. Running via Local Development Server (Recommended for Advanced APIs)
Some advanced browser capabilities (such as the native Web Speech API for voice search or strict geolocation permissions) function best when served over the `http://` protocol rather than `file://`.

If you have Visual Studio Code installed, simply use the **Live Server** extension, or run a quick local server using Python or Node:

```bash
# Using Python 3
python -m http.server 8000

# Using Node / npx
npx serve .
```

Then, open `http://localhost:8000` in your browser.

---

## 📱 Mobile Responsiveness & Optimization

WeatherNow has been meticulously tuned for mobile displays (`max-width: 600px`):
- **Space Optimization**: Tightened hero padding, compact scrollable search history chips (`max-height: 72px`), and optimized typography ensure essential data is visible instantly without endless scrolling.
- **Finger-Friendly Navigation**: The bottom navbar transitions into an easy-to-reach tab bar at the base of the screen, while the Floating Action Button (`#fab`) repositions to the right side above the bar to avoid content occlusion.
- **Touch-Optimized Charts & Maps**: Leaflet maps and Chart.js graphs automatically scale and adjust touch targets for seamless mobile swiping and inspection.

---

## 📜 License & Acknowledgements

- **Design & Engineering**: Developed by Jagathees.
- **Copyright**: © 2026 WeatherNow. All rights reserved.
- **Data Sources**: Weather data provided freely by Open-Meteo under non-commercial open licenses.
