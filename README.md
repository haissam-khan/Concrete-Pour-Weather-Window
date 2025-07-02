# 🏗️ Concrete Pour Weather Window (Japan)

A bilingual web app that helps project managers in Japan assess if the next 48 hours are safe for a concrete pour. It evaluates hourly temperature, rain risk, and wind to provide a simple "Safe to Pour" gauge and professional curing advice based on **ACI (American Concrete Institute)** guidelines.

## 🎯 Why This Matters

Concrete placement requires very specific conditions to avoid cracking, delayed curing, or rework. But weather forecasts are often vague, especially in construction contexts. This tool gives actionable, localized insight for Japan-based teams.

## 💡 Features

- 🌐 **Bilingual Support (EN/JA)** — Switchable UI for local teams and global managers
- 📍 **Localized Geocoding** — Search by Japanese city or postal code
- 🕒 **48-Hour Hourly Forecast** — Evaluates each hour using Open-Meteo weather data
- 🚦 **Green/Red Safety Gauge** — Instantly shows whether it’s safe to pour
- 📊 **Detailed Forecast Table** — Flags conditions like:
  - 🌡️ **Too cold**: < 5°C  
  - 🔥 **Too hot**: > 35°C  
  - 🌧️ **Rain risk**: High probability or volume
- 🧠 **Curing Tips** — Real-world recommendations based on detected conditions
- 💻 Fully client-side, responsive, mobile-friendly

## 🛠️ Tech Stack

- **Frontend**: HTML, Tailwind CSS, Vanilla JavaScript
- **Weather API**: Open-Meteo (hourly forecast + geocoding)
- **Standards Used**: ACI (American Concrete Institute) thresholds for concrete pour conditions

## 🚀 How to Use

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/concrete-pour-weather-window.git
