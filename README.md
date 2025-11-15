# 🌆 Smart City Dashboard

A simple and interactive Smart City Dashboard built using **HTML, CSS, JavaScript, Leaflet.js and Chart.js**.  
It allows users to search any city and view **Weather, Air Quality (AQI), PM2.5, PM10, Energy Consumption**, and simulated **Waste & Transport** data.

---

##  Features

- Search any city (Geocoding using Nominatim API)
-  Interactive Map (Leaflet + OpenStreetMap)
- Real-time Weather (Open-Meteo)
- Air Quality: AQI, PM2.5, PM10 (Open-Meteo Air Quality API)
- Energy Consumption (World Bank API)
- Waste & Transport Status (Simulated)
- Charts (AQI Trend, Energy Bar Chart, Waste Donut Chart)
- Dark Mode Toggle
- Auto-Refresh every 5 minutes
- Saves last searched city using LocalStorage

---

## 🧠 APIs Used

| API | Purpose | Example |
|------|---------|---------|
| **Nominatim (OpenStreetMap)** | City → Latitude/Longitude | `/search?format=json&q=Delhi` |
| **Open-Meteo Weather API** | Current weather | `/forecast?latitude=...&longitude=...&current_weather=true` |
| **Open-Meteo Air Quality API** | PM2.5, PM10, AQI | `/air-quality?hourly=pm2_5,pm10,us_aqi` |
| **World Bank API** | Energy use per capita | `/indicator/EG.USE.PCAP.KG.OE?format=json` |

---

## 🛠️ Tech Stack

- **HTML5 / CSS 
- **JavaScript 
- **Leaflet.js** (Maps)
- **Chart.js** (Charts)
- **OpenStreetMap**
- **Open-Meteo APIs**
- **World Bank API**

---

## 📂 Project Structure
📁 Smart-City-Dashboard
├── index.html
├── styles.css
├── script.js
└── README.md

---

## ⚙️ How to Run Locally

Because the app uses `fetch()`, run with a local server:

### Option 1: Python
```bash

---

📝 How It Works (Short Explanation)

User enters a city

App geocodes it → gets lat, lon

Map centers on that location

The dashboard fetches:

Weather data

Air quality data (PM2.5, PM10, AQI)

Country-level energy consumption

Charts update accordingly

Waste & transport are simulated values

The app remembers the last searched city using LocalStorage
