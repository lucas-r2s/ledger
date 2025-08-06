---
title: Welcome to my blog
---

**API Name:** `WeatherTrack API`

**Purpose:** Provides real-time and historical weather data for a given location.

**Base URL:** `https://api.weathertrack.io/v1`

**Endpoints:**

| Method | Endpoint                                 | Description                        |
| ------ | ---------------------------------------- | ---------------------------------- |
| GET    | `/current?city={city}`                   | Get current weather for a city     |
| GET    | `/forecast?lat={lat}&lon={lon}`          | 7-day forecast for a geo point     |
| GET    | `/history?city={city}&date={yyyy-mm-dd}` | Historical data for a specific day |

**Example Response (`/current?city=Berlin`):**

```json
{
  "city": "Berlin",
  "temperature": 21.3,
  "condition": "Partly Cloudy",
  "humidity": 60,
  "wind_kph": 15.2,
  "timestamp": "2025-08-05T23:00:00Z"
}
```

**Auth:** Requires API key in `Authorization` header:
`Authorization: Bearer YOUR_API_KEY`

Think of it like a weather dashboard backend—you feed it location data, it feeds back clean, structured weather info.

