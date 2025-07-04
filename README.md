# 🏗️ Concrete Pour Weather Window | コンクリート打設可否判断ツール

A bilingual web app that helps teams in the EPC, infrastructure and construction sectors to conveniently check whether the next 48 hours are suitable for concrete pouring, using American Concrete Institute (ACI) guidelines and local weather data. Designed to promote safety, avoid rework, and support field decision-making across job sites.

## 🧠 What This Project Does

Users can enter any city name or Japanese postal code and instantly view:
- Hour-by-hour weather forecast (up to 48 hours)
- Color-coded gauge showing overall pour safety
- Risk flags based on rain, wind, and temperature
- Curing advice based on ACI concrete placement standards

This tool supports quick, informed decisions by supervisors, engineers, and project managers — especially when balancing site pressure with safe concrete placement.

## 🎯 Why It Matters

In EPC and construction projects, pouring concrete in unsuitable weather leads to cracking, curing delays, rework, and safety issues. Yet, site decisions are often made under pressure, without clear reference to global standards.

In my case, I particularly observed that Japan’s summer weather, with its high humidity and sudden rain, makes this especially risky.

This tool:
- Aligns decisions with **ACI guidance**  
- Provides **objective safety indicators**  
- Encourages **safe scheduling and documentation**

> 💡 I designed this app as part of our continuous safety efforts at Air Liquide Japan. It was also used during project planning and internal safety training sessions to demonstrate how global best practices can be made simple and accessible.

## 🚀 Features

- 🌐 **Bilingual Interface** — Toggle between English and Japanese
- 📍 **Geolocation Support** — Enter any city or postal code in Japan
- ⏱️ **48-Hour Forecast Table** — Temperature, precipitation, wind
- 🚦 **Pour Safety Gauge** — Instant green/red indicator
- 📋 **ACI-Based Risk Flags** — Too cold, too hot, rain risk, high wind
- 🧠 **Curing Tips** — Responsive suggestions based on detected risks
- 💬 **Tooltips, Thresholds, and Cautions** — All based on ACI guidance
- 📱 Responsive layout for mobile use at job sites

## 💡 ACI Weather Risk Thresholds

| Condition      | Threshold                      | Action                                 |
|----------------|--------------------------------|----------------------------------------|
| **Too Cold**   | Temp < 5°C                     | Use insulation, heat water/aggregates |
| **Too Hot**    | Temp > 35°C                    | Use set retarders, shading             |
| **Rain Risk**  | Precip. > 30% or > 0.25mm      | Protect forms and surfaces             |
| **High Wind**  | Wind > 25 m/s                  | Risk of cracking; use wind barriers    |

_These thresholds are derived from ACI (American Concrete Institute) guidance on hot and cold weather concrete placement._

## 🛠️ Tech Stack / Tools Used

- HTML, Tailwind CSS, Vanilla JavaScript  
- **Open-Meteo API** — Forecast and geolocation  
- ACI standard modeling — Safety logic based on temperature, rain, wind  
- Custom translation and UX system for bilingual rendering  

## 🌐 Live Demo

👉 [https://khanhaissam.github.io/concrete-pour-weather-window/](https://khanhaissam.github.io/concrete-pour-weather-window/)

## 🧪 How to Run This Project

> No setup needed — just clone and open `index.html` in your browser.

### 🔑 Step 1: Replace Weather API Key (Optional for Open-Meteo)

Open-Meteo works without authentication, but if you switch to OpenWeatherMap or another service, you’ll need to:

```js
const API_KEY = 'YOUR_OPENWEATHERMAP_API_KEY';
```

### 🗺️ Step 2: Use the Tool

1. Enter a **city name** or **postal code**  
2. Click **"Check Weather"**  
3. View the **safety gauge** and **forecast table**  
4. Read **ACI-based curing tips** when unsafe conditions are detected

