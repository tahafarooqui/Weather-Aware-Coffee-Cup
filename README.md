# ☕ Weather-Aware Coffee Cup — SVG Animated Sky, Seasons, and Freshness Meter

An interactive HTML, CSS, and JavaScript project that visualizes a coffee cup in a **dynamic SVG environment** that adapts in real time to **local weather conditions**.  
The scene changes with the **time of day, seasons, and weather effects**, while a **freshness meter** calculates how close your coffee is to the perfect temperature based on outside conditions.

[Demo:](https://tahafarooqui.github.io/Weather-Aware-Coffee-Cup/)

## ✨ Features

### 🌤 Dynamic SVG Sky
- Time-of-day modes: **day**, **night**, **dawn**, and **dusk**
- Seasonal themes: **summer**, **mild**, **cold**, **autumn**
- Weather effects: **clear**, **rain**, **snow**, **thunderstorm**, **fog**
- Animated elements: drifting clouds, lightning, snowflakes, raindrops, fog layers, falling leaves, fireflies

### ☕ Weather-Linked Coffee Cup
- Coffee level, color, and steam intensity linked to coffee temperature
- Cup color and steam opacity adapt based on outside temperature
- Iced coffee visuals for very hot days

### 📊 Coffee Freshness Meter
- Calculates the **optimal coffee temperature** based on outdoor weather
- Scores freshness from **0–100%**
- Mood indicator: Perfect, Good, Okay, Needs tweak
- Adjusts for humidity on hot days

### 🧩 User Controls
- JSON-based configuration for coffee properties:
```json
{
  "level": 0.75,
  "color": "#6f4e37",
  "temperatureC": 70,
  "surfaceColor": "#3b1f0e"
}
```
- Real-time **Apply** button to update visuals instantly

### 🌍 Live Weather Integration
- Uses [Open-Meteo API](https://open-meteo.com/) for real-time weather data
- Auto-detects location via Geolocation API
- Falls back to **London weather** if location is denied

---

## 🛠 Tech Stack
- **HTML5** — Structure & SVG graphics  
- **CSS3** — Styling, seasonal themes, and animations  
- **JavaScript (Vanilla)** — Weather logic, SVG manipulation, freshness scoring  
- **Open-Meteo API** — Weather data  
- **SVG** — Scalable vector-based graphics

---

## 🚀 Getting Started

### 1) Clone the Repository
```bash
git clone https://github.com/tahafarooqui/Weather-Aware-Coffee-Cup
cd weather-aware-coffee-cup
```

### 2) Open the App
Just open `index.html` in your favorite browser.

### 3) Allow Location Access
This enables **real-time weather adaptation**. If denied, London’s weather is used as a fallback.

### 4) Customize Your Coffee
- Edit the JSON in the text area
- Click **Apply** to see changes instantly

---

## ⚙️ How It Works

**Weather Detection**
- Geolocation → Open-Meteo fetch  
- Derives: season, daypart, condition (clear/rain/snow/thunder/fog), cloud cover, humidity, wind

**Scene Rendering**
- Toggles CSS classes for season, weather, and time of day  
- Animates clouds, rain, snow, fog, leaves, and fireflies as needed

**Coffee Adjustment**
- Links cup color & steam to outside temperature  
- Freshness meter estimates how close the coffee is to the ideal serving temperature

---

## 🧪 File Structure
```
.
├─ index.html
└─ README.md
```

---

## 📌 Potential Improvements
- °C / °F toggle
- Manual location input
- Persist coffee settings via LocalStorage
- Granular weather mappings per WMO codes
- Optional sound effects (rain, thunder, pouring)

---

## 📜 License
This project is licensed under the **MIT License** (add a `LICENSE` file if you plan to open-source).

---

## 🙌 Acknowledgements
- [Open-Meteo API](https://open-meteo.com/) for free weather data  
- Inspiration from creative coding & SVG animation communities
