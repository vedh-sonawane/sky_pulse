SkyPulse — Real-Time Weather App

Stay ahead of the weather. Accurate forecasts, severe alerts, and beautiful visualizations for anywhere in the world.


🌤️ Overview
SkyPulse is a modern, beautifully designed weather application that delivers real-time weather data, hourly forecasts, and severe weather alerts for any location on Earth. Whether you're planning a weekend trip, deciding what to wear, or tracking an incoming storm, SkyPulse gives you everything you need in one clean, intuitive interface.
Built with a focus on accuracy, speed, and design, SkyPulse goes beyond basic temperature readings — offering air quality data, UV index, wind maps, precipitation radar, and personalized alerts so you're never caught off guard by the weather again.

✨ Features
🌡️ Real-Time Weather Data

Current temperature, feels like, humidity, and pressure
Wind speed, direction, and gusts
Visibility and cloud cover percentage
Dew point and atmospheric conditions
Updates every 15 minutes for maximum accuracy

📅 Forecasts

Hourly forecast for the next 48 hours
7-day extended forecast
Precipitation probability by the hour
High and low temperature ranges
Sunrise and sunset times for every day

🚨 Severe Weather Alerts

Real-time push notifications for storms, tornadoes, floods, and extreme heat
Government-issued weather warnings integrated directly into the app
Customizable alert thresholds — set your own temperature and wind limits
Emergency broadcast integration for your local area

🗺️ Weather Maps & Radar

Live precipitation radar with animated playback
Wind flow visualization maps
Temperature gradient maps
Cloud cover satellite imagery
Storm tracking with projected path

🌬️ Air Quality & Health

Air Quality Index (AQI) with health recommendations
Pollen count for allergy sufferers
UV index with sun protection advice
Humidity comfort levels
Best times to exercise outdoors

📍 Location Management

Auto-detect current location via GPS
Save multiple locations for quick switching
Search any city, town, or zip code worldwide
Home and work location shortcuts
Travel mode — auto-updates as you move

🎨 Beautiful UI

Dynamic backgrounds that change with weather conditions
Animated weather icons that reflect real conditions
Light and dark mode with automatic switching
Widget support for home screen quick glance
Minimalist design focused on readability

🌍 Global Coverage

Weather data for every country and territory
Localized units — Celsius/Fahrenheit, km/h or mph
Multi-language support
Time zone aware forecasts for travelers


🛠️ Tech Stack
LayerTechnologyFrontendNext.js 14, TypeScript, Tailwind CSSAnimationsFramer MotionMobileReact NativeBackendFastAPI, PythonWeather DataOpenWeatherMap API / WeatherAPIMaps & RadarMapbox GL JSNotificationsFirebase Cloud MessagingAuthNextAuth.jsDatabasePostgreSQLCachingRedis

📁 Project Structure
SkyPulse/
├── app/                          # Next.js App Router
│   ├── page.tsx                  # Homepage / current weather
│   ├── forecast/                 # Extended forecast page
│   ├── radar/                    # Live radar map
│   ├── alerts/                   # Severe weather alerts
│   ├── locations/                # Saved locations manager
│   └── settings/                 # User preferences
├── components/
│   ├── WeatherCard.tsx           # Current conditions card
│   ├── HourlyForecast.tsx        # Hourly forecast strip
│   ├── DailyForecast.tsx         # 7-day forecast list
│   ├── RadarMap.tsx              # Interactive radar map
│   ├── AirQuality.tsx            # AQI display component
│   ├── WeatherIcon.tsx           # Animated weather icons
│   └── AlertBanner.tsx           # Severe weather alert banner
├── backend/
│   ├── main.py                   # FastAPI app
│   ├── weather.py                # Weather data fetching
│   ├── alerts.py                 # Alert processing
│   ├── locations.py              # Location management
│   └── cache.py                  # Redis caching layer
├── lib/
│   ├── weather-api.ts            # Weather API client
│   └── utils.ts                  # Helper functions
└── package.json

⚙️ Setup & Installation
Prerequisites

Node.js 18+
Python 3.11+
A OpenWeatherMap API key (free at openweathermap.org)
A Mapbox API key (free at mapbox.com)
Firebase account for push notifications

1. Clone the Repository
bashgit clone https://github.com/yourusername/skypulse.git
cd skypulse
2. Install Frontend Dependencies
bashnpm install
3. Install Backend Dependencies
bashcd backend
python -m venv .venv
.venv\Scripts\activate
pip install fastapi uvicorn python-dotenv httpx redis
4. Configure Environment Variables
Create .env.local:
envNEXTAUTH_URL=http://localhost:3000
NEXTAUTH_SECRET=your_secret
OPENWEATHER_API_KEY=your_openweather_key
MAPBOX_API_KEY=your_mapbox_key
FIREBASE_API_KEY=your_firebase_key
DATABASE_URL=postgresql://user:password@localhost:5432/skypulse
Create backend/.env:
envOPENWEATHER_API_KEY=your_openweather_key
REDIS_URL=redis://localhost:6379
5. Start the Application
Terminal 1 — Backend:
bashcd backend
uvicorn main:app --reload --port 8000
Terminal 2 — Frontend:
bashnpm run dev
Open http://localhost:3000

🎯 Usage

Open SkyPulse and allow location access
See your current weather conditions instantly
Swipe through the hourly forecast for the next 48 hours
Check the 7-day forecast for trip planning
Open the radar map to track incoming precipitation
Save multiple locations for places you visit frequently
Set up custom alerts for conditions that matter to you


🔑 API Keys Required
ServicePurposeGet it hereOpenWeatherMapWeather data & forecastsopenweathermap.org/apiMapboxRadar & weather mapsmapbox.comFirebasePush notificationsfirebase.google.com

🗺️ Roadmap

 Apple Watch and Wear OS widgets
 Historical weather data and comparisons
 Agricultural weather mode for farmers
 Flight weather integration for travelers
 Ski resort snow conditions
 Beach and surf conditions
 Gardening planner based on weather forecast
 Smart home integration — auto-close windows when rain is detected


🌍 Why SkyPulse?
Weather affects every single day of our lives — what we wear, where we go, how we feel. Yet most weather apps are cluttered, inaccurate, or just plain ugly. SkyPulse was built to be the weather app that people actually enjoy using — one that's fast, accurate, beautiful, and genuinely useful whether you're a casual user just checking if it'll rain, or an outdoor enthusiast who needs detailed hourly wind and UV data.

🤝 Contributing
Contributions are welcome! Please open an issue first to discuss what you would like to change.

Fork the repository
Create your feature branch (git checkout -b feature/AmazingFeature)
Commit your changes (git commit -m 'Add AmazingFeature')
Push to the branch (git push origin feature/AmazingFeature)
Open a Pull Request


📄 License
MIT License — free to use, modify, and distribute.

🙏 Credits

OpenWeatherMap — Weather data provider
Mapbox — Maps and radar visualization
Firebase — Push notifications
Tailwind CSS — Styling
Framer Motion — Animations


Built with ❤️ by SkyPulse — Always know what's coming.
