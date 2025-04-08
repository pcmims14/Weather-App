# Q-SYS Weather App

A custom Q-SYS Weather App designed for real-time weather display using external weather data APIs. Built with Lua scripting inside Q-SYS Designer, this component can show temperature, weather conditions, and location info on a Q-SYS control interface.

## 🎯 Features

- 🌦️ Real-time weather updates via API (OpenWeatherMap or similar)
- 📍 Displays location, temperature, and condition
- 🔁 Periodic auto-refresh with adjustable update interval
- ✅ Integrated UI controls for manual refresh
- ⚙️ Easy-to-configure Lua backend
- 🛠️ Built using Q-SYS Designer

## 📁 Project Contents

- `Weather App.quc` – The main Q-SYS component with embedded Lua scripting and UI controls.
- `README.md` – You're looking at it.

## 🧰 Requirements

- Q-SYS Designer v9.5 or later
- Core running the Weather App component
- Internet access from Q-SYS Core (for API requests)
- An API key from a weather service (e.g., OpenWeatherMap)

## 🛠️ Setup Instructions

1. **Import the Component**  
   Open Q-SYS Designer and import `Weather App.quc` into your design.

2. **Edit the Lua Script (if needed)**  
   - Enter your API key and set the target location.
   - Adjust the refresh interval or endpoints as needed.

3. **Deploy the Design**  
   Push your design to a Core with internet access.

4. **Monitor Weather**  
   View real-time weather on the control interface. You can manually refresh or let it auto-update.

## 🧑‍💻 Configuration Example (Lua Snippet)

Inside the Lua script:
```lua
local api_key = "your_api_key_here"
local city = "New York"
local units = "imperial" -- or "metric"
local update_interval = 600 -- in seconds
